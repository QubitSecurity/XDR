# 네트워크 격리 허용IP 등록

**Method:** `POST`  
**Endpoint:** `/account/isolation/allowip`  
**설명:** 네트워크 격리 허용IP 등록 API

---

## 요청(Request)

### 요청 항목(RequestBody)

- **`idAddress`** (String, 필수) : ip 주소
    
- **`description`** (String) : 설명
    
- **`serverId`** (Number, 필수) : 서버Id
    

### 요청 예시

```
/system/isolation/allowip

 ```

``` json
{
  "idAddress" : "192.129.221.1/32",
  "description" : "설명",
  "serverId" : 123
}

 ```

---

## 응답(Response)

### 응답 항목

- **`code`** (String) : 응답코드 (`0000`만 정상)
    
- **`message`** (String) : 응답 메시지
    
- **`data`** (JSON Object) : 응답 데이터
    

### 응답 예시

``` json
{
  "code": "0000",
  "message": "성공",
  "data": {}
}

 ```