# LF 회원 API


<a name="overview"></a>
## Overview
LF 회원 API Docs


### Version information
*Version* : 1.0


### License information
*Terms of service* : http://www.lfmall.co.kr


### URI scheme
*Host* : dev-napi.lfmall.co.kr  
*BasePath* : /swagger/customer


### Tags

* 입점 회원 : Supply Controller
* 입점 회원 로그인 : Login Controller
* 회원 공통 : Common Controller




<a name="paths"></a>
## Resources

<a name="a7ccb03ab0036624e95aa8f2a6c5e8de"></a>
### 입점 회원
Supply Controller


<a name="detailauthphonenousingget"></a>
#### 2단계 인증관리 조회
```
GET /customer/supply/v1/authPhoneNos/mgrId/{mgrId}
```


##### Description
설명 : 2단계 인증관리 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**mgrId**  <br>*required*|mgrId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«AuthPhoneDTO»](#fdc1fa6b8ac6e3e2dc764e0b734ec64f)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/supply/v1/authPhoneNos/mgrId/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : {
    "dpSphone1" : "string",
    "dpSphone10" : "string",
    "dpSphone11" : "string",
    "dpSphone12" : "string",
    "dpSphone13" : "string",
    "dpSphone14" : "string",
    "dpSphone15" : "string",
    "dpSphone16" : "string",
    "dpSphone17" : "string",
    "dpSphone18" : "string",
    "dpSphone19" : "string",
    "dpSphone2" : "string",
    "dpSphone20" : "string",
    "dpSphone3" : "string",
    "dpSphone4" : "string",
    "dpSphone5" : "string",
    "dpSphone6" : "string",
    "dpSphone7" : "string",
    "dpSphone8" : "string",
    "dpSphone9" : "string",
    "maxCnt" : 0,
    "mgrId" : "string",
    "sphone1" : "string",
    "sphone10" : "string",
    "sphone10UseYn" : "string",
    "sphone11" : "string",
    "sphone11UseYn" : "string",
    "sphone12" : "string",
    "sphone12UseYn" : "string",
    "sphone13" : "string",
    "sphone13UseYn" : "string",
    "sphone14" : "string",
    "sphone14UseYn" : "string",
    "sphone15" : "string",
    "sphone15UseYn" : "string",
    "sphone16" : "string",
    "sphone16UseYn" : "string",
    "sphone17" : "string",
    "sphone17UseYn" : "string",
    "sphone18" : "string",
    "sphone18UseYn" : "string",
    "sphone19" : "string",
    "sphone19UseYn" : "string",
    "sphone1UseYn" : "string",
    "sphone2" : "string",
    "sphone20" : "string",
    "sphone20UseYn" : "string",
    "sphone2UseYn" : "string",
    "sphone3" : "string",
    "sphone3UseYn" : "string",
    "sphone4" : "string",
    "sphone4UseYn" : "string",
    "sphone5" : "string",
    "sphone5UseYn" : "string",
    "sphone6" : "string",
    "sphone6UseYn" : "string",
    "sphone7" : "string",
    "sphone7UseYn" : "string",
    "sphone8" : "string",
    "sphone8UseYn" : "string",
    "sphone9" : "string",
    "sphone9UseYn" : "string"
  },
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="detailauthphonenosaveusingget"></a>
#### 2단계 인증관리 조회(저장을 위한)
```
GET /customer/supply/v1/authPhoneNos/mgrId/{mgrId}/save
```


##### Description
설명 : 2단계 인증관리 조회(저장을 위한)


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**mgrId**  <br>*required*|mgrId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«AuthPhoneDTO»](#fdc1fa6b8ac6e3e2dc764e0b734ec64f)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/supply/v1/authPhoneNos/mgrId/string/save
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : {
    "dpSphone1" : "string",
    "dpSphone10" : "string",
    "dpSphone11" : "string",
    "dpSphone12" : "string",
    "dpSphone13" : "string",
    "dpSphone14" : "string",
    "dpSphone15" : "string",
    "dpSphone16" : "string",
    "dpSphone17" : "string",
    "dpSphone18" : "string",
    "dpSphone19" : "string",
    "dpSphone2" : "string",
    "dpSphone20" : "string",
    "dpSphone3" : "string",
    "dpSphone4" : "string",
    "dpSphone5" : "string",
    "dpSphone6" : "string",
    "dpSphone7" : "string",
    "dpSphone8" : "string",
    "dpSphone9" : "string",
    "maxCnt" : 0,
    "mgrId" : "string",
    "sphone1" : "string",
    "sphone10" : "string",
    "sphone10UseYn" : "string",
    "sphone11" : "string",
    "sphone11UseYn" : "string",
    "sphone12" : "string",
    "sphone12UseYn" : "string",
    "sphone13" : "string",
    "sphone13UseYn" : "string",
    "sphone14" : "string",
    "sphone14UseYn" : "string",
    "sphone15" : "string",
    "sphone15UseYn" : "string",
    "sphone16" : "string",
    "sphone16UseYn" : "string",
    "sphone17" : "string",
    "sphone17UseYn" : "string",
    "sphone18" : "string",
    "sphone18UseYn" : "string",
    "sphone19" : "string",
    "sphone19UseYn" : "string",
    "sphone1UseYn" : "string",
    "sphone2" : "string",
    "sphone20" : "string",
    "sphone20UseYn" : "string",
    "sphone2UseYn" : "string",
    "sphone3" : "string",
    "sphone3UseYn" : "string",
    "sphone4" : "string",
    "sphone4UseYn" : "string",
    "sphone5" : "string",
    "sphone5UseYn" : "string",
    "sphone6" : "string",
    "sphone6UseYn" : "string",
    "sphone7" : "string",
    "sphone7UseYn" : "string",
    "sphone8" : "string",
    "sphone8UseYn" : "string",
    "sphone9" : "string",
    "sphone9UseYn" : "string"
  },
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="detailsupplycontractinfousingget"></a>
#### 계약정보 상세
```
GET /customer/supply/v1/contractInfo/supplyEntrCd/{supplyEntrCd}
```


##### Description
설명 : 계약정보 상세


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**supplyEntrCd**  <br>*required*|supplyEntrCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«SupplyContractInfoDTO»](#5c3ecb1ee3b9c98b1f4b3480fc85952b)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/supply/v1/contractInfo/supplyEntrCd/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : {
    "agreeDt" : "string",
    "agreeYn" : "string",
    "bizDtlAddr" : "string",
    "bizFixAddr" : "string",
    "bizNo" : "string",
    "contractNm" : "string",
    "ownerNm" : "string",
    "regDt" : "string",
    "status" : "string",
    "supplyEntrCd" : "string",
    "supplyEntrNm" : "string"
  },
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="listsupplycontractinfousingget"></a>
#### 계약정보 조회
```
GET /customer/supply/v1/contractInfos/supplyEntrCd/{supplyEntrCd}
```


##### Description
설명 : 계약정보 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**supplyEntrCd**  <br>*required*|supplyEntrCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«SupplyContractInfoDTO»»](#88cc75844f257dd714e8b456ff4ea7d1)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/supply/v1/contractInfos/supplyEntrCd/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : [ {
    "agreeDt" : "string",
    "agreeYn" : "string",
    "bizDtlAddr" : "string",
    "bizFixAddr" : "string",
    "bizNo" : "string",
    "contractNm" : "string",
    "ownerNm" : "string",
    "regDt" : "string",
    "status" : "string",
    "supplyEntrCd" : "string",
    "supplyEntrNm" : "string"
  } ],
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="createauthphonenousingpost"></a>
#### 2단계 인증관리 등록
```
POST /customer/supply/v1/createAuthPhoneNo
```


