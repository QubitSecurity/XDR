# 원격제어

**Method:** `PUT`
**Endpoint:** `/system/servermanagementstatus/{serverId}`
**설명:** 원격제어 API

---

## 요청(Request)

### 요청 항목(PathVariable)

- **`serverId`** (String, 필수) : 서버id

### 요청 항목(RequestBody)

- **`type`** (String, 필수) : 원격제어 종류('networkIsolate', 'hostShutdown')
- **`isUse`** (boolean, 필수) : 사용여부

### 요청 예시

```
/system/servermanagementstatus/7255

```

---

## 응답(Response)

### 응답 항목

- **`code`** (String) : 응답코드 (`0000`만 정상)
- **`message`** (String) : 응답 메시지
- **`data`** (JSON Object) : 응답 데이터

### 응답 예시

```json
{
  "code": "0000",
  "message": "성공",
  "data": {}
}

```
