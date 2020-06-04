# LF 상품 API


<a name="overview"></a>
## Overview
LF 상품 API Docs


### Version information
*Version* : 1.0


### License information
*Terms of service* : http://www.lfmall.co.kr


### URI scheme
*Host* : dev-napi.lfmall.co.kr  
*BasePath* : /swagger/product


### Tags

* 브랜드 : Product Brand Controller
* 상품 공통 : Product Common Controller
* 상품 속성 : Product Property Controller
* 상품 정보 : Product Info Controller
* 상품 정보 고시 : Product Information Notice Controller
* 상품 카테고리 : Product Category Controller




<a name="paths"></a>
## Resources

<a name="f0863f556714bb1f9754e61d00c9526a"></a>
### 브랜드
Product Brand Controller


<a name="brandbasefeeusingget"></a>
#### 브랜드 기본 가격 조회
```
GET /product/brand/v1/brand/baseFee/brandCd/{brandCd}
```


##### Description
설명 : 브랜드 기본 가격 조회(기본 배송비, 무료배송비최소구매금액, 판매수수료율)


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**brandCd**  <br>*required*|brandCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«BrandBaseFeeInfoDTO»](#de1205c441370f002551b3f96853eff5)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/product/brand/v1/brand/baseFee/brandCd/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : {
    "deliveryFee" : "string",
    "minOrdAmt" : "string",
    "sellFeeRate" : "string"
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


<a name="listpartnerbrandusingget"></a>
#### 입점사 브랜드 리스트 조회
```
GET /product/brand/v1/brand/list/partner/supplyEntr/{supplyEntrCd}
```


##### Description
설명 : 입점사 브랜드 리스트 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**supplyEntrCd**  <br>*required*|supplyEntrCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«BrandInfoDTO»»](#5ccb0c78d2f3393a9071bd2e6f852f8f)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/product/brand/v1/brand/list/partner/supplyEntr/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : [ {
    "brandCd" : "string",
    "brandGroupNm" : "string"
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


<a name="brandmdusingget"></a>
#### 브랜드 MD 조회
```
GET /product/brand/v1/brand/md/brandCd/{brandCd}
```


##### Description
설명 : 브랜드 MD 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**brandCd**  <br>*required*|brandCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«BrandManagerInfoDTO»](#c350bfb96d708367925b686630bd0dde)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/product/brand/v1/brand/md/brandCd/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : {
    "mgrId" : "string",
    "mgrNm" : "string"
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


<a name="detailbrandcntusingget"></a>
#### 신규 브랜드 등록 > 브랜드 중복 체크
```
GET /product/brand/v1/brandCnt/supplyEntrCd/{supplyEntrCd}/brandNm/{brandNm}/brandEnm/{brandEnm}
```


##### Description
설명 : 신규 브랜드 등록 > 브랜드 중복 체크


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**brandEnm**  <br>*required*|brandEnm|string|
|**Path**|**brandNm**  <br>*required*|brandNm|string|
|**Path**|**supplyEntrCd**  <br>*required*|supplyEntrCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«int»](#3d8f4041e4ffd0ebb48bc9d2cf7190ed)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/product/brand/v1/brandCnt/supplyEntrCd/string/brandNm/string/brandEnm/string
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


<a name="listsupplybrandinfousingget"></a>
#### 계정정보 상세 > 브랜드 목록 조회
```
GET /product/brand/v1/brandInfos/supplyEntrCd/{supplyEntrCd}
```


##### Description
설명 : 계정정보 상세 > 브랜드 목록 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**supplyEntrCd**  <br>*required*|supplyEntrCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«SupplyBrandInfoDTO»»](#5d5ad40a0f74ec07720782c0d5bbb404)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/product/brand/v1/brandInfos/supplyEntrCd/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : [ {
    "brandCd" : "string",
    "brandEnm" : "string",
    "brandNm" : "string",
    "confirmYn" : "string",
    "deliveryFee" : 0,
    "deliveryLocCd" : "string",
    "deliveryLocNm" : "string",
    "mgrId" : "string",
    "minOrdAmt" : 0,
    "num" : 0,
    "supplyEntrCd" : "string",
    "tbrandEnm" : "string",
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


<a name="createbrandusingpost"></a>
#### 신규 브랜드 등록 > 등록
```
POST /product/brand/v1/createBrand
```


##### Description
설명 : 신규 브랜드 등록 > 등록


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Body**|**stbBrand**  <br>*required*|stbBrand|[BrandInfo](#brandinfo)|


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
/product/brand/v1/createBrand
```


###### Request body
```json
{
  "brandCd" : "string",
  "brandEnm" : "string",
  "brandGroupNm" : "string",
  "brandNm" : "string",
  "confirmYn" : "string",
  "deliveryFee" : "string",
  "deliveryLocCd" : "string",
  "deliveryLocNm" : "string",
  "mgrId" : "string",
  "minOrdAmt" : "string",
  "num" : 0,
  "sellFeeRate" : "string",
  "supplyEntrCd" : "string",
  "tbrandEnm" : "string",
  "useYn" : "string"
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


<a name="b2388ab4e0052ca16af3f5ea13c24799"></a>
### 상품 공통
Product Common Controller


<a name="listcodeusingget"></a>
#### 공통 코드 조회
```
GET /product/common/v1/code/groupCd/{groupCd}
```


##### Description
설명 : 공통 코드 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**groupCd**  <br>*required*|groupCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«CodeInfoDTO»»](#c6fda04002c495b8323eedcd1381cf9b)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/product/common/v1/code/groupCd/string
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


<a name="listsymbolusingget"></a>
#### 특수 문자 조회
```
GET /product/common/v1/symbol/groupCd/{groupCd}
```


##### Description
설명 : 특수 문자 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**groupCd**  <br>*required*|groupCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|< [SymbolInfoDTO](#symbolinfodto) > array|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/product/common/v1/symbol/groupCd/string
```


##### Example HTTP response

###### Response 200
```json
[ {
  "code" : "string"
} ]
```


<a name="dd2b0cafcf586af3da0098f375b037ad"></a>
### 상품 속성
Product Property Controller


<a name="listpropertyusingget"></a>
#### 상품 속성 조회
```
GET /product/property/v1/properties/standardCategoryId/{standardCategoryId}
```


##### Description
설명 : 상품 속성 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**standardCategoryId**  <br>*required*|standardCategoryId|string|
|**Query**|**prodCd**  <br>*optional*|prodCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«ProductPropertyInfoDTO»»](#0439f24885f9a4e3d525cc45e125973b)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/product/property/v1/properties/standardCategoryId/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : [ {
    "checkId1" : "string",
    "checkId2" : "string",
    "checkId3" : "string",
    "checkId4" : "string",
    "checkId5" : "string",
    "id1" : "string",
    "id2" : "string",
    "id3" : "string",
    "id4" : "string",
    "id5" : "string",
    "propertyId" : "string",
    "propertyName" : "string",
    "rowNo" : "string",
    "rowSpan" : "string",
    "value1" : "string",
    "value2" : "string",
    "value3" : "string",
    "value4" : "string",
    "value5" : "string"
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


<a name="listpropertyvalueusingget"></a>
#### 상품 속성값 조회
```
GET /product/property/v1/property/value/prodCd/{prodCd}
```


##### Description
설명 : 상품 속성값 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**prodCd**  <br>*required*|prodCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«ProductPropertyValueDTO»»](#3ef2bb388096b92aa7f8a67af498540f)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/product/property/v1/property/value/prodCd/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : [ {
    "prodCd" : "string",
    "propertyValueId" : "string"
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


<a name="6d6be93d0d527b0ecc4241ea9a1a3e31"></a>
### 상품 정보
Product Info Controller


<a name="listpartnercopyproductsusingget"></a>
#### 입점 > 상품 복사하기 상품 리스트 조회
```
GET /product/productinfo/v1/copy/products/regId/{regId}
```


##### Description
설명 : 입점 > 상품 복사하기 상품 리스트 조회


##### Parameters

|Type|Name|Description|Schema|Default|
|---|---|---|---|---|
|**Path**|**regId**  <br>*required*|등록자ID|string|`"kjkim01"`|
|**Query**|**prodCd**  <br>*optional*|prodCd|string||
|**Query**|**prodNm**  <br>*optional*|상품명|string|`"셔츠"`|
|**Query**|**supplyProdCd**  <br>*optional*|supplyProdCd|string||


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«PartnerProductCopyDTO»»](#1cadd0ab8a3dd5aac99577669e77e54f)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/product/productinfo/v1/copy/products/regId/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : [ {
    "adminMemo" : "string",
    "brandCd" : "string",
    "changeAbleyn" : "string",
    "changeFeeFreeYn" : "string",
    "codYn" : "string",
    "colorYn" : "string",
    "confirmDt" : "string",
    "confirmField" : "string",
    "confirmImgPath" : "string",
    "confirmInstitute" : "string",
    "confirmNo" : "string",
    "confirmValidEndDt" : "string",
    "confirmValidStartDt" : "string",
    "dcRate" : "string",
    "deliveryDt" : "string",
    "deliveryFee" : "string",
    "deliveryLocCd" : "string",
    "deliveryMethod" : "string",
    "gratitudeDesc" : "string",
    "importNo" : "string",
    "importationGb" : "string",
    "importerNm" : "string",
    "issueDt" : "string",
    "itemkindCd" : "string",
    "kcGb" : "string",
    "listPrice" : "string",
    "mainImgUrl" : "string",
    "makeDt" : "string",
    "makeNm" : "string",
    "makeYear" : "string",
    "materialDesc" : "string",
    "maxOrdQty" : "string",
    "minOrdAmt" : "string",
    "minOrdQty" : "string",
    "minorBuyYn" : "string",
    "modelCd" : "string",
    "modelNm" : "string",
    "nativeCd" : "string",
    "nativeDetail" : "string",
    "optionSetYn" : "string",
    "orderMakingRd" : "string",
    "overseasAddr" : "string",
    "overseasAgency" : "string",
    "overseasBizno" : "string",
    "overseasSeller" : "string",
    "prodCd" : "string",
    "prodNm" : "string",
    "prodNmEng" : "string",
    "prodPrice" : "string",
    "prodSexGb" : "string",
    "prodSpecCd" : "string",
    "prodStockQty" : "string",
    "prodStsCd" : "string",
    "prodStsNm" : "string",
    "prodWeight" : "string",
    "productOriginPrice" : "string",
    "regDt" : "string",
    "returnAbleyn" : "string",
    "returnFeeFreeYn" : "string",
    "safeConfirmYn" : "string",
    "seasonCd" : "string",
    "sellFeeRate" : "string",
    "separateSettingCost" : "string",
    "simpleProductExplain" : "string",
    "spointRate" : "string",
    "standardcategoryid" : "string",
    "styleYy" : "string",
    "supplyProdCd" : "string",
    "supplyProdNm" : "string",
    "validDays" : "string",
    "validDt" : "string",
    "vatCd" : "string"
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


<a name="listpartnerproductstatuscountusingget"></a>
#### 입점 > 상품 상태별 등록 현황
```
GET /product/productinfo/v1/product-status/count/supplyEntr/{supplyEntrCd}
```


##### Description
설명 : 입점 > 상품 상태별 등록 현황


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**supplyEntrCd**  <br>*required*|supplyEntrCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«PartnerProductStatusCountDTO»»](#89ce2647fb9a768fe714edea38254b70)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/product/productinfo/v1/product-status/count/supplyEntr/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : [ {
    "cntByProdStsCd" : "string",
    "prodStsCd" : "string",
    "totalCnt" : "string"
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


<a name="listpartnerproductsusingget"></a>
#### 입점 > 상품 상태별 상품 리스트 조회
```
GET /product/productinfo/v1/product-status/products/supplyEntr/{supplyEntrCd}/{prodStsCd}
```


##### Description
설명 : 입점 > 상품 상태별 상품 리스트 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**prodStsCd**  <br>*required*|prodStsCd|string|
|**Path**|**supplyEntrCd**  <br>*required*|supplyEntrCd|string|
|**Query**|**pageNum**  <br>*required*|pageNum|string|
|**Query**|**pageSize**  <br>*required*|pageSize|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«PartnerProductListDTO»»](#e5b5114c0eba078919e0f03080f8f1a4)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/product/productinfo/v1/product-status/products/supplyEntr/string/string?pageNum=string&pageSize=string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : [ {
    "adminMemo" : "string",
    "brandCd" : "string",
    "brandNm" : "string",
    "categoryNm" : "string",
    "codYn" : "string",
    "dcRate" : "string",
    "deliveryFee" : "string",
    "deliveryLocNm" : "string",
    "gratitudeDesc" : "string",
    "itemYy" : "string",
    "listPrice" : "string",
    "mdId" : "string",
    "mdNm" : "string",
    "monthSellQty" : "string",
    "optionQty" : "string",
    "optionSetYn" : "string",
    "overseasAddr" : "string",
    "overseasAgency" : "string",
    "overseasBizno" : "string",
    "overseasSeller" : "string",
    "prodCd" : "string",
    "prodImgUrl" : "string",
    "prodNm" : "string",
    "prodPrice" : "string",
    "prodStsCd" : "string",
    "prodStsNm" : "string",
    "regDt" : "string",
    "returnNm" : "string",
    "reviewCnt" : "string",
    "rnum" : "string",
    "sellFeeRate" : "string",
    "separateSettingCost" : "string",
    "spointRate" : "string",
    "standardcategoryid" : "string",
    "stockQty" : "string",
    "supplyProdCd" : "string",
    "totalCnt" : "string",
    "totalSellQty" : "string",
    "upDt" : "string",
    "weekSellQty" : "string"
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


<a name="productdetailusingget"></a>
#### 입점 > 상품 상세 정보 조회
```
GET /product/productinfo/v1/product/detail/prodCd/{prodCd}
```


##### Description
설명 : 입점 > 상품 상세 정보 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**prodCd**  <br>*required*|prodCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«ProductDetailDTO»](#d6f43ac7fdce058952f37f7199581f77)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/product/productinfo/v1/product/detail/prodCd/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : {
    "adminMemo" : "string",
    "brandCd" : "string",
    "changeAbleyn" : "string",
    "changeFeeFreeYn" : "string",
    "codYn" : "string",
    "colorCd" : "string",
    "colorYn" : "string",
    "confirmDt" : "string",
    "confirmField" : "string",
    "confirmImgPath" : "string",
    "confirmInstitute" : "string",
    "confirmNo" : "string",
    "confirmValidEndDt" : "string",
    "confirmValidStartDt" : "string",
    "dcRate" : "string",
    "deliveryDt" : "string",
    "deliveryFee" : "string",
    "deliveryLocCd" : "string",
    "deliveryMethod" : "string",
    "exceptEntrYn" : "string",
    "gratitudeDesc" : "string",
    "importNo" : "string",
    "importationGb" : "string",
    "importerNm" : "string",
    "issueDt" : "string",
    "itemYy" : "string",
    "itemkindCd" : "string",
    "kcGb" : "string",
    "listPrice" : "string",
    "mainImgUrl" : "string",
    "makeDt" : "string",
    "makeNm" : "string",
    "makeYear" : "string",
    "materialDesc" : "string",
    "maxOrdQty" : "string",
    "mdId" : "string",
    "mdNm" : "string",
    "minOrdAmt" : "string",
    "minOrdQty" : "string",
    "minorBuyYn" : "string",
    "modelCd" : "string",
    "modelNm" : "string",
    "nativeCd" : "string",
    "nativeDetail" : "string",
    "notiList" : [ {
      "niCd" : "string",
      "niCdNm" : "string",
      "niCdNm2" : "string",
      "niTypeCd" : "string",
      "niTypeCdNm" : "string",
      "niValue" : "string",
      "niValue2" : "string",
      "niValueGb" : "string",
      "prodCd" : "string"
    } ],
    "optionList" : [ {
      "enterpriseOptionCd" : "string",
      "extraCharge" : "string",
      "optionNm1" : "string",
      "optionNm2" : "string",
      "optionValue1" : "string",
      "optionValue2" : "string",
      "priority" : "string",
      "prodOptionCd" : "string",
      "saleAbleYn" : "string",
      "stockQty" : "string",
      "useYn" : "string"
    } ],
    "optionSetYn" : "string",
    "orderMakingRd" : "string",
    "overseasAddr" : "string",
    "overseasAgency" : "string",
    "overseasBizno" : "string",
    "overseasSeller" : "string",
    "priceResYn" : "string",
    "prodCd" : "string",
    "prodDesc" : "string",
    "prodNm" : "string",
    "prodNmEng" : "string",
    "prodPrice" : "string",
    "prodSexGb" : "string",
    "prodSpecCd" : "string",
    "prodStockQty" : "string",
    "prodStsCd" : "string",
    "prodStsNm" : "string",
    "prodWeight" : "string",
    "productOriginPrice" : "string",
    "regDt" : "string",
    "returnAbleyn" : "string",
    "returnFeeFreeYn" : "string",
    "safeConfirmYn" : "string",
    "seasonCd" : "string",
    "sellFeeRate" : "string",
    "sellfeerateResYn" : "string",
    "separateSettingCost" : "string",
    "simpleProductExplain" : "string",
    "soldoutDisplayYn" : "string",
    "soldoutDisplayoptYn" : "string",
    "spointRate" : "string",
    "standardcategory1deptCd" : "string",
    "standardcategory2deptCd" : "string",
    "standardcategory3deptCd" : "string",
    "standardcategoryid" : "string",
    "styleYy" : "string",
    "supplyEntrCd" : "string",
    "supplyProdCd" : "string",
    "supplyProdNm" : "string",
    "validDays" : "string",
    "validDt" : "string",
    "vatCd" : "string"
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


<a name="saveproductusingpost"></a>
#### 입점 > 상품 개별 등록
```
POST /product/productinfo/v1/save/product
```


##### Description
설명 : 입점 > 상품 개별 등록


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**FormData**|**imageFile**  <br>*optional*|imageFile|< file > array(multi)|
|**Body**|**productInfoDTO**  <br>*required*|productInfoDTO|[ProductInfoDTO](#productinfodto)|


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
/product/productinfo/v1/save/product
```


###### Request formData
```json
"file"
```


###### Request body
```json
{
  "adminMemo" : "string",
  "brandCd" : "string",
  "changeAbleyn" : "string",
  "changeFeeFreeYn" : "string",
  "codYn" : "string",
  "colorCd" : "string",
  "colorYn" : "string",
  "confirmNo" : "string",
  "dcRate" : "string",
  "deliveryDt" : "string",
  "deliveryFee" : "string",
  "deliveryLocCd" : "string",
  "deliveryMethod" : "string",
  "importationGb" : "string",
  "itemYy" : "string",
  "itemkindCd" : "string",
  "kcGb" : "string",
  "listPrice" : "string",
  "makeNm" : "string",
  "maxOrdQty" : "string",
  "mdId" : "string",
  "minOrdAmt" : "string",
  "minOrdQty" : "string",
  "minorBuyYn" : "string",
  "modelCd" : "string",
  "modelNm" : "string",
  "nativeCd" : "string",
  "niCd0" : "string",
  "niCd1" : "string",
  "niCd10" : "string",
  "niCd11" : "string",
  "niCd12" : "string",
  "niCd13" : "string",
  "niCd14" : "string",
  "niCd2" : "string",
  "niCd3" : "string",
  "niCd4" : "string",
  "niCd5" : "string",
  "niCd6" : "string",
  "niCd7" : "string",
  "niCd8" : "string",
  "niCd9" : "string",
  "niTypeCd" : "string",
  "optionSetYn" : "string",
  "orderMakingRd" : "string",
  "overseasAddr" : "string",
  "overseasAgency" : "string",
  "overseasBizno" : "string",
  "overseasSeller" : "string",
  "prodCd" : "string",
  "prodDesc" : "string",
  "prodNm" : "string",
  "prodPrice" : "string",
  "prodSexGb" : "string",
  "prodSpecCd" : "string",
  "prodStockQty" : "string",
  "prodStsCd" : "string",
  "productOptionInfo" : {
    "optionList" : [ {
      "enterpriseOptionCd" : "string",
      "extraCharge" : "string",
      "optionNm1" : "string",
      "optionNm2" : "string",
      "optionValue1" : "string",
      "optionValue2" : "string",
      "priority" : "string",
      "prodOptionCd" : "string",
      "saleAbleYn" : "string",
      "stockQty" : "string",
      "useYn" : "string"
    } ],
    "optionSetYn" : "string",
    "prodStockQty" : "string"
  },
  "productOriginPrice" : "string",
  "propertyList" : [ "string" ],
  "regId" : "string",
  "returnAbleyn" : "string",
  "returnFeeFreeYn" : "string",
  "seasonCd" : "string",
  "sellFeeRate" : "string",
  "separateSettingCost" : "string",
  "soldoutDisplayYn" : "string",
  "soldoutDisplayoptYn" : "string",
  "spointRate" : "string",
  "standardcategoryid" : "string",
  "supplyEntrCd" : "string",
  "supplyProdCd" : "string",
  "vatCd" : "string"
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


<a name="1e7e9c49e7ad4db6e78fa728776243b8"></a>
### 상품 정보 고시
Product Information Notice Controller


<a name="listnoticeusingget"></a>
#### 상품 고시정보 조회
```
GET /product/information/notice/v1/informationnotices/niTypeCd/{niTypeCd}
```


##### Description
설명 : 상품 고시정보 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**niTypeCd**  <br>*required*|niTypeCd|string|
|**Query**|**prodCd**  <br>*optional*|prodCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«ProductInformationNoticeInfoDTO»»](#a733eb32db21e3f169b25afc1a73e1b3)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/product/information/notice/v1/informationnotices/niTypeCd/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : [ {
    "niCd" : "string",
    "niCdNm" : "string",
    "niCdNm2" : "string",
    "niTypeCd" : "string",
    "niTypeCdNm" : "string",
    "niValue" : "string",
    "niValue2" : "string",
    "niValueGb" : "string",
    "prodCd" : "string"
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


<a name="2fc8e3c2d64c6cd6a0875783ee6fc6e1"></a>
### 상품 카테고리
Product Category Controller


<a name="listitemkindbrandusingget"></a>
#### 상품분류 목록 조회 (브랜드코드로 찾는 경우 포함)
```
GET /product/category/v1/itemkind/list/brand
```


##### Description
설명 : 상품분류 목록 조회 (브랜드코드로 찾는 경우 포함)


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Query**|**brandCd**  <br>*optional*|brandCd|string|
|**Query**|**itemkindCd**  <br>*optional*|itemkindCd|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«ItemKindWithBrandDTO»»](#69f8c88fb054de9c7e1c0470559200c6)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/product/category/v1/itemkind/list/brand
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : [ {
    "code" : "string",
    "deliveryLocCd" : "string",
    "itemkindCd" : "string",
    "itemkindNm" : "string"
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


<a name="listcategoryusingget"></a>
#### 물리 카테고리 정보 조회
```
GET /product/category/v1/standardcategory/list/{depth}
```


##### Description
설명 : 물리 카테고리 정보 조회


##### Parameters

|Type|Name|Description|Schema|
|---|---|---|---|
|**Path**|**depth**  <br>*required*|depth|string|
|**Query**|**parentId**  <br>*optional*|parentId|string|


##### Responses

|HTTP Code|Description|Schema|
|---|---|---|
|**200**|OK|[LfdcResponse«List«StandardCategoryInfoDTO»»](#b3b220f1c2ea56c578aaf79ff65af21f)|


##### Produces

* `\*/*`


##### Example HTTP request

###### Request path
```
/product/category/v1/standardcategory/list/string
```


##### Example HTTP response

###### Response 200
```json
{
  "body" : [ {
    "code" : "string",
    "codeNm" : "string",
    "createymdt" : "string",
    "creatorid" : "string",
    "depth" : "string",
    "modifierid" : "string",
    "modifyymdt" : "string",
    "parentId" : "string",
    "usable" : "string"
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

<a name="brandbasefeeinfodto"></a>
### BrandBaseFeeInfoDTO

|Name|Description|Schema|
|---|---|---|
|**deliveryFee**  <br>*optional*|**Example** : `"string"`|string|
|**minOrdAmt**  <br>*optional*|**Example** : `"string"`|string|
|**sellFeeRate**  <br>*optional*|**Example** : `"string"`|string|


<a name="brandinfo"></a>
### BrandInfo

|Name|Description|Schema|
|---|---|---|
|**brandCd**  <br>*optional*|**Example** : `"string"`|string|
|**brandEnm**  <br>*optional*|**Example** : `"string"`|string|
|**brandGroupNm**  <br>*optional*|**Example** : `"string"`|string|
|**brandNm**  <br>*optional*|**Example** : `"string"`|string|
|**confirmYn**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryFee**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocCd**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocNm**  <br>*optional*|**Example** : `"string"`|string|
|**mgrId**  <br>*optional*|**Example** : `"string"`|string|
|**minOrdAmt**  <br>*optional*|**Example** : `"string"`|string|
|**num**  <br>*optional*|**Example** : `0`|integer (int32)|
|**sellFeeRate**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrCd**  <br>*optional*|**Example** : `"string"`|string|
|**tbrandEnm**  <br>*optional*|**Example** : `"string"`|string|
|**useYn**  <br>*optional*|**Example** : `"string"`|string|


<a name="brandinfodto"></a>
### BrandInfoDTO

|Name|Description|Schema|
|---|---|---|
|**brandCd**  <br>*optional*|**Example** : `"string"`|string|
|**brandGroupNm**  <br>*optional*|**Example** : `"string"`|string|


<a name="brandmanagerinfodto"></a>
### BrandManagerInfoDTO

|Name|Description|Schema|
|---|---|---|
|**mgrId**  <br>*optional*|**Example** : `"string"`|string|
|**mgrNm**  <br>*optional*|**Example** : `"string"`|string|


<a name="codeinfodto"></a>
### CodeInfoDTO

|Name|Description|Schema|
|---|---|---|
|**attrC1**  <br>*optional*|**Example** : `"string"`|string|
|**code**  <br>*optional*|**Example** : `"string"`|string|
|**codeDesc**  <br>*optional*|**Example** : `"string"`|string|
|**codeNm**  <br>*optional*|**Example** : `"string"`|string|


<a name="itemkindwithbranddto"></a>
### ItemKindWithBrandDTO

|Name|Description|Schema|
|---|---|---|
|**code**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocCd**  <br>*optional*|**Example** : `"string"`|string|
|**itemkindCd**  <br>*optional*|**Example** : `"string"`|string|
|**itemkindNm**  <br>*optional*|**Example** : `"string"`|string|


<a name="lfdcheader"></a>
### LfdcHeader

|Name|Description|Schema|
|---|---|---|
|**additionalMessage**  <br>*optional*|**Example** : `"string"`|string|
|**status**  <br>*optional*|**Example** : `"string"`|string|


<a name="de1205c441370f002551b3f96853eff5"></a>
### LfdcResponse«BrandBaseFeeInfoDTO»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `"[brandbasefeeinfodto](#brandbasefeeinfodto)"`|[BrandBaseFeeInfoDTO](#brandbasefeeinfodto)|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="c350bfb96d708367925b686630bd0dde"></a>
### LfdcResponse«BrandManagerInfoDTO»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `"[brandmanagerinfodto](#brandmanagerinfodto)"`|[BrandManagerInfoDTO](#brandmanagerinfodto)|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="5ccb0c78d2f3393a9071bd2e6f852f8f"></a>
### LfdcResponse«List«BrandInfoDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[brandinfodto](#brandinfodto)" ]`|< [BrandInfoDTO](#brandinfodto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="c6fda04002c495b8323eedcd1381cf9b"></a>
### LfdcResponse«List«CodeInfoDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[codeinfodto](#codeinfodto)" ]`|< [CodeInfoDTO](#codeinfodto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="69f8c88fb054de9c7e1c0470559200c6"></a>
### LfdcResponse«List«ItemKindWithBrandDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[itemkindwithbranddto](#itemkindwithbranddto)" ]`|< [ItemKindWithBrandDTO](#itemkindwithbranddto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="1cadd0ab8a3dd5aac99577669e77e54f"></a>
### LfdcResponse«List«PartnerProductCopyDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[partnerproductcopydto](#partnerproductcopydto)" ]`|< [PartnerProductCopyDTO](#partnerproductcopydto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="e5b5114c0eba078919e0f03080f8f1a4"></a>
### LfdcResponse«List«PartnerProductListDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[partnerproductlistdto](#partnerproductlistdto)" ]`|< [PartnerProductListDTO](#partnerproductlistdto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="89ce2647fb9a768fe714edea38254b70"></a>
### LfdcResponse«List«PartnerProductStatusCountDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[partnerproductstatuscountdto](#partnerproductstatuscountdto)" ]`|< [PartnerProductStatusCountDTO](#partnerproductstatuscountdto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="a733eb32db21e3f169b25afc1a73e1b3"></a>
### LfdcResponse«List«ProductInformationNoticeInfoDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[productinformationnoticeinfodto](#productinformationnoticeinfodto)" ]`|< [ProductInformationNoticeInfoDTO](#productinformationnoticeinfodto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="0439f24885f9a4e3d525cc45e125973b"></a>
### LfdcResponse«List«ProductPropertyInfoDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[productpropertyinfodto](#productpropertyinfodto)" ]`|< [ProductPropertyInfoDTO](#productpropertyinfodto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="3ef2bb388096b92aa7f8a67af498540f"></a>
### LfdcResponse«List«ProductPropertyValueDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[productpropertyvaluedto](#productpropertyvaluedto)" ]`|< [ProductPropertyValueDTO](#productpropertyvaluedto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="b3b220f1c2ea56c578aaf79ff65af21f"></a>
### LfdcResponse«List«StandardCategoryInfoDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[standardcategoryinfodto](#standardcategoryinfodto)" ]`|< [StandardCategoryInfoDTO](#standardcategoryinfodto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="5d5ad40a0f74ec07720782c0d5bbb404"></a>
### LfdcResponse«List«SupplyBrandInfoDTO»»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `[ "[supplybrandinfodto](#supplybrandinfodto)" ]`|< [SupplyBrandInfoDTO](#supplybrandinfodto) > array|
|**header**  <br>*optional*|**Example** : `"[lfdcheader](#lfdcheader)"`|[LfdcHeader](#lfdcheader)|
|**paging**  <br>*optional*|**Example** : `"[paginginfo](#paginginfo)"`|[PagingInfo](#paginginfo)|


<a name="d6f43ac7fdce058952f37f7199581f77"></a>
### LfdcResponse«ProductDetailDTO»

|Name|Description|Schema|
|---|---|---|
|**body**  <br>*optional*|**Example** : `"[productdetaildto](#productdetaildto)"`|[ProductDetailDTO](#productdetaildto)|
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


<a name="paginginfo"></a>
### PagingInfo

|Name|Description|Schema|
|---|---|---|
|**gridId**  <br>*optional*|**Example** : `"string"`|string|
|**pagingIndex**  <br>*optional*|**Example** : `0`|integer (int32)|
|**pagingTotalCount**  <br>*optional*|**Example** : `0`|integer (int32)|
|**pagingWindowSize**  <br>*optional*|**Example** : `0`|integer (int32)|


<a name="partnerproductcopydto"></a>
### PartnerProductCopyDTO

|Name|Description|Schema|
|---|---|---|
|**adminMemo**  <br>*optional*|**Example** : `"string"`|string|
|**brandCd**  <br>*optional*|**Example** : `"string"`|string|
|**changeAbleyn**  <br>*optional*|**Example** : `"string"`|string|
|**changeFeeFreeYn**  <br>*optional*|**Example** : `"string"`|string|
|**codYn**  <br>*optional*|**Example** : `"string"`|string|
|**colorYn**  <br>*optional*|**Example** : `"string"`|string|
|**confirmDt**  <br>*optional*|**Example** : `"string"`|string|
|**confirmField**  <br>*optional*|**Example** : `"string"`|string|
|**confirmImgPath**  <br>*optional*|**Example** : `"string"`|string|
|**confirmInstitute**  <br>*optional*|**Example** : `"string"`|string|
|**confirmNo**  <br>*optional*|**Example** : `"string"`|string|
|**confirmValidEndDt**  <br>*optional*|**Example** : `"string"`|string|
|**confirmValidStartDt**  <br>*optional*|**Example** : `"string"`|string|
|**dcRate**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryDt**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryFee**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocCd**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryMethod**  <br>*optional*|**Example** : `"string"`|string|
|**gratitudeDesc**  <br>*optional*|**Example** : `"string"`|string|
|**importNo**  <br>*optional*|**Example** : `"string"`|string|
|**importationGb**  <br>*optional*|**Example** : `"string"`|string|
|**importerNm**  <br>*optional*|**Example** : `"string"`|string|
|**issueDt**  <br>*optional*|**Example** : `"string"`|string|
|**itemkindCd**  <br>*optional*|**Example** : `"string"`|string|
|**kcGb**  <br>*optional*|**Example** : `"string"`|string|
|**listPrice**  <br>*optional*|**Example** : `"string"`|string|
|**mainImgUrl**  <br>*optional*|**Example** : `"string"`|string|
|**makeDt**  <br>*optional*|**Example** : `"string"`|string|
|**makeNm**  <br>*optional*|**Example** : `"string"`|string|
|**makeYear**  <br>*optional*|**Example** : `"string"`|string|
|**materialDesc**  <br>*optional*|**Example** : `"string"`|string|
|**maxOrdQty**  <br>*optional*|**Example** : `"string"`|string|
|**minOrdAmt**  <br>*optional*|**Example** : `"string"`|string|
|**minOrdQty**  <br>*optional*|**Example** : `"string"`|string|
|**minorBuyYn**  <br>*optional*|**Example** : `"string"`|string|
|**modelCd**  <br>*optional*|**Example** : `"string"`|string|
|**modelNm**  <br>*optional*|**Example** : `"string"`|string|
|**nativeCd**  <br>*optional*|**Example** : `"string"`|string|
|**nativeDetail**  <br>*optional*|**Example** : `"string"`|string|
|**optionSetYn**  <br>*optional*|**Example** : `"string"`|string|
|**orderMakingRd**  <br>*optional*|**Example** : `"string"`|string|
|**overseasAddr**  <br>*optional*|**Example** : `"string"`|string|
|**overseasAgency**  <br>*optional*|**Example** : `"string"`|string|
|**overseasBizno**  <br>*optional*|**Example** : `"string"`|string|
|**overseasSeller**  <br>*optional*|**Example** : `"string"`|string|
|**prodCd**  <br>*optional*|**Example** : `"string"`|string|
|**prodNm**  <br>*optional*|**Example** : `"string"`|string|
|**prodNmEng**  <br>*optional*|**Example** : `"string"`|string|
|**prodPrice**  <br>*optional*|**Example** : `"string"`|string|
|**prodSexGb**  <br>*optional*|**Example** : `"string"`|string|
|**prodSpecCd**  <br>*optional*|**Example** : `"string"`|string|
|**prodStockQty**  <br>*optional*|**Example** : `"string"`|string|
|**prodStsCd**  <br>*optional*|**Example** : `"string"`|string|
|**prodStsNm**  <br>*optional*|**Example** : `"string"`|string|
|**prodWeight**  <br>*optional*|**Example** : `"string"`|string|
|**productOriginPrice**  <br>*optional*|**Example** : `"string"`|string|
|**regDt**  <br>*optional*|**Example** : `"string"`|string|
|**returnAbleyn**  <br>*optional*|**Example** : `"string"`|string|
|**returnFeeFreeYn**  <br>*optional*|**Example** : `"string"`|string|
|**safeConfirmYn**  <br>*optional*|**Example** : `"string"`|string|
|**seasonCd**  <br>*optional*|**Example** : `"string"`|string|
|**sellFeeRate**  <br>*optional*|**Example** : `"string"`|string|
|**separateSettingCost**  <br>*optional*|**Example** : `"string"`|string|
|**simpleProductExplain**  <br>*optional*|**Example** : `"string"`|string|
|**spointRate**  <br>*optional*|**Example** : `"string"`|string|
|**standardcategoryid**  <br>*optional*|**Example** : `"string"`|string|
|**styleYy**  <br>*optional*|**Example** : `"string"`|string|
|**supplyProdCd**  <br>*optional*|**Example** : `"string"`|string|
|**supplyProdNm**  <br>*optional*|**Example** : `"string"`|string|
|**validDays**  <br>*optional*|**Example** : `"string"`|string|
|**validDt**  <br>*optional*|**Example** : `"string"`|string|
|**vatCd**  <br>*optional*|**Example** : `"string"`|string|


<a name="partnerproductlistdto"></a>
### PartnerProductListDTO

|Name|Description|Schema|
|---|---|---|
|**adminMemo**  <br>*optional*|**Example** : `"string"`|string|
|**brandCd**  <br>*optional*|**Example** : `"string"`|string|
|**brandNm**  <br>*optional*|**Example** : `"string"`|string|
|**categoryNm**  <br>*optional*|**Example** : `"string"`|string|
|**codYn**  <br>*optional*|**Example** : `"string"`|string|
|**dcRate**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryFee**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocNm**  <br>*optional*|**Example** : `"string"`|string|
|**gratitudeDesc**  <br>*optional*|**Example** : `"string"`|string|
|**itemYy**  <br>*optional*|**Example** : `"string"`|string|
|**listPrice**  <br>*optional*|**Example** : `"string"`|string|
|**mdId**  <br>*optional*|**Example** : `"string"`|string|
|**mdNm**  <br>*optional*|**Example** : `"string"`|string|
|**monthSellQty**  <br>*optional*|**Example** : `"string"`|string|
|**optionQty**  <br>*optional*|**Example** : `"string"`|string|
|**optionSetYn**  <br>*optional*|**Example** : `"string"`|string|
|**overseasAddr**  <br>*optional*|**Example** : `"string"`|string|
|**overseasAgency**  <br>*optional*|**Example** : `"string"`|string|
|**overseasBizno**  <br>*optional*|**Example** : `"string"`|string|
|**overseasSeller**  <br>*optional*|**Example** : `"string"`|string|
|**prodCd**  <br>*optional*|**Example** : `"string"`|string|
|**prodImgUrl**  <br>*optional*|**Example** : `"string"`|string|
|**prodNm**  <br>*optional*|**Example** : `"string"`|string|
|**prodPrice**  <br>*optional*|**Example** : `"string"`|string|
|**prodStsCd**  <br>*optional*|**Example** : `"string"`|string|
|**prodStsNm**  <br>*optional*|**Example** : `"string"`|string|
|**regDt**  <br>*optional*|**Example** : `"string"`|string|
|**returnNm**  <br>*optional*|**Example** : `"string"`|string|
|**reviewCnt**  <br>*optional*|**Example** : `"string"`|string|
|**rnum**  <br>*optional*|**Example** : `"string"`|string|
|**sellFeeRate**  <br>*optional*|**Example** : `"string"`|string|
|**separateSettingCost**  <br>*optional*|**Example** : `"string"`|string|
|**spointRate**  <br>*optional*|**Example** : `"string"`|string|
|**standardcategoryid**  <br>*optional*|**Example** : `"string"`|string|
|**stockQty**  <br>*optional*|**Example** : `"string"`|string|
|**supplyProdCd**  <br>*optional*|**Example** : `"string"`|string|
|**totalCnt**  <br>*optional*|**Example** : `"string"`|string|
|**totalSellQty**  <br>*optional*|**Example** : `"string"`|string|
|**upDt**  <br>*optional*|**Example** : `"string"`|string|
|**weekSellQty**  <br>*optional*|**Example** : `"string"`|string|


<a name="partnerproductstatuscountdto"></a>
### PartnerProductStatusCountDTO

|Name|Description|Schema|
|---|---|---|
|**cntByProdStsCd**  <br>*optional*|**Example** : `"string"`|string|
|**prodStsCd**  <br>*optional*|**Example** : `"string"`|string|
|**totalCnt**  <br>*optional*|**Example** : `"string"`|string|


<a name="productdetaildto"></a>
### ProductDetailDTO

|Name|Description|Schema|
|---|---|---|
|**adminMemo**  <br>*optional*|**Example** : `"string"`|string|
|**brandCd**  <br>*optional*|**Example** : `"string"`|string|
|**changeAbleyn**  <br>*optional*|**Example** : `"string"`|string|
|**changeFeeFreeYn**  <br>*optional*|**Example** : `"string"`|string|
|**codYn**  <br>*optional*|**Example** : `"string"`|string|
|**colorCd**  <br>*optional*|**Example** : `"string"`|string|
|**colorYn**  <br>*optional*|**Example** : `"string"`|string|
|**confirmDt**  <br>*optional*|**Example** : `"string"`|string|
|**confirmField**  <br>*optional*|**Example** : `"string"`|string|
|**confirmImgPath**  <br>*optional*|**Example** : `"string"`|string|
|**confirmInstitute**  <br>*optional*|**Example** : `"string"`|string|
|**confirmNo**  <br>*optional*|**Example** : `"string"`|string|
|**confirmValidEndDt**  <br>*optional*|**Example** : `"string"`|string|
|**confirmValidStartDt**  <br>*optional*|**Example** : `"string"`|string|
|**dcRate**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryDt**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryFee**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocCd**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryMethod**  <br>*optional*|**Example** : `"string"`|string|
|**exceptEntrYn**  <br>*optional*|**Example** : `"string"`|string|
|**gratitudeDesc**  <br>*optional*|**Example** : `"string"`|string|
|**importNo**  <br>*optional*|**Example** : `"string"`|string|
|**importationGb**  <br>*optional*|**Example** : `"string"`|string|
|**importerNm**  <br>*optional*|**Example** : `"string"`|string|
|**issueDt**  <br>*optional*|**Example** : `"string"`|string|
|**itemYy**  <br>*optional*|**Example** : `"string"`|string|
|**itemkindCd**  <br>*optional*|**Example** : `"string"`|string|
|**kcGb**  <br>*optional*|**Example** : `"string"`|string|
|**listPrice**  <br>*optional*|**Example** : `"string"`|string|
|**mainImgUrl**  <br>*optional*|**Example** : `"string"`|string|
|**makeDt**  <br>*optional*|**Example** : `"string"`|string|
|**makeNm**  <br>*optional*|**Example** : `"string"`|string|
|**makeYear**  <br>*optional*|**Example** : `"string"`|string|
|**materialDesc**  <br>*optional*|**Example** : `"string"`|string|
|**maxOrdQty**  <br>*optional*|**Example** : `"string"`|string|
|**mdId**  <br>*optional*|**Example** : `"string"`|string|
|**mdNm**  <br>*optional*|**Example** : `"string"`|string|
|**minOrdAmt**  <br>*optional*|**Example** : `"string"`|string|
|**minOrdQty**  <br>*optional*|**Example** : `"string"`|string|
|**minorBuyYn**  <br>*optional*|**Example** : `"string"`|string|
|**modelCd**  <br>*optional*|**Example** : `"string"`|string|
|**modelNm**  <br>*optional*|**Example** : `"string"`|string|
|**nativeCd**  <br>*optional*|**Example** : `"string"`|string|
|**nativeDetail**  <br>*optional*|**Example** : `"string"`|string|
|**notiList**  <br>*optional*|**Example** : `[ "[productinformationnoticeinfodto](#productinformationnoticeinfodto)" ]`|< [ProductInformationNoticeInfoDTO](#productinformationnoticeinfodto) > array|
|**optionList**  <br>*optional*|**Example** : `[ "[productoptiondto](#productoptiondto)" ]`|< [ProductOptionDTO](#productoptiondto) > array|
|**optionSetYn**  <br>*optional*|**Example** : `"string"`|string|
|**orderMakingRd**  <br>*optional*|**Example** : `"string"`|string|
|**overseasAddr**  <br>*optional*|**Example** : `"string"`|string|
|**overseasAgency**  <br>*optional*|**Example** : `"string"`|string|
|**overseasBizno**  <br>*optional*|**Example** : `"string"`|string|
|**overseasSeller**  <br>*optional*|**Example** : `"string"`|string|
|**priceResYn**  <br>*optional*|**Example** : `"string"`|string|
|**prodCd**  <br>*optional*|**Example** : `"string"`|string|
|**prodDesc**  <br>*optional*|**Example** : `"string"`|string|
|**prodNm**  <br>*optional*|**Example** : `"string"`|string|
|**prodNmEng**  <br>*optional*|**Example** : `"string"`|string|
|**prodPrice**  <br>*optional*|**Example** : `"string"`|string|
|**prodSexGb**  <br>*optional*|**Example** : `"string"`|string|
|**prodSpecCd**  <br>*optional*|**Example** : `"string"`|string|
|**prodStockQty**  <br>*optional*|**Example** : `"string"`|string|
|**prodStsCd**  <br>*optional*|**Example** : `"string"`|string|
|**prodStsNm**  <br>*optional*|**Example** : `"string"`|string|
|**prodWeight**  <br>*optional*|**Example** : `"string"`|string|
|**productOriginPrice**  <br>*optional*|**Example** : `"string"`|string|
|**regDt**  <br>*optional*|**Example** : `"string"`|string|
|**returnAbleyn**  <br>*optional*|**Example** : `"string"`|string|
|**returnFeeFreeYn**  <br>*optional*|**Example** : `"string"`|string|
|**safeConfirmYn**  <br>*optional*|**Example** : `"string"`|string|
|**seasonCd**  <br>*optional*|**Example** : `"string"`|string|
|**sellFeeRate**  <br>*optional*|**Example** : `"string"`|string|
|**sellfeerateResYn**  <br>*optional*|**Example** : `"string"`|string|
|**separateSettingCost**  <br>*optional*|**Example** : `"string"`|string|
|**simpleProductExplain**  <br>*optional*|**Example** : `"string"`|string|
|**soldoutDisplayYn**  <br>*optional*|**Example** : `"string"`|string|
|**soldoutDisplayoptYn**  <br>*optional*|**Example** : `"string"`|string|
|**spointRate**  <br>*optional*|**Example** : `"string"`|string|
|**standardcategory1deptCd**  <br>*optional*|**Example** : `"string"`|string|
|**standardcategory2deptCd**  <br>*optional*|**Example** : `"string"`|string|
|**standardcategory3deptCd**  <br>*optional*|**Example** : `"string"`|string|
|**standardcategoryid**  <br>*optional*|**Example** : `"string"`|string|
|**styleYy**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrCd**  <br>*optional*|**Example** : `"string"`|string|
|**supplyProdCd**  <br>*optional*|**Example** : `"string"`|string|
|**supplyProdNm**  <br>*optional*|**Example** : `"string"`|string|
|**validDays**  <br>*optional*|**Example** : `"string"`|string|
|**validDt**  <br>*optional*|**Example** : `"string"`|string|
|**vatCd**  <br>*optional*|**Example** : `"string"`|string|


<a name="productinfodto"></a>
### ProductInfoDTO

|Name|Description|Schema|
|---|---|---|
|**adminMemo**  <br>*optional*|**Example** : `"string"`|string|
|**brandCd**  <br>*optional*|**Example** : `"string"`|string|
|**changeAbleyn**  <br>*optional*|**Example** : `"string"`|string|
|**changeFeeFreeYn**  <br>*optional*|**Example** : `"string"`|string|
|**codYn**  <br>*optional*|**Example** : `"string"`|string|
|**colorCd**  <br>*optional*|**Example** : `"string"`|string|
|**colorYn**  <br>*optional*|**Example** : `"string"`|string|
|**confirmNo**  <br>*optional*|**Example** : `"string"`|string|
|**dcRate**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryDt**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryFee**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocCd**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryMethod**  <br>*optional*|**Example** : `"string"`|string|
|**importationGb**  <br>*optional*|**Example** : `"string"`|string|
|**itemYy**  <br>*optional*|**Example** : `"string"`|string|
|**itemkindCd**  <br>*optional*|**Example** : `"string"`|string|
|**kcGb**  <br>*optional*|**Example** : `"string"`|string|
|**listPrice**  <br>*optional*|**Example** : `"string"`|string|
|**makeNm**  <br>*optional*|**Example** : `"string"`|string|
|**maxOrdQty**  <br>*optional*|**Example** : `"string"`|string|
|**mdId**  <br>*optional*|**Example** : `"string"`|string|
|**minOrdAmt**  <br>*optional*|**Example** : `"string"`|string|
|**minOrdQty**  <br>*optional*|**Example** : `"string"`|string|
|**minorBuyYn**  <br>*optional*|**Example** : `"string"`|string|
|**modelCd**  <br>*optional*|**Example** : `"string"`|string|
|**modelNm**  <br>*optional*|**Example** : `"string"`|string|
|**nativeCd**  <br>*optional*|**Example** : `"string"`|string|
|**niCd0**  <br>*optional*|**Example** : `"string"`|string|
|**niCd1**  <br>*optional*|**Example** : `"string"`|string|
|**niCd10**  <br>*optional*|**Example** : `"string"`|string|
|**niCd11**  <br>*optional*|**Example** : `"string"`|string|
|**niCd12**  <br>*optional*|**Example** : `"string"`|string|
|**niCd13**  <br>*optional*|**Example** : `"string"`|string|
|**niCd14**  <br>*optional*|**Example** : `"string"`|string|
|**niCd2**  <br>*optional*|**Example** : `"string"`|string|
|**niCd3**  <br>*optional*|**Example** : `"string"`|string|
|**niCd4**  <br>*optional*|**Example** : `"string"`|string|
|**niCd5**  <br>*optional*|**Example** : `"string"`|string|
|**niCd6**  <br>*optional*|**Example** : `"string"`|string|
|**niCd7**  <br>*optional*|**Example** : `"string"`|string|
|**niCd8**  <br>*optional*|**Example** : `"string"`|string|
|**niCd9**  <br>*optional*|**Example** : `"string"`|string|
|**niTypeCd**  <br>*optional*|**Example** : `"string"`|string|
|**optionSetYn**  <br>*optional*|**Example** : `"string"`|string|
|**orderMakingRd**  <br>*optional*|**Example** : `"string"`|string|
|**overseasAddr**  <br>*optional*|**Example** : `"string"`|string|
|**overseasAgency**  <br>*optional*|**Example** : `"string"`|string|
|**overseasBizno**  <br>*optional*|**Example** : `"string"`|string|
|**overseasSeller**  <br>*optional*|**Example** : `"string"`|string|
|**prodCd**  <br>*optional*|**Example** : `"string"`|string|
|**prodDesc**  <br>*optional*|**Example** : `"string"`|string|
|**prodNm**  <br>*optional*|**Example** : `"string"`|string|
|**prodPrice**  <br>*optional*|**Example** : `"string"`|string|
|**prodSexGb**  <br>*optional*|**Example** : `"string"`|string|
|**prodSpecCd**  <br>*optional*|**Example** : `"string"`|string|
|**prodStockQty**  <br>*optional*|**Example** : `"string"`|string|
|**prodStsCd**  <br>*optional*|**Example** : `"string"`|string|
|**productOptionInfo**  <br>*optional*|**Example** : `"[productoptioninfodto](#productoptioninfodto)"`|[ProductOptionInfoDTO](#productoptioninfodto)|
|**productOriginPrice**  <br>*optional*|**Example** : `"string"`|string|
|**propertyList**  <br>*optional*|**Example** : `[ "string" ]`|< string > array|
|**regId**  <br>*optional*|**Example** : `"string"`|string|
|**returnAbleyn**  <br>*optional*|**Example** : `"string"`|string|
|**returnFeeFreeYn**  <br>*optional*|**Example** : `"string"`|string|
|**seasonCd**  <br>*optional*|**Example** : `"string"`|string|
|**sellFeeRate**  <br>*optional*|**Example** : `"string"`|string|
|**separateSettingCost**  <br>*optional*|**Example** : `"string"`|string|
|**soldoutDisplayYn**  <br>*optional*|**Example** : `"string"`|string|
|**soldoutDisplayoptYn**  <br>*optional*|**Example** : `"string"`|string|
|**spointRate**  <br>*optional*|**Example** : `"string"`|string|
|**standardcategoryid**  <br>*optional*|**Example** : `"string"`|string|
|**supplyEntrCd**  <br>*optional*|**Example** : `"string"`|string|
|**supplyProdCd**  <br>*optional*|**Example** : `"string"`|string|
|**vatCd**  <br>*optional*|**Example** : `"string"`|string|


<a name="productinformationnoticeinfodto"></a>
### ProductInformationNoticeInfoDTO

|Name|Description|Schema|
|---|---|---|
|**niCd**  <br>*optional*|**Example** : `"string"`|string|
|**niCdNm**  <br>*optional*|**Example** : `"string"`|string|
|**niCdNm2**  <br>*optional*|**Example** : `"string"`|string|
|**niTypeCd**  <br>*optional*|**Example** : `"string"`|string|
|**niTypeCdNm**  <br>*optional*|**Example** : `"string"`|string|
|**niValue**  <br>*optional*|**Example** : `"string"`|string|
|**niValue2**  <br>*optional*|**Example** : `"string"`|string|
|**niValueGb**  <br>*optional*|**Example** : `"string"`|string|
|**prodCd**  <br>*optional*|**Example** : `"string"`|string|


<a name="productoptiondto"></a>
### ProductOptionDTO

|Name|Description|Schema|
|---|---|---|
|**enterpriseOptionCd**  <br>*optional*|**Example** : `"string"`|string|
|**extraCharge**  <br>*optional*|**Example** : `"string"`|string|
|**optionNm1**  <br>*optional*|**Example** : `"string"`|string|
|**optionNm2**  <br>*optional*|**Example** : `"string"`|string|
|**optionValue1**  <br>*optional*|**Example** : `"string"`|string|
|**optionValue2**  <br>*optional*|**Example** : `"string"`|string|
|**priority**  <br>*optional*|**Example** : `"string"`|string|
|**prodOptionCd**  <br>*optional*|**Example** : `"string"`|string|
|**saleAbleYn**  <br>*optional*|**Example** : `"string"`|string|
|**stockQty**  <br>*optional*|**Example** : `"string"`|string|
|**useYn**  <br>*optional*|**Example** : `"string"`|string|


<a name="productoptioninfodto"></a>
### ProductOptionInfoDTO

|Name|Description|Schema|
|---|---|---|
|**optionList**  <br>*optional*|**Example** : `[ "[productoptiondto](#productoptiondto)" ]`|< [ProductOptionDTO](#productoptiondto) > array|
|**optionSetYn**  <br>*optional*|**Example** : `"string"`|string|
|**prodStockQty**  <br>*optional*|**Example** : `"string"`|string|


<a name="productpropertyinfodto"></a>
### ProductPropertyInfoDTO

|Name|Description|Schema|
|---|---|---|
|**checkId1**  <br>*optional*|**Example** : `"string"`|string|
|**checkId2**  <br>*optional*|**Example** : `"string"`|string|
|**checkId3**  <br>*optional*|**Example** : `"string"`|string|
|**checkId4**  <br>*optional*|**Example** : `"string"`|string|
|**checkId5**  <br>*optional*|**Example** : `"string"`|string|
|**id1**  <br>*optional*|**Example** : `"string"`|string|
|**id2**  <br>*optional*|**Example** : `"string"`|string|
|**id3**  <br>*optional*|**Example** : `"string"`|string|
|**id4**  <br>*optional*|**Example** : `"string"`|string|
|**id5**  <br>*optional*|**Example** : `"string"`|string|
|**propertyId**  <br>*optional*|**Example** : `"string"`|string|
|**propertyName**  <br>*optional*|**Example** : `"string"`|string|
|**rowNo**  <br>*optional*|**Example** : `"string"`|string|
|**rowSpan**  <br>*optional*|**Example** : `"string"`|string|
|**value1**  <br>*optional*|**Example** : `"string"`|string|
|**value2**  <br>*optional*|**Example** : `"string"`|string|
|**value3**  <br>*optional*|**Example** : `"string"`|string|
|**value4**  <br>*optional*|**Example** : `"string"`|string|
|**value5**  <br>*optional*|**Example** : `"string"`|string|


<a name="productpropertyvaluedto"></a>
### ProductPropertyValueDTO

|Name|Description|Schema|
|---|---|---|
|**prodCd**  <br>*optional*|**Example** : `"string"`|string|
|**propertyValueId**  <br>*optional*|**Example** : `"string"`|string|


<a name="standardcategoryinfodto"></a>
### StandardCategoryInfoDTO

|Name|Description|Schema|
|---|---|---|
|**code**  <br>*optional*|**Example** : `"string"`|string|
|**codeNm**  <br>*optional*|**Example** : `"string"`|string|
|**createymdt**  <br>*optional*|**Example** : `"string"`|string|
|**creatorid**  <br>*optional*|**Example** : `"string"`|string|
|**depth**  <br>*optional*|**Example** : `"string"`|string|
|**modifierid**  <br>*optional*|**Example** : `"string"`|string|
|**modifyymdt**  <br>*optional*|**Example** : `"string"`|string|
|**parentId**  <br>*optional*|**Example** : `"string"`|string|
|**usable**  <br>*optional*|**Example** : `"string"`|string|


<a name="supplybrandinfodto"></a>
### SupplyBrandInfoDTO

|Name|Description|Schema|
|---|---|---|
|**brandCd**  <br>*optional*|**Example** : `"string"`|string|
|**brandEnm**  <br>*optional*|**Example** : `"string"`|string|
|**brandNm**  <br>*optional*|**Example** : `"string"`|string|
|**confirmYn**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryFee**  <br>*optional*|**Example** : `0`|integer (int32)|
|**deliveryLocCd**  <br>*optional*|**Example** : `"string"`|string|
|**deliveryLocNm**  <br>*optional*|**Example** : `"string"`|string|
|**mgrId**  <br>*optional*|**Example** : `"string"`|string|
|**minOrdAmt**  <br>*optional*|**Example** : `0`|integer (int32)|
|**num**  <br>*optional*|**Example** : `0`|integer (int32)|
|**supplyEntrCd**  <br>*optional*|**Example** : `"string"`|string|
|**tbrandEnm**  <br>*optional*|**Example** : `"string"`|string|
|**useYn**  <br>*optional*|**Example** : `"string"`|string|


<a name="symbolinfodto"></a>
### SymbolInfoDTO

|Name|Description|Schema|
|---|---|---|
|**code**  <br>*optional*|**Example** : `"string"`|string|