##### Description
설명 : 2단계 인증관리 등록


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**lstManager**  <br>*required*|lstManager|[LstManager](#lstmanager)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«int»](#3d8f4041e4ffd0ebb48bc9d2cf7190ed)|


##### Consumes

* `application/json`


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/supply/v1/createAuthPhoneNo
```


###### Request body
```json
{
  "chgEmail" : "string",
  "chgNm" : "string",
  "createOrderNo" : "string",
  "deptNm" : "string",
  "dpSphone1" : "string",
  "dpSphone10" : "string",
  "dpSphone11" : "string",
  "dpSphone12" : "string",
  "dpSphone13" : "string",
  "dpSphone14" : "string",
  "dpSphone15" : "string",
  "dpSphone16" : "string",
  "dpSphone17" : "string",
  "dpSphone18" : "string",
  "dpSphone19" : "string",
  "dpSphone2" : "string",
  "dpSphone20" : "string",
  "dpSphone3" : "string",
  "dpSphone4" : "string",
  "dpSphone5" : "string",
  "dpSphone6" : "string",
  "dpSphone7" : "string",
  "dpSphone8" : "string",
  "dpSphone9" : "string",
  "expYn" : "string",
  "extEntrCd" : "string",
  "extEntrNm" : "string",
  "inactiveYn" : "string",
  "initYn" : "string",
  "ipAddr" : "string",
  "ipChkYn" : "string",
  "irsftpUseYn" : "string",
  "linksiteCd" : "string",
  "linksiteNm" : "string",
  "loginFailCnt" : 0,
  "loginYn" : "string",
  "macAddr" : "string",
  "macUseYn" : "string",
  "maxCnt" : 0,
  "mgrId" : "string",
  "mgrNm" : "string",
  "newPasswd" : "string",
  "partNm" : "string",
  "passwd" : "string",
  "plinksiteCd" : "string",
  "pointGradeCd" : "string",
  "printGb" : "string",
  "regId" : "string",
  "result" : "string",
  "resultCnt" : 0,
  "roleCd" : "string",
  "roleNm" : "string",
  "sphone" : "string",
  "sphone1" : "string",
  "sphone10" : "string",
  "sphone10UseYn" : "string",
  "sphone11" : "string",
  "sphone11UseYn" : "string",
  "sphone12" : "string",
  "sphone12UseYn" : "string",
  "sphone13" : "string",
  "sphone13UseYn" : "string",
  "sphone14" : "string",
  "sphone14UseYn" : "string",
  "sphone15" : "string",
  "sphone15UseYn" : "string",
  "sphone16" : "string",
  "sphone16UseYn" : "string",
  "sphone17" : "string",
  "sphone17UseYn" : "string",
  "sphone18" : "string",
  "sphone18UseYn" : "string",
  "sphone19" : "string",
  "sphone19UseYn" : "string",
  "sphone1UseYn" : "string",
  "sphone2" : "string",
  "sphone20" : "string",
  "sphone20UseYn" : "string",
  "sphone2UseYn" : "string",
  "sphone3" : "string",
  "sphone3UseYn" : "string",
  "sphone4" : "string",
  "sphone4UseYn" : "string",
  "sphone5" : "string",
  "sphone5UseYn" : "string",
  "sphone6" : "string",
  "sphone6UseYn" : "string",
  "sphone7" : "string",
  "sphone7UseYn" : "string",
  "sphone8" : "string",
  "sphone8UseYn" : "string",
  "sphone9" : "string",
  "sphone9UseYn" : "string",
  "supplyEntrCd" : "string",
  "supplyEntrNm" : "string",
  "upId" : "string",
  "webGb" : "string"
}
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : 0,
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="createpartnerjoinusingput"></a>
#### 입점업체 등록
```
PUT /customer/supply/v1/createPartnerJoin
```


##### Description
설명 : 입점업체 등록


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**partnerJoinDTO**  <br>*required*|partnerJoinDTO|[PartnerJoinDTO](#partnerjoindto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«int»](#3d8f4041e4ffd0ebb48bc9d2cf7190ed)|


##### Consumes

* `application/json`


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/supply/v1/createPartnerJoin
```


###### Request body
```json
{
  "accountNm" : "string",
  "accountNo" : "string",
  "agreeYn" : "string",
  "bankCd" : "string",
  "bankNm" : "string",
  "bizDtlAddr" : "string",
  "bizFixAddr" : "string",
  "bizGb" : "string",
  "bizKind" : "string",
  "bizNo" : "string",
  "bizType" : "string",
  "bizZipNo" : "string",
  "bssnlcsAttachFile" : "string",
  "bssnlcsAttachFileUnique" : "string",
  "chgEmail" : "string",
  "chgHphone1" : "string",
  "chgHphone2" : "string",
  "chgHphone3" : "string",
  "chgNm" : "string",
  "cprpaccAttachFile" : "string",
  "cprpaccAttachFileUnique" : "string",
  "csOperatorEmail" : "string",
  "csOperatorNm" : "string",
  "csOperatorPhone1" : "string",
  "csOperatorPhone2" : "string",
  "csOperatorPhone3" : "string",
  "homeUrl" : "string",
  "ipAddr" : "string",
  "mgrId" : "string",
  "ownerNm" : "string",
  "passwd" : "string",
  "phone1" : "string",
  "phone2" : "string",
  "phone3" : "string",
  "prsformAttachFile" : "string",
  "prsformAttachFileUnique" : "string",
  "pymagrmAttachFile" : "string",
  "pymagrmAttachFileUnique" : "string",
  "sacOperatorEmail" : "string",
  "sacOperatorNm" : "string",
  "sacOperatorPhone1" : "string",
  "sacOperatorPhone2" : "string",
  "sacOperatorPhone3" : "string",
  "slctfcAttachFile" : "string",
  "slctfcAttachFileUnique" : "string",
  "stmtAttachFile" : "string",
  "stmtAttachFileUnique" : "string",
  "supplyEntrCd" : "string",
  "supplyEntrNm" : "string"
}
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : 0,
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="createpasswdchangehistoryusingpost"></a>
#### 비밀번호 변경 히스토리 저장
```
POST /customer/supply/v1/createPasswdChangeHistory
```


##### Description
설명 : 비밀번호 변경 히스토리 저장


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**passwdChangeHistoryDTO**  <br>*required*|passwdChangeHistoryDTO|[PasswdChangeHistoryDTO](#passwdchangehistorydto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«int»](#3d8f4041e4ffd0ebb48bc9d2cf7190ed)|


##### Consumes

* `application/json`


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/supply/v1/createPasswdChangeHistory
```


###### Request body
```json
{
  "creGb" : "string",
  "mgrId" : "string",
  "webGb" : "string"
}
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : 0,
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="getdbpasswordusingget"></a>
#### 비밀번호 조회
```
GET /customer/supply/v1/dbPassword/{mgrId}
```


##### Description
설명 : 비밀번호 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**mgrId**  <br>*required*|mgrId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«string»](#54534ab374d197cc878c0dd5cf11a3f9)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/supply/v1/dbPassword/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : "string",
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="detailencryptedpasswordusingget_1"></a>
#### 평문비밀번호를 암호화한 비밀번호 조회
```
GET /customer/supply/v1/encryptedPassword/{password}
```


##### Description
설명 : 평문비밀번호를 암호화한 비밀번호 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**password**  <br>*required*|password|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«string»](#54534ab374d197cc878c0dd5cf11a3f9)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/supply/v1/encryptedPassword/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : "string",
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="getentrappprovalynusingget"></a>
#### 입점승인 여부 조회
```
GET /customer/supply/v1/entrApprovalYn/mgrId/{mgrId}
```


##### Description
설명 : 입점승인 여부 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**mgrId**  <br>*required*|mgrId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«string»](#54534ab374d197cc878c0dd5cf11a3f9)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/supply/v1/entrApprovalYn/mgrId/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : "string",
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="getnecessaryconfirminfousingget"></a>
#### 메인페이지 - 필수 확인사항(판매수수료율, 약관동의)
```
GET /customer/supply/v1/necessaryConfirmInfo/supplyEntrCd/{supplyEntrCd}
```


##### Description
설명 : 메인페이지 - 필수 확인사항(판매수수료율, 약관동의)


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**supplyEntrCd**  <br>*required*|supplyEntrCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«NecessaryInfoDTO»](#e84dffa0b443eada5af8fad8a92c8e7d)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/supply/v1/necessaryConfirmInfo/supplyEntrCd/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : {
    "agreeYn" : "string",
    "sellFeeRateConfirmYn" : "string",
    "supplyEntrCd" : "string"
  },
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="getsupplyentriddupcheckusingget"></a>
#### 입점업체 아이디 중복체크
```
GET /customer/supply/v1/supplyEntr/mgrId/{mgrId}
```


##### Description
설명 : 입점업체 아이디 중복체크


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**mgrId**  <br>*required*|mgrId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«int»](#3d8f4041e4ffd0ebb48bc9d2cf7190ed)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/supply/v1/supplyEntr/mgrId/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : 0,
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="detailsupplyentrusingget"></a>
#### 계정정보 상세
```
GET /customer/supply/v1/supplyEntr/supplyEntrCd/{supplyEntrCd}
```


##### Description
설명 : 계정정보 상세


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**supplyEntrCd**  <br>*required*|supplyEntrCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«StbSupplyEntrDTO»](#10033ca1e0f3a32be9616dd5d1f6c3c4)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/supply/v1/supplyEntr/supplyEntrCd/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : {
    "accountCode" : "string",
    "accountNm" : "string",
    "accountNo" : "string",
    "bankNm" : "string",
    "bizDtlAddr" : "string",
    "bizFixAddr" : "string",
    "bizGb" : "string",
    "bizKind" : "string",
    "bizNo" : "string",
    "bizType" : "string",
    "bizZipNo" : "string",
    "chgEmail" : "string",
    "chgFax1" : "string",
    "chgFax2" : "string",
    "chgFax3" : "string",
    "chgHphone1" : "string",
    "chgHphone2" : "string",
    "chgHphone3" : "string",
    "chgNm" : "string",
    "csOperatorEmail" : "string",
    "csOperatorNm" : "string",
    "csOperatorPhone1" : "string",
    "csOperatorPhone2" : "string",
    "csOperatorPhone3" : "string",
    "entrStsCd" : "string",
    "entrStsNm" : "string",
    "fax1" : "string",
    "fax2" : "string",
    "fax3" : "string",
    "ownerNm" : "string",
    "phone1" : "string",
    "phone2" : "string",
    "phone3" : "string",
    "sacOperatorEmail" : "string",
    "sacOperatorNm" : "string",
    "sacOperatorPhone1" : "string",
    "sacOperatorPhone2" : "string",
    "sacOperatorPhone3" : "string",
    "sellFeeRate" : 0,
    "settleDay" : "string",
    "supplyEntrCd" : "string",
    "supplyEntrNm" : "string",
    "upId" : "string",
    "upSupplyEntrCd" : "string"
  },
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="updateauthphonenousingpatch"></a>
#### 2단계 인증관리 > 수정
```
PATCH /customer/supply/v1/updateAuthPhoneNo
```


##### Description
설명 : 2단계 인증관리 > 수정


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**authPhoneDTO**  <br>*required*|authPhoneDTO|[AuthPhoneDTO](#authphonedto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«int»](#3d8f4041e4ffd0ebb48bc9d2cf7190ed)|


##### Consumes

* `application/json`


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/supply/v1/updateAuthPhoneNo
```


###### Request body
```json
{
  "dpSphone1" : "string",
  "dpSphone10" : "string",
  "dpSphone11" : "string",
  "dpSphone12" : "string",
  "dpSphone13" : "string",
  "dpSphone14" : "string",
  "dpSphone15" : "string",
  "dpSphone16" : "string",
  "dpSphone17" : "string",
  "dpSphone18" : "string",
  "dpSphone19" : "string",
  "dpSphone2" : "string",
  "dpSphone20" : "string",
  "dpSphone3" : "string",
  "dpSphone4" : "string",
  "dpSphone5" : "string",
  "dpSphone6" : "string",
  "dpSphone7" : "string",
  "dpSphone8" : "string",
  "dpSphone9" : "string",
  "maxCnt" : 0,
  "mgrId" : "string",
  "sphone1" : "string",
  "sphone10" : "string",
  "sphone10UseYn" : "string",
  "sphone11" : "string",
  "sphone11UseYn" : "string",
  "sphone12" : "string",
  "sphone12UseYn" : "string",
  "sphone13" : "string",
  "sphone13UseYn" : "string",
  "sphone14" : "string",
  "sphone14UseYn" : "string",
  "sphone15" : "string",
  "sphone15UseYn" : "string",
  "sphone16" : "string",
  "sphone16UseYn" : "string",
  "sphone17" : "string",
  "sphone17UseYn" : "string",
  "sphone18" : "string",
  "sphone18UseYn" : "string",
  "sphone19" : "string",
  "sphone19UseYn" : "string",
  "sphone1UseYn" : "string",
  "sphone2" : "string",
  "sphone20" : "string",
  "sphone20UseYn" : "string",
  "sphone2UseYn" : "string",
  "sphone3" : "string",
  "sphone3UseYn" : "string",
  "sphone4" : "string",
  "sphone4UseYn" : "string",
  "sphone5" : "string",
  "sphone5UseYn" : "string",
  "sphone6" : "string",
  "sphone6UseYn" : "string",
  "sphone7" : "string",
  "sphone7UseYn" : "string",
  "sphone8" : "string",
  "sphone8UseYn" : "string",
  "sphone9" : "string",
  "sphone9UseYn" : "string"
}
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : 0,
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="updatepasswordusingpatch"></a>
#### 비밀번호 변경
```
PATCH /customer/supply/v1/updatePassword
```


##### Description
설명 : 비밀번호 변경


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**lstManager**  <br>*required*|lstManager|[LstManager](#lstmanager)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«int»](#3d8f4041e4ffd0ebb48bc9d2cf7190ed)|


##### Consumes

* `application/json`


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/supply/v1/updatePassword
```


###### Request body
```json
{
  "chgEmail" : "string",
  "chgNm" : "string",
  "createOrderNo" : "string",
  "deptNm" : "string",
  "dpSphone1" : "string",
  "dpSphone10" : "string",
  "dpSphone11" : "string",
  "dpSphone12" : "string",
  "dpSphone13" : "string",
  "dpSphone14" : "string",
  "dpSphone15" : "string",
  "dpSphone16" : "string",
  "dpSphone17" : "string",
  "dpSphone18" : "string",
  "dpSphone19" : "string",
  "dpSphone2" : "string",
  "dpSphone20" : "string",
  "dpSphone3" : "string",
  "dpSphone4" : "string",
  "dpSphone5" : "string",
  "dpSphone6" : "string",
  "dpSphone7" : "string",
  "dpSphone8" : "string",
  "dpSphone9" : "string",
  "expYn" : "string",
  "extEntrCd" : "string",
  "extEntrNm" : "string",
  "inactiveYn" : "string",
  "initYn" : "string",
  "ipAddr" : "string",
  "ipChkYn" : "string",
  "irsftpUseYn" : "string",
  "linksiteCd" : "string",
  "linksiteNm" : "string",
  "loginFailCnt" : 0,
  "loginYn" : "string",
  "macAddr" : "string",
  "macUseYn" : "string",
  "maxCnt" : 0,
  "mgrId" : "string",
  "mgrNm" : "string",
  "newPasswd" : "string",
  "partNm" : "string",
  "passwd" : "string",
  "plinksiteCd" : "string",
  "pointGradeCd" : "string",
  "printGb" : "string",
  "regId" : "string",
  "result" : "string",
  "resultCnt" : 0,
  "roleCd" : "string",
  "roleNm" : "string",
  "sphone" : "string",
  "sphone1" : "string",
  "sphone10" : "string",
  "sphone10UseYn" : "string",
  "sphone11" : "string",
  "sphone11UseYn" : "string",
  "sphone12" : "string",
  "sphone12UseYn" : "string",
  "sphone13" : "string",
  "sphone13UseYn" : "string",
  "sphone14" : "string",
  "sphone14UseYn" : "string",
  "sphone15" : "string",
  "sphone15UseYn" : "string",
  "sphone16" : "string",
  "sphone16UseYn" : "string",
  "sphone17" : "string",
  "sphone17UseYn" : "string",
  "sphone18" : "string",
  "sphone18UseYn" : "string",
  "sphone19" : "string",
  "sphone19UseYn" : "string",
  "sphone1UseYn" : "string",
  "sphone2" : "string",
  "sphone20" : "string",
  "sphone20UseYn" : "string",
  "sphone2UseYn" : "string",
  "sphone3" : "string",
  "sphone3UseYn" : "string",
  "sphone4" : "string",
  "sphone4UseYn" : "string",
  "sphone5" : "string",
  "sphone5UseYn" : "string",
  "sphone6" : "string",
  "sphone6UseYn" : "string",
  "sphone7" : "string",
  "sphone7UseYn" : "string",
  "sphone8" : "string",
  "sphone8UseYn" : "string",
  "sphone9" : "string",
  "sphone9UseYn" : "string",
  "supplyEntrCd" : "string",
  "supplyEntrNm" : "string",
  "upId" : "string",
  "webGb" : "string"
}
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : 0,
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="updatesupplyentrusingpatch"></a>
#### 계정정보 수정
```
PATCH /customer/supply/v1/updateSupplyEntr
```


##### Description
설명 : 계정정보 수정


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**stbSupplyEntrDTO**  <br>*required*|stbSupplyEntrDTO|[StbSupplyEntrDTO](#stbsupplyentrdto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«int»](#3d8f4041e4ffd0ebb48bc9d2cf7190ed)|


##### Consumes

* `application/json`


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/supply/v1/updateSupplyEntr
```


###### Request body
```json
{
  "accountCode" : "string",
  "accountNm" : "string",
  "accountNo" : "string",
  "bankNm" : "string",
  "bizDtlAddr" : "string",
  "bizFixAddr" : "string",
  "bizGb" : "string",
  "bizKind" : "string",
  "bizNo" : "string",
  "bizType" : "string",
  "bizZipNo" : "string",
  "chgEmail" : "string",
  "chgFax1" : "string",
  "chgFax2" : "string",
  "chgFax3" : "string",
  "chgHphone1" : "string",
  "chgHphone2" : "string",
  "chgHphone3" : "string",
  "chgNm" : "string",
  "csOperatorEmail" : "string",
  "csOperatorNm" : "string",
  "csOperatorPhone1" : "string",
  "csOperatorPhone2" : "string",
  "csOperatorPhone3" : "string",
  "entrStsCd" : "string",
  "entrStsNm" : "string",
  "fax1" : "string",
  "fax2" : "string",
  "fax3" : "string",
  "ownerNm" : "string",
  "phone1" : "string",
  "phone2" : "string",
  "phone3" : "string",
  "sacOperatorEmail" : "string",
  "sacOperatorNm" : "string",
  "sacOperatorPhone1" : "string",
  "sacOperatorPhone2" : "string",
  "sacOperatorPhone3" : "string",
  "sellFeeRate" : 0,
  "settleDay" : "string",
  "supplyEntrCd" : "string",
  "supplyEntrNm" : "string",
  "upId" : "string",
  "upSupplyEntrCd" : "string"
}
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : 0,
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="69cc83cd855dba10510deacfab65dfc7"></a>
### 입점 회원 로그인
Login Controller


<a name="createloginhistoryusingpost"></a>
#### 로그인이력 Insert
```
POST /customer/login/v1/createLoginHistory
```


##### Description
설명 : 로그인이력 Insert


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**loginDTO**  <br>*required*|loginDTO|[LoginDTO](#logindto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«int»](#3d8f4041e4ffd0ebb48bc9d2cf7190ed)|


##### Consumes

* `application/json`


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/login/v1/createLoginHistory
```


###### Request body
```json
{
  "deptNm" : "string",
  "extEntrCd" : "string",
  "extEntrNm" : "string",
  "ipAddr" : "string",
  "ipChkYn" : "string",
  "irsftpUseYn" : "string",
  "linksiteCd" : "string",
  "linksiteNm" : "string",
  "loginFailCnt" : 0,
  "loginYn" : "string",
  "macAddr" : "string",
  "macUseYn" : "string",
  "mgrId" : "string",
  "mgrNm" : "string",
  "partNm" : "string",
  "passwd" : "string",
  "plinksiteCd" : "string",
  "pointGradeCd" : "string",
  "printGb" : "string",
  "roleCd" : "string",
  "roleNm" : "string",
  "supplyEntrCd" : "string",
  "supplyEntrNm" : "string",
  "webGb" : "string"
}
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : 0,
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="getloginfailcntusingget"></a>
#### 로그인 실패 카운트
```
GET /customer/login/v1/logicFailCnt/loginId/{loginId}/ipAddr/{ipAddr}
```


##### Description
설명 : 로그인 실패 카운트


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**ipAddr**  <br>*required*|ipAddr|string|
|**Path**|**loginId**  <br>*required*|loginId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«int»](#3d8f4041e4ffd0ebb48bc9d2cf7190ed)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/login/v1/logicFailCnt/loginId/string/ipAddr/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : 0,
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="getloginauthnoexistsynusingget"></a>
#### 로그인 휴대폰 인증번호 존재여부 조회
```
GET /customer/login/v1/login/authNoExistsYn/mgrId/{mgrId}
```


##### Description
설명 : 로그인 휴대폰 인증번호 존재여부 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**mgrId**  <br>*required*|mgrId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«string»](#54534ab374d197cc878c0dd5cf11a3f9)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/login/v1/login/authNoExistsYn/mgrId/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : "string",
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="getloginusingget"></a>
#### 사용자 정보 조회
```
GET /customer/login/v1/login/loginId/{loginId}/ipAddr/{ipAddr}/webGb/{webGb}
```


##### Description
설명 : 사용자 정보 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**ipAddr**  <br>*required*|ipAddr|string|
|**Path**|**loginId**  <br>*required*|loginId|string|
|**Path**|**webGb**  <br>*required*|webGb|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«LoginDTO»](#ad2dcfef43ab20bd34db328c8ab73bee)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/login/v1/login/loginId/string/ipAddr/string/webGb/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : {
    "deptNm" : "string",
    "extEntrCd" : "string",
    "extEntrNm" : "string",
    "ipAddr" : "string",
    "ipChkYn" : "string",
    "irsftpUseYn" : "string",
    "linksiteCd" : "string",
    "linksiteNm" : "string",
    "loginFailCnt" : 0,
    "loginYn" : "string",
    "macAddr" : "string",
    "macUseYn" : "string",
    "mgrId" : "string",
    "mgrNm" : "string",
    "partNm" : "string",
    "passwd" : "string",
    "plinksiteCd" : "string",
    "pointGradeCd" : "string",
    "printGb" : "string",
    "roleCd" : "string",
    "roleNm" : "string",
    "supplyEntrCd" : "string",
    "supplyEntrNm" : "string",
    "webGb" : "string"
  },
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="getpasswdexpireusingput"></a>
#### 비밀번호 만료 체크
```
PUT /customer/login/v1/passwdExpire
```


##### Description
설명 : 비밀번호 만료 체크


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**lstManagerDto**  <br>*required*|lstManagerDto|[LstManagerDTO](#lstmanagerdto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«PasswordExpireDTO»](#df3a9eb8ae17f59fef9cf4dd911c8d2c)|


##### Consumes

* `application/json`


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/login/v1/passwdExpire
```


###### Request body
```json
{
  "createOrderNo" : "string",
  "deptNm" : "string",
  "expYn" : "string",
  "extEntrCd" : "string",
  "extEntrNm" : "string",
  "inactiveYn" : "string",
  "initYn" : "string",
  "ipAddr" : "string",
  "ipChkYn" : "string",
  "irsftpUseYn" : "string",
  "linksiteCd" : "string",
  "linksiteNm" : "string",
  "loginFailCnt" : 0,
  "loginYn" : "string",
  "macAddr" : "string",
  "macUseYn" : "string",
  "mgrId" : "string",
  "mgrNm" : "string",
  "newPasswd" : "string",
  "partNm" : "string",
  "passwd" : "string",
  "plinksiteCd" : "string",
  "pointGradeCd" : "string",
  "printGb" : "string",
  "regId" : "string",
  "roleCd" : "string",
  "roleNm" : "string",
  "sphone" : "string",
  "supplyEntrCd" : "string",
  "supplyEntrNm" : "string",
  "upId" : "string",
  "webGb" : "string"
}
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : {
    "expYn" : "string",
    "inactiveYn" : "string",
    "initYn" : "string"
  },
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="updatelastlogindateusingpatch"></a>
#### 최종로그인일시 수정
```
PATCH /customer/login/v1/updateLastLoginDate
```


##### Description
설명 : 최종로그인일시 수정


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**loginDTO**  <br>*required*|loginDTO|[LoginDTO](#logindto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«int»](#3d8f4041e4ffd0ebb48bc9d2cf7190ed)|


##### Consumes

* `application/json`


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/login/v1/updateLastLoginDate
```


###### Request body
```json
{
  "deptNm" : "string",
  "extEntrCd" : "string",
  "extEntrNm" : "string",
  "ipAddr" : "string",
  "ipChkYn" : "string",
  "irsftpUseYn" : "string",
  "linksiteCd" : "string",
  "linksiteNm" : "string",
  "loginFailCnt" : 0,
  "loginYn" : "string",
  "macAddr" : "string",
  "macUseYn" : "string",
  "mgrId" : "string",
  "mgrNm" : "string",
  "partNm" : "string",
  "passwd" : "string",
  "plinksiteCd" : "string",
  "pointGradeCd" : "string",
  "printGb" : "string",
  "roleCd" : "string",
  "roleNm" : "string",
  "supplyEntrCd" : "string",
  "supplyEntrNm" : "string",
  "webGb" : "string"
}
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : 0,
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="updateloginfailusingpatch"></a>
#### 로그인 성공시 로그인실패 카운트 0으로 세팅
```
PATCH /customer/login/v1/updateLoginFail
```


##### Description
설명 : 로그인 성공시 로그인실패 카운트 0으로 세팅


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**lstManagerDto**  <br>*required*|lstManagerDto|[LstManagerDTO](#lstmanagerdto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«int»](#3d8f4041e4ffd0ebb48bc9d2cf7190ed)|


##### Consumes

* `application/json`


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/login/v1/updateLoginFail
```


###### Request body
```json
{
  "createOrderNo" : "string",
  "deptNm" : "string",
  "expYn" : "string",
  "extEntrCd" : "string",
  "extEntrNm" : "string",
  "inactiveYn" : "string",
  "initYn" : "string",
  "ipAddr" : "string",
  "ipChkYn" : "string",
  "irsftpUseYn" : "string",
  "linksiteCd" : "string",
  "linksiteNm" : "string",
  "loginFailCnt" : 0,
  "loginYn" : "string",
  "macAddr" : "string",
  "macUseYn" : "string",
  "mgrId" : "string",
  "mgrNm" : "string",
  "newPasswd" : "string",
  "partNm" : "string",
  "passwd" : "string",
  "plinksiteCd" : "string",
  "pointGradeCd" : "string",
  "printGb" : "string",
  "regId" : "string",
  "roleCd" : "string",
  "roleNm" : "string",
  "sphone" : "string",
  "supplyEntrCd" : "string",
  "supplyEntrNm" : "string",
  "upId" : "string",
  "webGb" : "string"
}
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : 0,
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="6e94abdb647cc9956eb3b2af3c57af8e"></a>
### 회원 공통
Common Controller


<a name="executeaccountauthenticationusingput"></a>
#### 계좌인증
```
PUT /customer/common/v1/accountAuthentication
```


##### Description
설명 : 계좌인증


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**accountAuthenticationDTO**  <br>*required*|accountAuthenticationDTO|[AccountAuthenticationDTO](#accountauthenticationdto)|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«string»](#54534ab374d197cc878c0dd5cf11a3f9)|


##### Consumes

* `application/json`


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/common/v1/accountAuthentication
```


###### Request body
```json
{
  "accountNm" : "string",
  "accountNo" : "string",
  "bankCd" : "string"
}
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : "string",
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="listallowipusingget"></a>
#### 사내 IP주소 목록
```
GET /customer/common/v1/allowIp/groupCd/{groupCd}
```


##### Description
설명 : 사내 IP주소 목록


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**groupCd**  <br>*required*|groupCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«AllowIpDTO»»](#6337366a9d30d684b4fd862563b34869)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/common/v1/allowIp/groupCd/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : [ {
    "codeNm" : "string"
  } ],
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="listcodeusingget"></a>
#### 코드값 조회
```
GET /customer/common/v1/code/groupCd/{groupCd}
```


##### Description
설명 : 코드값 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**groupCd**  <br>*required*|groupCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«CodeDTO»»](#791a66e885021b66ebc2a4c839933f27)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/common/v1/code/groupCd/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : [ {
    "attrC1" : "string",
    "code" : "string",
    "codeDesc" : "string",
    "codeNm" : "string"
  } ],
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```


<a name="detailencryptedpasswordusingget"></a>
#### 평문비밀번호를 암호화한 비밀번호 조회
```
GET /customer/common/v1/password/{password}
```


##### Description
설명 : 평문비밀번호를 암호화한 비밀번호 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**password**  <br>*required*|password|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«string»](#54534ab374d197cc878c0dd5cf11a3f9)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/customer/common/v1/password/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : "string",
  "header" : {
    "additionalMessage" : "string",
    "status" : "string"
  },
  "paging" : {
    "gridId" : "string",
    "pagingIndex" : 0,
    "pagingTotalCount" : 0,
    "pagingWindowSize" : 0
  }
}
```




<a name="definitions"></a>
## Definitions

<a name="accountauthenticationdto"></a>
### AccountAuthenticationDTO

|Name|Description|Schema|
|---|---|---|
|**accountNm**  <br>*optional*|**Example** : `"string"`|string|
|**accountNo**  <br>*optional*|**Example** : `"string"`|string|
|**bankCd**  <br>*optional*|**Example** : `"string"`|string|


<a name="allowipdto"></a>
### AllowIpDTO

|Name|Description|Schema|
|---|---|---|
|**codeNm**  <br>*optional*|**Example** : `"string"`|string|


<a name="authphonedto"></a>
### AuthPhoneDTO

|Name|Description|Schema|
|---|---|---|
|**dpSphone1**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone10**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone11**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone12**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone13**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone14**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone15**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone16**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone17**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone18**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone19**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone2**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone20**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone3**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone4**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone5**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone6**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone7**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone8**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone9**  <br>*optional*|**Example** : `"string"`|string|
|**maxCnt**  <br>*optional*|**Example** : `0`|integer (int32)|
|**mgrId**  <br>*optional*|**Example** : `"string"`|string|
|**sphone1**  <br>*optional*|**Example** : `"string"`|string|
|**sphone10**  <br>*optional*|**Example** : `"string"`|string|
|**sphone10UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone11**  <br>*optional*|**Example** : `"string"`|string|
|**sphone11UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone12**  <br>*optional*|**Example** : `"string"`|string|
|**sphone12UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone13**  <br>*optional*|**Example** : `"string"`|string|
|**sphone13UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone14**  <br>*optional*|**Example** : `"string"`|string|
|**sphone14UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone15**  <br>*optional*|**Example** : `"string"`|string|
|**sphone15UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone16**  <br>*optional*|**Example** : `"string"`|string|
|**sphone16UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone17**  <br>*optional*|**Example** : `"string"`|string|
|**sphone17UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone18**  <br>*optional*|**Example** : `"string"`|string|
|**sphone18UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone19**  <br>*optional*|**Example** : `"string"`|string|
|**sphone19UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone1UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone2**  <br>*optional*|**Example** : `"string"`|string|
|**sphone20**  <br>*optional*|**Example** : `"string"`|string|
|**sphone20UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone2UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone3**  <br>*optional*|**Example** : `"string"`|string|
|**sphone3UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone4**  <br>*optional*|**Example** : `"string"`|string|
|**sphone4UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone5**  <br>*optional*|**Example** : `"string"`|string|
|**sphone5UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone6**  <br>*optional*|**Example** : `"string"`|string|
|**sphone6UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone7**  <br>*optional*|**Example** : `"string"`|string|
|**sphone7UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone8**  <br>*optional*|**Example** : `"string"`|string|
|**sphone8UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone9**  <br>*optional*|**Example** : `"string"`|string|
|**sphone9UseYn**  <br>*optional*|**Example** : `"string"`|string|


<a name="codedto"></a>
### CodeDTO

|Name|Description|Schema|
|---|---|---|
|**attrC1**  <br>*optional*|**Example** : `"string"`|string|
|**code**  <br>*optional*|**Example** : `"string"`|string|
|**codeDesc**  <br>*optional*|**Example** : `"string"`|string|
|**codeNm**  <br>*optional*|**Example** : `"string"`|string|


<a name="lfdcheader"></a>
### LfdcHeader

|Name|Description|Schema|
|---|---|---|
|**additionalMessage**  <br>*optional*|**Example** : `"string"`|string|
|**status**  <br>*optional*|**Example** : `"string"`|string|


<a name="fdc1fa6b8ac6e3e2dc764e0b734ec64f"></a>
### LfdcResponse«AuthPhoneDTO»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `"[authphonedto](#authphonedto)"`|[AuthPhoneDTO](#authphonedto)|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="6337366a9d30d684b4fd862563b34869"></a>
### LfdcResponse«List«AllowIpDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[allowipdto](#allowipdto)" ]`|< [AllowIpDTO](#allowipdto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="791a66e885021b66ebc2a4c839933f27"></a>
### LfdcResponse«List«CodeDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[codedto](#codedto)" ]`|< [CodeDTO](#codedto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="88cc75844f257dd714e8b456ff4ea7d1"></a>
### LfdcResponse«List«SupplyContractInfoDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[supplycontractinfodto](#supplycontractinfodto)" ]`|< [SupplyContractInfoDTO](#supplycontractinfodto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="ad2dcfef43ab20bd34db328c8ab73bee"></a>
### LfdcResponse«LoginDTO»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `"[logindto](#logindto)"`|[LoginDTO](#logindto)|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="e84dffa0b443eada5af8fad8a92c8e7d"></a>
### LfdcResponse«NecessaryInfoDTO»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `"[necessaryinfodto](#necessaryinfodto)"`|[NecessaryInfoDTO](#necessaryinfodto)|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="df3a9eb8ae17f59fef9cf4dd911c8d2c"></a>
### LfdcResponse«PasswordExpireDTO»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `"[passwordexpiredto](#passwordexpiredto)"`|[PasswordExpireDTO](#passwordexpiredto)|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="10033ca1e0f3a32be9616dd5d1f6c3c4"></a>
### LfdcResponse«StbSupplyEntrDTO»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `"[stbsupplyentrdto](#stbsupplyentrdto)"`|[StbSupplyEntrDTO](#stbsupplyentrdto)|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="5c3ecb1ee3b9c98b1f4b3480fc85952b"></a>
### LfdcResponse«SupplyContractInfoDTO»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `"[supplycontractinfodto](#supplycontractinfodto)"`|[SupplyContractInfoDTO](#supplycontractinfodto)|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="3d8f4041e4ffd0ebb48bc9d2cf7190ed"></a>
### LfdcResponse«int»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `0`|integer (int32)|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="54534ab374d197cc878c0dd5cf11a3f9"></a>
### LfdcResponse«string»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `"string"`|string|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="logindto"></a>
### LoginDTO

|Name|Description|Schema|
|---|---|---|
|**deptNm**  <br>*optional*|**Example** : `"string"`|string|
|**extEntrCd**  <br>*optional*|**Example** : `"string"`|string|
|**extEntrNm**  <br>*optional*|**Example** : `"string"`|string|
|**ipAddr**  <br>*optional*|**Example** : `"string"`|string|
|**ipChkYn**  <br>*optional*|**Example** : `"string"`|string|
|**irsftpUseYn**  <br>*optional*|**Example** : `"string"`|string|
|**linksiteCd**  <br>*optional*|**Example** : `"string"`|string|
|**linksiteNm**  <br>*optional*|**Example** : `"string"`|string|
|**loginFailCnt**  <br>*optional*|**Example** : `0`|integer (int32)|
|**loginYn**  <br>*optional*|**Example** : `"string"`|string|
|**macAddr**  <br>*optional*|**Example** : `"string"`|string|
|**macUseYn**  <br>*optional*|**Example** : `"string"`|string|
|**mgrId**  <br>*optional*|**Example** : `"string"`|string|
|**mgrNm**  <br>*optional*|**Example** : `"string"`|string|
|**partNm**  <br>*optional*|**Example** : `"string"`|string|
|**passwd**  <br>*optional*|**Example** : `"string"`|string|
|**plinksiteCd**  <br>*optional*|**Example** : `"string"`|string|
|**pointGradeCd**  <br>*optional*|**Example** : `"string"`|string|
|**printGb**  <br>*optional*|**Example** : `"string"`|string|
|**roleCd**  <br>*optional*|**Example** : `"string"`|string|
|**roleNm**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrCd**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrNm**  <br>*optional*|**Example** : `"string"`|string|
|**webGb**  <br>*optional*|**Example** : `"string"`|string|


<a name="lstmanager"></a>
### LstManager

|Name|Description|Schema|
|---|---|---|
|**chgEmail**  <br>*optional*|**Example** : `"string"`|string|
|**chgNm**  <br>*optional*|**Example** : `"string"`|string|
|**createOrderNo**  <br>*optional*|**Example** : `"string"`|string|
|**deptNm**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone1**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone10**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone11**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone12**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone13**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone14**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone15**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone16**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone17**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone18**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone19**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone2**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone20**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone3**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone4**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone5**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone6**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone7**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone8**  <br>*optional*|**Example** : `"string"`|string|
|**dpSphone9**  <br>*optional*|**Example** : `"string"`|string|
|**expYn**  <br>*optional*|**Example** : `"string"`|string|
|**extEntrCd**  <br>*optional*|**Example** : `"string"`|string|
|**extEntrNm**  <br>*optional*|**Example** : `"string"`|string|
|**inactiveYn**  <br>*optional*|**Example** : `"string"`|string|
|**initYn**  <br>*optional*|**Example** : `"string"`|string|
|**ipAddr**  <br>*optional*|**Example** : `"string"`|string|
|**ipChkYn**  <br>*optional*|**Example** : `"string"`|string|
|**irsftpUseYn**  <br>*optional*|**Example** : `"string"`|string|
|**linksiteCd**  <br>*optional*|**Example** : `"string"`|string|
|**linksiteNm**  <br>*optional*|**Example** : `"string"`|string|
|**loginFailCnt**  <br>*optional*|**Example** : `0`|integer (int32)|
|**loginYn**  <br>*optional*|**Example** : `"string"`|string|
|**macAddr**  <br>*optional*|**Example** : `"string"`|string|
|**macUseYn**  <br>*optional*|**Example** : `"string"`|string|
|**maxCnt**  <br>*optional*|**Example** : `0`|integer (int32)|
|**mgrId**  <br>*optional*|**Example** : `"string"`|string|
|**mgrNm**  <br>*optional*|**Example** : `"string"`|string|
|**newPasswd**  <br>*optional*|**Example** : `"string"`|string|
|**partNm**  <br>*optional*|**Example** : `"string"`|string|
|**passwd**  <br>*optional*|**Example** : `"string"`|string|
|**plinksiteCd**  <br>*optional*|**Example** : `"string"`|string|
|**pointGradeCd**  <br>*optional*|**Example** : `"string"`|string|
|**printGb**  <br>*optional*|**Example** : `"string"`|string|
|**regId**  <br>*optional*|**Example** : `"string"`|string|
|**result**  <br>*optional*|**Example** : `"string"`|string|
|**resultCnt**  <br>*optional*|**Example** : `0`|integer (int32)|
|**roleCd**  <br>*optional*|**Example** : `"string"`|string|
|**roleNm**  <br>*optional*|**Example** : `"string"`|string|
|**sphone**  <br>*optional*|**Example** : `"string"`|string|
|**sphone1**  <br>*optional*|**Example** : `"string"`|string|
|**sphone10**  <br>*optional*|**Example** : `"string"`|string|
|**sphone10UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone11**  <br>*optional*|**Example** : `"string"`|string|
|**sphone11UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone12**  <br>*optional*|**Example** : `"string"`|string|
|**sphone12UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone13**  <br>*optional*|**Example** : `"string"`|string|
|**sphone13UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone14**  <br>*optional*|**Example** : `"string"`|string|
|**sphone14UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone15**  <br>*optional*|**Example** : `"string"`|string|
|**sphone15UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone16**  <br>*optional*|**Example** : `"string"`|string|
|**sphone16UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone17**  <br>*optional*|**Example** : `"string"`|string|
|**sphone17UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone18**  <br>*optional*|**Example** : `"string"`|string|
|**sphone18UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone19**  <br>*optional*|**Example** : `"string"`|string|
|**sphone19UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone1UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone2**  <br>*optional*|**Example** : `"string"`|string|
|**sphone20**  <br>*optional*|**Example** : `"string"`|string|
|**sphone20UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone2UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone3**  <br>*optional*|**Example** : `"string"`|string|
|**sphone3UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone4**  <br>*optional*|**Example** : `"string"`|string|
|**sphone4UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone5**  <br>*optional*|**Example** : `"string"`|string|
|**sphone5UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone6**  <br>*optional*|**Example** : `"string"`|string|
|**sphone6UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone7**  <br>*optional*|**Example** : `"string"`|string|
|**sphone7UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone8**  <br>*optional*|**Example** : `"string"`|string|
|**sphone8UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**sphone9**  <br>*optional*|**Example** : `"string"`|string|
|**sphone9UseYn**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrCd**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrNm**  <br>*optional*|**Example** : `"string"`|string|
|**upId**  <br>*optional*|**Example** : `"string"`|string|
|**webGb**  <br>*optional*|**Example** : `"string"`|string|


<a name="lstmanagerdto"></a>
### LstManagerDTO

|Name|Description|Schema|
|---|---|---|
|**createOrderNo**  <br>*optional*|**Example** : `"string"`|string|
|**deptNm**  <br>*optional*|**Example** : `"string"`|string|
|**expYn**  <br>*optional*|**Example** : `"string"`|string|
|**extEntrCd**  <br>*optional*|**Example** : `"string"`|string|
|**extEntrNm**  <br>*optional*|**Example** : `"string"`|string|
|**inactiveYn**  <br>*optional*|**Example** : `"string"`|string|
|**initYn**  <br>*optional*|**Example** : `"string"`|string|
|**ipAddr**  <br>*optional*|**Example** : `"string"`|string|
|**ipChkYn**  <br>*optional*|**Example** : `"string"`|string|
|**irsftpUseYn**  <br>*optional*|**Example** : `"string"`|string|
|**linksiteCd**  <br>*optional*|**Example** : `"string"`|string|
|**linksiteNm**  <br>*optional*|**Example** : `"string"`|string|
|**loginFailCnt**  <br>*optional*|**Example** : `0`|integer (int32)|
|**loginYn**  <br>*optional*|**Example** : `"string"`|string|
|**macAddr**  <br>*optional*|**Example** : `"string"`|string|
|**macUseYn**  <br>*optional*|**Example** : `"string"`|string|
|**mgrId**  <br>*optional*|**Example** : `"string"`|string|
|**mgrNm**  <br>*optional*|**Example** : `"string"`|string|
|**newPasswd**  <br>*optional*|**Example** : `"string"`|string|
|**partNm**  <br>*optional*|**Example** : `"string"`|string|
|**passwd**  <br>*optional*|**Example** : `"string"`|string|
|**plinksiteCd**  <br>*optional*|**Example** : `"string"`|string|
|**pointGradeCd**  <br>*optional*|**Example** : `"string"`|string|
|**printGb**  <br>*optional*|**Example** : `"string"`|string|
|**regId**  <br>*optional*|**Example** : `"string"`|string|
|**roleCd**  <br>*optional*|**Example** : `"string"`|string|
|**roleNm**  <br>*optional*|**Example** : `"string"`|string|
|**sphone**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrCd**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrNm**  <br>*optional*|**Example** : `"string"`|string|
|**upId**  <br>*optional*|**Example** : `"string"`|string|
|**webGb**  <br>*optional*|**Example** : `"string"`|string|


<a name="necessaryinfodto"></a>
### NecessaryInfoDTO

|Name|Description|Schema|
|---|---|---|
|**agreeYn**  <br>*optional*|**Example** : `"string"`|string|
|**sellFeeRateConfirmYn**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrCd**  <br>*optional*|**Example** : `"string"`|string|


<a name="paginginfo"></a>
### PagingInfo

|Name|Description|Schema|
|---|---|---|
|**gridId**  <br>*optional*|**Example** : `"string"`|string|
|**pagingIndex**  <br>*optional*|**Example** : `0`|integer (int32)|
|**pagingTotalCount**  <br>*optional*|**Example** : `0`|integer (int32)|
|**pagingWindowSize**  <br>*optional*|**Example** : `0`|integer (int32)|


<a name="partnerjoindto"></a>
### PartnerJoinDTO

|Name|Description|Schema|
|---|---|---|
|**accountNm**  <br>*optional*|**Example** : `"string"`|string|
|**accountNo**  <br>*optional*|**Example** : `"string"`|string|
|**agreeYn**  <br>*optional*|**Example** : `"string"`|string|
|**bankCd**  <br>*optional*|**Example** : `"string"`|string|
|**bankNm**  <br>*optional*|**Example** : `"string"`|string|
|**bizDtlAddr**  <br>*optional*|**Example** : `"string"`|string|
|**bizFixAddr**  <br>*optional*|**Example** : `"string"`|string|
|**bizGb**  <br>*optional*|**Example** : `"string"`|string|
|**bizKind**  <br>*optional*|**Example** : `"string"`|string|
|**bizNo**  <br>*optional*|**Example** : `"string"`|string|
|**bizType**  <br>*optional*|**Example** : `"string"`|string|
|**bizZipNo**  <br>*optional*|**Example** : `"string"`|string|
|**bssnlcsAttachFile**  <br>*optional*|**Example** : `"string"`|string|
|**bssnlcsAttachFileUnique**  <br>*optional*|**Example** : `"string"`|string|
|**chgEmail**  <br>*optional*|**Example** : `"string"`|string|
|**chgHphone1**  <br>*optional*|**Example** : `"string"`|string|
|**chgHphone2**  <br>*optional*|**Example** : `"string"`|string|
|**chgHphone3**  <br>*optional*|**Example** : `"string"`|string|
|**chgNm**  <br>*optional*|**Example** : `"string"`|string|
|**cprpaccAttachFile**  <br>*optional*|**Example** : `"string"`|string|
|**cprpaccAttachFileUnique**  <br>*optional*|**Example** : `"string"`|string|
|**csOperatorEmail**  <br>*optional*|**Example** : `"string"`|string|
|**csOperatorNm**  <br>*optional*|**Example** : `"string"`|string|
|**csOperatorPhone1**  <br>*optional*|**Example** : `"string"`|string|
|**csOperatorPhone2**  <br>*optional*|**Example** : `"string"`|string|
|**csOperatorPhone3**  <br>*optional*|**Example** : `"string"`|string|
|**homeUrl**  <br>*optional*|**Example** : `"string"`|string|
|**ipAddr**  <br>*optional*|**Example** : `"string"`|string|
|**mgrId**  <br>*optional*|**Example** : `"string"`|string|
|**ownerNm**  <br>*optional*|**Example** : `"string"`|string|
|**passwd**  <br>*optional*|**Example** : `"string"`|string|
|**phone1**  <br>*optional*|**Example** : `"string"`|string|
|**phone2**  <br>*optional*|**Example** : `"string"`|string|
|**phone3**  <br>*optional*|**Example** : `"string"`|string|
|**prsformAttachFile**  <br>*optional*|**Example** : `"string"`|string|
|**prsformAttachFileUnique**  <br>*optional*|**Example** : `"string"`|string|
|**pymagrmAttachFile**  <br>*optional*|**Example** : `"string"`|string|
|**pymagrmAttachFileUnique**  <br>*optional*|**Example** : `"string"`|string|
|**sacOperatorEmail**  <br>*optional*|**Example** : `"string"`|string|
|**sacOperatorNm**  <br>*optional*|**Example** : `"string"`|string|
|**sacOperatorPhone1**  <br>*optional*|**Example** : `"string"`|string|
|**sacOperatorPhone2**  <br>*optional*|**Example** : `"string"`|string|
|**sacOperatorPhone3**  <br>*optional*|**Example** : `"string"`|string|
|**slctfcAttachFile**  <br>*optional*|**Example** : `"string"`|string|
|**slctfcAttachFileUnique**  <br>*optional*|**Example** : `"string"`|string|
|**stmtAttachFile**  <br>*optional*|**Example** : `"string"`|string|
|**stmtAttachFileUnique**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrCd**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrNm**  <br>*optional*|**Example** : `"string"`|string|


<a name="passwdchangehistorydto"></a>
### PasswdChangeHistoryDTO

|Name|Description|Schema|
|---|---|---|
|**creGb**  <br>*optional*|**Example** : `"string"`|string|
|**mgrId**  <br>*optional*|**Example** : `"string"`|string|
|**webGb**  <br>*optional*|**Example** : `"string"`|string|


<a name="passwordexpiredto"></a>
### PasswordExpireDTO

|Name|Description|Schema|
|---|---|---|
|**expYn**  <br>*optional*|**Example** : `"string"`|string|
|**inactiveYn**  <br>*optional*|**Example** : `"string"`|string|
|**initYn**  <br>*optional*|**Example** : `"string"`|string|


<a name="stbsupplyentrdto"></a>
### StbSupplyEntrDTO

|Name|Description|Schema|
|---|---|---|
|**accountCode**  <br>*optional*|**Example** : `"string"`|string|
|**accountNm**  <br>*optional*|**Example** : `"string"`|string|
|**accountNo**  <br>*optional*|**Example** : `"string"`|string|
|**bankNm**  <br>*optional*|**Example** : `"string"`|string|
|**bizDtlAddr**  <br>*optional*|**Example** : `"string"`|string|
|**bizFixAddr**  <br>*optional*|**Example** : `"string"`|string|
|**bizGb**  <br>*optional*|**Example** : `"string"`|string|
|**bizKind**  <br>*optional*|**Example** : `"string"`|string|
|**bizNo**  <br>*optional*|**Example** : `"string"`|string|
|**bizType**  <br>*optional*|**Example** : `"string"`|string|
|**bizZipNo**  <br>*optional*|**Example** : `"string"`|string|
|**chgEmail**  <br>*optional*|**Example** : `"string"`|string|
|**chgFax1**  <br>*optional*|**Example** : `"string"`|string|
|**chgFax2**  <br>*optional*|**Example** : `"string"`|string|
|**chgFax3**  <br>*optional*|**Example** : `"string"`|string|
|**chgHphone1**  <br>*optional*|**Example** : `"string"`|string|
|**chgHphone2**  <br>*optional*|**Example** : `"string"`|string|
|**chgHphone3**  <br>*optional*|**Example** : `"string"`|string|
|**chgNm**  <br>*optional*|**Example** : `"string"`|string|
|**csOperatorEmail**  <br>*optional*|**Example** : `"string"`|string|
|**csOperatorNm**  <br>*optional*|**Example** : `"string"`|string|
|**csOperatorPhone1**  <br>*optional*|**Example** : `"string"`|string|
|**csOperatorPhone2**  <br>*optional*|**Example** : `"string"`|string|
|**csOperatorPhone3**  <br>*optional*|**Example** : `"string"`|string|
|**entrStsCd**  <br>*optional*|**Example** : `"string"`|string|
|**entrStsNm**  <br>*optional*|**Example** : `"string"`|string|
|**fax1**  <br>*optional*|**Example** : `"string"`|string|
|**fax2**  <br>*optional*|**Example** : `"string"`|string|
|**fax3**  <br>*optional*|**Example** : `"string"`|string|
|**ownerNm**  <br>*optional*|**Example** : `"string"`|string|
|**phone1**  <br>*optional*|**Example** : `"string"`|string|
|**phone2**  <br>*optional*|**Example** : `"string"`|string|
|**phone3**  <br>*optional*|**Example** : `"string"`|string|
|**sacOperatorEmail**  <br>*optional*|**Example** : `"string"`|string|
|**sacOperatorNm**  <br>*optional*|**Example** : `"string"`|string|
|**sacOperatorPhone1**  <br>*optional*|**Example** : `"string"`|string|
|**sacOperatorPhone2**  <br>*optional*|**Example** : `"string"`|string|
|**sacOperatorPhone3**  <br>*optional*|**Example** : `"string"`|string|
|**sellFeeRate**  <br>*optional*|**Example** : `0`|integer (int32)|
|**settleDay**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrCd**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrNm**  <br>*optional*|**Example** : `"string"`|string|
|**upId**  <br>*optional*|**Example** : `"string"`|string|
|**upSupplyEntrCd**  <br>*optional*|**Example** : `"string"`|string|


<a name="supplycontractinfodto"></a>
### SupplyContractInfoDTO

|Name|Description|Schema|
|---|---|---|
|**agreeDt**  <br>*optional*|**Example** : `"string"`|string|
|**agreeYn**  <br>*optional*|**Example** : `"string"`|string|
|**bizDtlAddr**  <br>*optional*|**Example** : `"string"`|string|
|**bizFixAddr**  <br>*optional*|**Example** : `"string"`|string|
|**bizNo**  <br>*optional*|**Example** : `"string"`|string|
|**contractNm**  <br>*optional*|**Example** : `"string"`|string|
|**ownerNm**  <br>*optional*|**Example** : `"string"`|string|
|**regDt**  <br>*optional*|**Example** : `"string"`|string|
|**status**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrCd**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrNm**  <br>*optional*|**Example** : `"string"`|string|





