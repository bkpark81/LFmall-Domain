# LF 물류 API


<a name="overview"></a>
## Overview
LF 물류 API Docs


### Version information
*Version* : 1.0


### License information
*Terms of service* : http://www.lfmall.co.kr


### URI scheme
*Host* : dev-napi.lfmall.co.kr  
*BasePath* : /swagger/fulfilment


### Tags

* 물류 공통 : Common Controller
* 물류 출고처 : Fulfilment Origin Controller




<a name="paths"></a>
## Resources

<a name="3168ddef841b49c7a6b038413bc7de86"></a>
### 물류 공통
Common Controller


<a name="listcodeusingget"></a>
#### 코드값 조회
```
GET /fulfilment/common/v1/code/groupCd/{groupCd}
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
/fulfilment/common/v1/code/groupCd/string
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


<a name="liststbdeliveryentrusingget"></a>
#### 택배사 코드값 조회
```
GET /fulfilment/common/v1/stbDeliveryEntr
```


##### Description
설명 : 택배사 코드값 조회


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«DeliveryDTO»»](#2001792aa000eb030780d1f66d4d7be9)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/fulfilment/common/v1/stbDeliveryEntr
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : [ {
    "deliveryEntrCd" : "string",
    "deliveryEntrNm" : "string"
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


<a name="eca11196ca5ade4d31db9fd177172578"></a>
### 물류 출고처
Fulfilment Origin Controller


<a name="listdeliverylocusingget"></a>
#### 출고처 목록 조회
```
GET /fulfilment/origin/v1/deliveryLoc/supplyEntrCd/{supplyEntrCd}
```


##### Description
설명 : 출고처 목록 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**supplyEntrCd**  <br>*required*|supplyEntrCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«DeliveryLocInfoDTO»»](#9017131443ddd718d66951c1ecf14e45)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/fulfilment/origin/v1/deliveryLoc/supplyEntrCd/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : [ {
    "deliveryLocCd" : "string",
    "deliveryLocNm" : "string",
    "useYn" : "string"
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


<a name="createdeliveryreturnusingpost"></a>
#### 출고처/반품지 등록
```
POST /fulfilment/origin/v1/deliveryReturn
```


##### Description
설명 : 출고처/반품지 등록


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**deliveryReturnLocDTO**  <br>*required*|deliveryReturnLocDTO|[DeliveryReturnLocDTO](#deliveryreturnlocdto)|


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
/fulfilment/origin/v1/deliveryReturn
```


###### Request body
```json
{
  "deliveryEntrCd" : "string",
  "deliveryEntrNm" : "string",
  "deliveryLocAddrFull" : "string",
  "deliveryLocCd" : "string",
  "deliveryLocDtlAddr" : "string",
  "deliveryLocFixAddr" : "string",
  "deliveryLocNm" : "string",
  "deliveryLocPhone1" : "string",
  "deliveryLocPhone2" : "string",
  "deliveryLocPhone3" : "string",
  "deliveryLocZip1" : "string",
  "deliveryLocZip2" : "string",
  "locCd" : "string",
  "returnAddrFull" : "string",
  "returnDtlAddr" : "string",
  "returnFixAddr" : "string",
  "returnZipNo" : "string",
  "rnum" : 0,
  "supplyEntrCd" : "string",
  "supplyEntrNm" : "string",
  "totalCnt" : 0,
  "upId" : "string",
  "useYn" : "string",
  "verifiedYn" : "string"
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


<a name="updatedeliveryreturnusingpatch"></a>
#### 출고처/반품지 수정
```
PATCH /fulfilment/origin/v1/deliveryReturn
```


##### Description
설명 : 출고처/반품지 수정


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**deliveryReturnLocDTO**  <br>*required*|deliveryReturnLocDTO|[DeliveryReturnLocDTO](#deliveryreturnlocdto)|


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
/fulfilment/origin/v1/deliveryReturn
```


