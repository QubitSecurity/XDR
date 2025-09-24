# 네트워크 격리 허용IP 목록 조회

**Method:** `GET`  
**Endpoint:** `/system/isolation/allowip/{serverId}`  
**설명:** 네트워크 격리 허용IP 목록 조회 API

---

## 요청(Request)

### 요청 항목(PathVariable)

- **`serverId`** (Number, 필수) : 서버id
    

### 요청 항목(Parameter)

- **`page`** (Number, 필수) : 현재페이지 (페이지 크기= 10)
    

### 요청 예시

```
/system/isolation/allowip/1043?page=1

 ```

---

## 응답(Response)

### 응답 항목

- **`code`** (String) : 응답코드 (`0000`만 정상)
    
- **`message`** (String) : 응답 메시지
    
- **`data`** (JSON Object) : 응답 데이터
    
    - **`totalPage`** (int) : 총 페이지수
        
    - **`totalCount`** (int) : 총 개수
        
    - **`nowPage`** (int) : 현재페이지 번호
        
    - **`list`** (JSON Array) : 서버 목록(페이징)
        
        - **`isolationAllowIpId`** (Number) : 네트워크 허용ip id
            
        - **`ipAddress`** (String) : ip 주소
            
        - **`description`** (String) : 설명
            
        - **`createBy`** (String) : 등록자
            
        - **`createDatetime`** (String) : 등록일시
            

### 응답 예시

``` json
{
    "code": "0000",
    "message": "success",
    "data": {
        "list": [
            {
                "isolationAllowIpId": 22,
                "ipAddress": "192.9.0.1/32",
                "description": "설명",
                "createBy": "AAA-toren",
                "createDatetime": "2025-09-08T06:53:50.000Z"
            },
            {
                "isolationAllowIpId": 21,
                "ipAddress": "192.8.0.1/32",
                "description": "설명",
                "createBy": "AAA-toren",
                "createDatetime": "2025-09-08T06:53:48.000Z"
            },
            {
                "isolationAllowIpId": 20,
                "ipAddress": "192.7.0.1/32",
                "description": "설명",
                "createBy": "AAA-toren",
                "createDatetime": "2025-09-08T06:53:44.000Z"
            },
            {
                "isolationAllowIpId": 19,
                "ipAddress": "192.6.0.1/32",
                "description": "설명",
                "createBy": "AAA-toren",
                "createDatetime": "2025-09-08T06:53:42.000Z"
            },
            {
                "isolationAllowIpId": 18,
                "ipAddress": "192.5.0.1/32",
                "description": "설명",
                "createBy": "AAA-toren",
                "createDatetime": "2025-09-08T06:53:39.000Z"
            },
            {
                "isolationAllowIpId": 17,
                "ipAddress": "192.4.0.1/32",
                "description": "설명",
                "createBy": "AAA-toren",
                "createDatetime": "2025-09-08T06:53:36.000Z"
            },
            {
                "isolationAllowIpId": 16,
                "ipAddress": "192.3.0.1/32",
                "description": "설명",
                "createBy": "AAA-toren",
                "createDatetime": "2025-09-08T06:53:34.000Z"
            },
            {
                "isolationAllowIpId": 15,
                "ipAddress": "192.2.0.1/32",
                "description": "설명",
                "createBy": "AAA-toren",
                "createDatetime": "2025-09-08T06:53:31.000Z"
            },
            {
                "isolationAllowIpId": 14,
                "ipAddress": "192.1.0.1/32",
                "description": "설명",
                "createBy": "AAA-toren",
                "createDatetime": "2025-09-08T06:53:28.000Z"
            },
            {
                "isolationAllowIpId": 13,
                "ipAddress": "192.0.0.1/32",
                "description": "설명",
                "createBy": "AAA-toren",
                "createDatetime": "2025-09-08T06:53:00.000Z"
            }
        ],
        "totalPage": 1,
        "totalCount": 10,
        "nowPage": 1
    }
}

 ```