# 네트워크 격리 허용 IP삭제

**Method:** `DELETE`  
**Endpoint:**`/system/isolation/allowip/{isolationAllowIpId}`  
**설명:** 네트워크 격리 허용Ip 삭제 API

---

## 요청(Request)

### 요청 항목(PathVariable)

- **`isolationAllowIpId`** (Number, 필수) : 네트워크 격리 허용IP id (네트워크 격리 허용IP 목록 조회 API 참조)
    

### 요청 예시

```
/system/isolation/allowip/7255

 ```

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