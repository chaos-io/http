# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [authority.proto](#authority-proto)
    - [Authority](#http-v1-Authority)
  
- [string_values.proto](#string_values-proto)
    - [StringValues](#http-v1-StringValues)
  
- [header.proto](#header-proto)
    - [Header](#http-v1-Header)
    - [Header.ValsEntry](#http-v1-Header-ValsEntry)
  
- [http.proto](#http-proto)
    - [CreateResourceRequest](#http-v1-CreateResourceRequest)
    - [DeleteResourceRequest](#http-v1-DeleteResourceRequest)
    - [DeleteResourceResponse](#http-v1-DeleteResourceResponse)
    - [GetResourceRequest](#http-v1-GetResourceRequest)
    - [ListResourcesRequest](#http-v1-ListResourcesRequest)
    - [ListResourcesResponse](#http-v1-ListResourcesResponse)
    - [Resource](#http-v1-Resource)
    - [UpdateResourceRequest](#http-v1-UpdateResourceRequest)
  
- [method.proto](#method-proto)
    - [Method](#http-v1-Method)
  
- [query.proto](#query-proto)
    - [Query](#http-v1-Query)
    - [Query.ValsEntry](#http-v1-Query-ValsEntry)
  
- [url.proto](#url-proto)
    - [Url](#http-v1-Url)
  
- [version.proto](#version-proto)
    - [Version](#http-v1-Version)
  
- [request.proto](#request-proto)
    - [Request](#http-v1-Request)
  
- [Scalar Value Types](#scalar-value-types)



<a name="authority-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## authority.proto



<a name="http-v1-Authority"></a>

### Authority



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| user_info | [string](#string) |  |  |
| host | [string](#string) |  |  |
| port | [string](#string) |  |  |





 

 

 

 



<a name="string_values-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## string_values.proto



<a name="http-v1-StringValues"></a>

### StringValues



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| vals | [string](#string) | repeated |  |





 

 

 

 



<a name="header-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## header.proto



<a name="http-v1-Header"></a>

### Header



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| Vals | [Header.ValsEntry](#http-v1-Header-ValsEntry) | repeated |  |






<a name="http-v1-Header-ValsEntry"></a>

### Header.ValsEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [StringValues](#http-v1-StringValues) |  |  |





 

 

 

 



<a name="http-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## http.proto



<a name="http-v1-CreateResourceRequest"></a>

### CreateResourceRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| resource | [Resource](#http-v1-Resource) |  |  |
| locale | [string](#string) |  |  |






<a name="http-v1-DeleteResourceRequest"></a>

### DeleteResourceRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [string](#string) |  |  |
| locale | [string](#string) |  |  |






<a name="http-v1-DeleteResourceResponse"></a>

### DeleteResourceResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [string](#string) |  |  |






<a name="http-v1-GetResourceRequest"></a>

### GetResourceRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [string](#string) |  |  |






<a name="http-v1-ListResourcesRequest"></a>

### ListResourcesRequest







<a name="http-v1-ListResourcesResponse"></a>

### ListResourcesResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| resources | [Resource](#http-v1-Resource) | repeated |  |






<a name="http-v1-Resource"></a>

### Resource



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| id | [string](#string) |  |  |
| name | [string](#string) |  |  |






<a name="http-v1-UpdateResourceRequest"></a>

### UpdateResourceRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| resource | [Resource](#http-v1-Resource) |  |  |
| locale | [string](#string) |  |  |





 

 

 

 



<a name="method-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## method.proto


 


<a name="http-v1-Method"></a>

### Method


| Name | Number | Description |
| ---- | ------ | ----------- |
| METHOD_UNSPECIFIED | 0 |  |
| METHOD_GET | 1 |  |
| METHOD_POST | 2 |  |
| METHOD_PUT | 3 |  |
| METHOD_DELETE | 4 |  |
| METHOD_CONNECT | 5 |  |
| METHOD_OPTIONS | 6 |  |
| METHOD_TRACE | 7 |  |


 

 

 



<a name="query-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## query.proto



<a name="http-v1-Query"></a>

### Query



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| Vals | [Query.ValsEntry](#http-v1-Query-ValsEntry) | repeated |  |






<a name="http-v1-Query-ValsEntry"></a>

### Query.ValsEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [StringValues](#http-v1-StringValues) |  |  |





 

 

 

 



<a name="url-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## url.proto



<a name="http-v1-Url"></a>

### Url



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| scheme | [string](#string) |  |  |
| authority | [Authority](#http-v1-Authority) |  |  |
| path | [string](#string) |  |  |
| raw_path | [string](#string) |  |  |
| query | [Query](#http-v1-Query) |  |  |
| raw_query | [string](#string) |  |  |
| fragment | [string](#string) |  |  |
| raw_fragment | [string](#string) |  |  |





 

 

 

 



<a name="version-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## version.proto



<a name="http-v1-Version"></a>

### Version



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| proto | [string](#string) |  |  |
| major | [int32](#int32) |  |  |
| minor | [int32](#int32) |  |  |





 

 

 

 



<a name="request-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## request.proto



<a name="http-v1-Request"></a>

### Request



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| method | [Method](#http-v1-Method) |  |  |
| url | [Url](#http-v1-Url) |  |  |
| version | [Version](#http-v1-Version) |  |  |
| header | [Header](#http-v1-Header) |  |  |
| body | [google.protobuf.Value](#google-protobuf-Value) |  |  |





 

 

 

 



## Scalar Value Types

| .proto Type | Notes | C++ | Java | Python | Go | C# | PHP | Ruby |
| ----------- | ----- | --- | ---- | ------ | -- | -- | --- | ---- |
| <a name="double" /> double |  | double | double | float | float64 | double | float | Float |
| <a name="float" /> float |  | float | float | float | float32 | float | float | Float |
| <a name="int32" /> int32 | Uses variable-length encoding. Inefficient for encoding negative numbers – if your field is likely to have negative values, use sint32 instead. | int32 | int | int | int32 | int | integer | Bignum or Fixnum (as required) |
| <a name="int64" /> int64 | Uses variable-length encoding. Inefficient for encoding negative numbers – if your field is likely to have negative values, use sint64 instead. | int64 | long | int/long | int64 | long | integer/string | Bignum |
| <a name="uint32" /> uint32 | Uses variable-length encoding. | uint32 | int | int/long | uint32 | uint | integer | Bignum or Fixnum (as required) |
| <a name="uint64" /> uint64 | Uses variable-length encoding. | uint64 | long | int/long | uint64 | ulong | integer/string | Bignum or Fixnum (as required) |
| <a name="sint32" /> sint32 | Uses variable-length encoding. Signed int value. These more efficiently encode negative numbers than regular int32s. | int32 | int | int | int32 | int | integer | Bignum or Fixnum (as required) |
| <a name="sint64" /> sint64 | Uses variable-length encoding. Signed int value. These more efficiently encode negative numbers than regular int64s. | int64 | long | int/long | int64 | long | integer/string | Bignum |
| <a name="fixed32" /> fixed32 | Always four bytes. More efficient than uint32 if values are often greater than 2^28. | uint32 | int | int | uint32 | uint | integer | Bignum or Fixnum (as required) |
| <a name="fixed64" /> fixed64 | Always eight bytes. More efficient than uint64 if values are often greater than 2^56. | uint64 | long | int/long | uint64 | ulong | integer/string | Bignum |
| <a name="sfixed32" /> sfixed32 | Always four bytes. | int32 | int | int | int32 | int | integer | Bignum or Fixnum (as required) |
| <a name="sfixed64" /> sfixed64 | Always eight bytes. | int64 | long | int/long | int64 | long | integer/string | Bignum |
| <a name="bool" /> bool |  | bool | boolean | boolean | bool | bool | boolean | TrueClass/FalseClass |
| <a name="string" /> string | A string must always contain UTF-8 encoded or 7-bit ASCII text. | string | String | str/unicode | string | string | string | String (UTF-8) |
| <a name="bytes" /> bytes | May contain any arbitrary sequence of bytes. | string | ByteString | str | []byte | ByteString | string | String (ASCII-8BIT) |

