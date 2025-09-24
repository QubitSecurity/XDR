# 시스템관리 목록 조회

**Method:** `GET`  
**Endpoint:** `/system/servers`  
**설명:** 시스템관리 목록 조회 API

---

## 요청(Request)

### 요청 항목(Parameter)

- **`page`** (int, 선택) : 현재페이지
    
- **`size`** (int, 선택) : 사이즈
    
- **`sort`** (String, 선택) : 정렬순서 - serverId,desc : 날짜(최신순), serverId,asc : 날짜(과거순), serverIp,desc : 호스트(높은순), serverIp,asc : 호스트(낮은순)
    
- **`serverGroupIds`** (array, 선택) : 서버그룹id
    
- **`osTypes`** (array, 선택) : osTypeList
    
- **`serverIds`** (array, 선택) : 서버id
    
- **`logTypeSummary`** (String, 선택) : 로그유형 요약
    
- **`registerTypes`** (String, 선택) : 서버 등록방법(license : 라이선스, user : 직접)
    
- **`isSaveFullLog`** (boolean, 선택) : 전체로그 저장여부
    
- **`isAgentDel`** (boolean, 선택) : 에이전트 삭제여부
    
- **`summarySearch`** (String, 선택) : 등록 : all, on : isLogUploadOn, off : isLogUploadOff, 에이전트 : isAgentActive, osType : osType 코드, 웹방화벽 : isWaf
    
- **`serverIp`** (String, 선택) : 호스트
    
- **`hostname`** (String, 선택) : 호스트명
    
- **`createDatetime`** (String, 선택) : 등록일(yyyy-M-d H:m:s)
    
- **`serverName`** (String, 선택) : 별칭
    

### 요청 예시

```
/system/servers?page=1&size=20&sort=searverId|desc&serverGroupIds=&osTypes=&serverIds=&logTypeSummary=®isterTypes=&isSaveFullLog=&isAgentDel=&summarySearch=all=&serverIp=&hostname=&serverName=&createDateTime=2025-3-02 5:20:2

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
        
        - **`serverId`** (Number) : 서버id
            
        - **`agentType`** (String) : 에이전트 구분
            
        - **`agentVersion`** (String) : 에이전트 버전
            
        - **`serverGroupId`** (Number) : 서버그룹id
            
        - **`serverGroupName`** (String) : 서버그룹명
            
        - **`edrBlockMode`** (String) : EDR 차단모드
            
        - **`osType`** (String) : OS 종류이름
            
        - **`osName`** (String) : OS 이름
            
        - **`osLatestVersion`** (String) : 업데이트 버전
            
        - **`hostname`** (String) : 호스트명
            
        - **`serverName`** (String) : 별칭
            
        - **`serverIp`** (boolean) : 서버 IP주소
            
        - **`registerType`** (String) : 등록타입 -
            
        - **`logTypeSummaries`** (Arrays) :로그유형
            
        - **`createDatetime`** (String) : 등록일시
            
        - **`isEdrSysFullUpload`** (boolean) : 전체로그 수집여부
            
        - **`isSaveFullLog`** (boolean) : 전체로그 저장여부
            
        - **`isLogUpload`** (boolean) : 동작 ON/OFF
            
        - **`isAgentActive`** (boolean) : agent 활동여부
            
        - **`isUseWebLog`** (boolean) : 웹로그 사용여부
            
        - **`isUseSysLog`** (boolean) : 시스템 로그 사용여부
            
        - **`isUseApplicationLog`** (boolean) : 어플리케이션 로그 사용여부
            
        - **`isUseNetworkLog`** (boolean) : 네트워크 로그 사용여부
            
        - **`isUseAgent`** (boolean) : agent사용여부
            
        - **`isResourceUpload`** (boolean) : 시스템 업로드 사용여부
            
        - **`isAgentDelete`** (boolean) : 에이전트 삭제 여부
            

### 응답 예시

``` json
{
  "code": "0000",
  "message": "성공",
  "data": {
    "totalPage": 1,
    "totalCount": 1,
    "nowPage": 1,
    "list": [
      {
        "serverId": 8001,
        "agentType": "android",
        "agentVersion": "1.3.0",
        "serverGroupId": 18,
        "serverGroupName": "PC",
        "edrBlockMode": "detect",
        "isAgentActive": true,
        "osType": "android",
        "serverIp": "192.168.0.101",
        "hostname": "f338fd48577f5c8e",
        "serverName": "별칭",
        "osName" : "Rocky Linux release 8.9 (Green Obsidian)",
        "osLatestVersion" : "1.10.0-1127.19.1.el7.x86_64"
        "registerType" : "License"
        "logTypeSummaries": [
               "system",
               "web"
        ],
        "isEdrSysFullUpload": true,
        "isSaveFullLog": true,
        "isLogUpload": true,
        "isUseSysLog": true,
        "isUseWebLog": false,
        "isUseApplicationLog": false,
        "isUseNetworkLog": false,
        "isUseAgent": true,
        "isAgentDelete": false,
        "createDatetime": "2024-11-01 14:54:57"
      }
    ]
  }
}

 ```