###### Request body
```json
{
  "deliveryEntrCd" : "string",
  "deliveryEntrNm" : "string",
  "deliveryLocAddrFull" : "string",
  "deliveryLocCd" : "string",
  "deliveryLocDtlAddr" : "string",
  "deliveryLocFixAddr" : "string",
  "deliveryLocNm" : "string",
  "deliveryLocPhone1" : "string",
  "deliveryLocPhone2" : "string",
  "deliveryLocPhone3" : "string",
  "deliveryLocZip1" : "string",
  "deliveryLocZip2" : "string",
  "locCd" : "string",
  "returnAddrFull" : "string",
  "returnDtlAddr" : "string",
  "returnFixAddr" : "string",
  "returnZipNo" : "string",
  "rnum" : 0,
  "supplyEntrCd" : "string",
  "supplyEntrNm" : "string",
  "totalCnt" : 0,
  "upId" : "string",
  "useYn" : "string",
  "verifiedYn" : "string"
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


<a name="listdeliveryreturnusingget"></a>
#### 출고처/반품지 목록 조회
```
GET /fulfilment/origin/v1/deliveryReturns/supplyEntrCd/{supplyEntrCd}
```


##### Description
설명 : 출고처/반품지 목록 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**supplyEntrCd**  <br>*required*|supplyEntrCd|string|
|**Query**|**pageNum**  <br>*required*|pageNum|string|
|**Query**|**pageSize**  <br>*required*|pageSize|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«DeliveryReturnLocDTO»»](#fb8428c0c95694cd2576aa651c94552b)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/fulfilment/origin/v1/deliveryReturns/supplyEntrCd/string?pageNum=string&pageSize=string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : [ {
    "deliveryEntrCd" : "string",
    "deliveryEntrNm" : "string",
    "deliveryLocAddrFull" : "string",
    "deliveryLocCd" : "string",
    "deliveryLocDtlAddr" : "string",
    "deliveryLocFixAddr" : "string",
    "deliveryLocNm" : "string",
    "deliveryLocPhone1" : "string",
    "deliveryLocPhone2" : "string",
    "deliveryLocPhone3" : "string",
    "deliveryLocZip1" : "string",
    "deliveryLocZip2" : "string",
    "locCd" : "string",
    "returnAddrFull" : "string",
    "returnDtlAddr" : "string",
    "returnFixAddr" : "string",
    "returnZipNo" : "string",
    "rnum" : 0,
    "supplyEntrCd" : "string",
    "supplyEntrNm" : "string",
    "totalCnt" : 0,
    "upId" : "string",
    "useYn" : "string",
    "verifiedYn" : "string"
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




<a name="definitions"></a>
## Definitions

<a name="codedto"></a>
### CodeDTO

|Name|Description|Schema|
|---|---|---|
|**attrC1**  <br>*optional*|**Example** : `"string"`|string|
|**code**  <br>*optional*|**Example** : `"string"`|string|
|**codeDesc**  <br>*optional*|**Example** : `"string"`|string|
|**codeNm**  <br>*optional*|**Example** : `"string"`|string|


<a name="deliverydto"></a>
### DeliveryDTO

|Name|Description|Schema|
|---|---|---|
|**deliveryEntrCd**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryEntrNm**  <br>*optional*|**Example** : `"string"`|string|


<a name="deliverylocinfodto"></a>
### DeliveryLocInfoDTO

|Name|Description|Schema|
|---|---|---|
|**deliveryLocCd**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocNm**  <br>*optional*|**Example** : `"string"`|string|
|**useYn**  <br>*optional*|**Example** : `"string"`|string|


<a name="deliveryreturnlocdto"></a>
### DeliveryReturnLocDTO

|Name|Description|Schema|
|---|---|---|
|**deliveryEntrCd**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryEntrNm**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocAddrFull**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocCd**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocDtlAddr**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocFixAddr**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocNm**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocPhone1**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocPhone2**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocPhone3**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocZip1**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocZip2**  <br>*optional*|**Example** : `"string"`|string|
|**locCd**  <br>*optional*|**Example** : `"string"`|string|
|**returnAddrFull**  <br>*optional*|**Example** : `"string"`|string|
|**returnDtlAddr**  <br>*optional*|**Example** : `"string"`|string|
|**returnFixAddr**  <br>*optional*|**Example** : `"string"`|string|
|**returnZipNo**  <br>*optional*|**Example** : `"string"`|string|
|**rnum**  <br>*optional*|**Example** : `0`|integer (int32)|
|**supplyEntrCd**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrNm**  <br>*optional*|**Example** : `"string"`|string|
|**totalCnt**  <br>*optional*|**Example** : `0`|integer (int32)|
|**upId**  <br>*optional*|**Example** : `"string"`|string|
|**useYn**  <br>*optional*|**Example** : `"string"`|string|
|**verifiedYn**  <br>*optional*|**Example** : `"string"`|string|


<a name="lfdcheader"></a>
### LfdcHeader

|Name|Description|Schema|
|---|---|---|
|**additionalMessage**  <br>*optional*|**Example** : `"string"`|string|
|**status**  <br>*optional*|**Example** : `"string"`|string|


<a name="791a66e885021b66ebc2a4c839933f27"></a>
### LfdcResponse«List«CodeDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[codedto](#codedto)" ]`|< [CodeDTO](#codedto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="2001792aa000eb030780d1f66d4d7be9"></a>
### LfdcResponse«List«DeliveryDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[deliverydto](#deliverydto)" ]`|< [DeliveryDTO](#deliverydto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="9017131443ddd718d66951c1ecf14e45"></a>
### LfdcResponse«List«DeliveryLocInfoDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[deliverylocinfodto](#deliverylocinfodto)" ]`|< [DeliveryLocInfoDTO](#deliverylocinfodto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="fb8428c0c95694cd2576aa651c94552b"></a>
### LfdcResponse«List«DeliveryReturnLocDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[deliveryreturnlocdto](#deliveryreturnlocdto)" ]`|< [DeliveryReturnLocDTO](#deliveryreturnlocdto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="3d8f4041e4ffd0ebb48bc9d2cf7190ed"></a>
### LfdcResponse«int»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `0`|integer (int32)|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="paginginfo"></a>
### PagingInfo

|Name|Description|Schema|
|---|---|---|
|**gridId**  <br>*optional*|**Example** : `"string"`|string|
|**pagingIndex**  <br>*optional*|**Example** : `0`|integer (int32)|
|**pagingTotalCount**  <br>*optional*|**Example** : `0`|integer (int32)|
|**pagingWindowSize**  <br>*optional*|**Example** : `0`|integer (int32)|





