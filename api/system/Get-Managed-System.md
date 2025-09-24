# 시스템관리 개별 조회

**Method:** `GET`  
**Endpoint:** `/system/servers/{serverId}`  
**설명:** 시스템관리 개별 조회 API

---

## 요청(Request)

### 요청 항목(PathVariable)

- **`serverId`** (Number, 필수) : 서버id
    

### 요청 예시

```
/system/servers/7743

 ```

---

## 응답(Response)

### 응답 항목

- **`code`** (String) : 응답코드 (`0000`만 정상)
    
- **`message`** (String) : 응답 메시지
    
- **`data`** (JSON Object) : 응답 데이터
    
    - **`info`** (JSON Object) : 서버 정보
        
        - **`serverId`** (Number) : 서버id
            
        - **`serverIp`** (boolean) : 서버 IP주소
            
        - **`macAddress`** (int) : 장비 고유주소
            
        - **`osName`** (String) : OS 릴리즈 이름
            
        - **`osLatestVersion`** (String) : 업데이트 버전
            
        - **`createDatetime`** (String) : 등록일시
            
        - **`edrDetectMode`** (String) : EDR 탐지모드
            
        - **`edrBlockMode`** (String) : EDR 차단모드
            
        - **`modPluraType`** (String) : 모드프루라 종류
            
        - **`modPluraVersion`** (String) : 모드 프루라 버전
            
        - **`modPluraStatus`** (String) : 0: 삭제 완료 상태, 1: 동작중, 9: 삭제 진행중
            
        - **`displayAgentExecuteState`** (String) : 0: 모드프루라 설치되어 있지 않음, 10: 요청 (업데이트 요청), 20: 진행 (업데이트 진행중), 30: 완료 (업데이트 진행할 것이 없음), 40: 실패 (업데이트 해야 함),
            
        - **`logTypeSummary`** (String) : 로그유형 요약
            
        - **`agentType`** (String) : agent 타입
            
        - **`logConfigPathCountList`** (array) : 서버로그설정경로 목록
            
            - **`logType`** (String) : 로그타입
                
            - **`OnCount`** (String) : on count
                
            - **`OffCount`** (String) : off count
                
        - **`isEdrSysFullUpload`** (boolean) : 서버 모드(SERVER)와 에이전트 모드(EDR)중 에이전트 모드일 경우, 전체로그 수집 여부에 대한 설정값
            
        - **`isUseWebLog`** (boolean) : 웹로그 사용여부
            
        - **`isUseApplicationLog`** (boolean) : 어플리케이션 로그 사용여부
            
        - **`isSaveFullLog`** (boolean) : 전체로그 저장여부
            
        - **`isResourceUpload`** (boolean) : 시스템 업로드 사용여부
            
        - **`isWafBlockMode`** (boolean) : waf 차단 모드여부
            
        - **`wafUploadMode`** (String) : 웹방화벽 전송 설정 정보 - ﻿10 : 전체로그 (차단+ 탐지+그외), 20 : 차단+탐지로그, 30 : 차단로그
            

### 응답 예시

``` json
{
  "code": "0000",
  "message": "성공",
  "data": {
     "info": {
       "serverId": 8001,
       "serverIp": "192.168.0.101",
       "macAddress": "",
       "osName": "Android 11",
       "osLatestVersion": "1.3.0",
       "createDatetime": "2024-11-01 14:54:57",
       "edrDetectMode": "server",
       "edrBlockMode": "detect",
       "isEdrSysFullUpload": "0",
       "isUseWebLog": false,
       "modPluraType": "ModPlura-Apache",
       "modPluraVersion": "5.5.4",
       "modPluraStatus": "1",
       "displayAgentExecuteState": "40",
       "logConfigPathCountList": [
         {
           "logType": "system",
           "OnCount": "1",
           "OffCount": "0"
         }
       ],
       "logTypeSummary": "system",
       "agentType": "SIEM_C",
       "wafUploadMode": "10",
       "isWafBlockMode": false,
       "isUseApplicationLog": false,
       "isSaveFullLog": true,
       "isResourceUpload": true
     }
   }
}

 ```
