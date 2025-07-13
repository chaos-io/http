# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [http/authority.proto](#http_authority-proto)
    - [Authority](#http-Authority)
  
- [http/string_values.proto](#http_string_values-proto)
    - [StringValues](#http-StringValues)
  
- [http/header.proto](#http_header-proto)
    - [Header](#http-Header)
    - [Header.ValsEntry](#http-Header-ValsEntry)
  
- [http/method.proto](#http_method-proto)
    - [Method](#http-Method)
  
- [http/query.proto](#http_query-proto)
    - [Query](#http-Query)
    - [Query.ValsEntry](#http-Query-ValsEntry)
  
- [http/url.proto](#http_url-proto)
    - [Url](#http-Url)
  
- [http/version.proto](#http_version-proto)
    - [Version](#http-Version)
  
- [http/request.proto](#http_request-proto)
    - [Request](#http-Request)
  
- [Scalar Value Types](#scalar-value-types)



<a name="http_authority-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## http/authority.proto



<a name="http-Authority"></a>

### Authority



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| user_info | [string](#string) |  |  |
| host | [string](#string) |  |  |
| port | [string](#string) |  |  |





 

 

 

 



<a name="http_string_values-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## http/string_values.proto



<a name="http-StringValues"></a>

### StringValues



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| vals | [string](#string) | repeated |  |





 

 

 

 



<a name="http_header-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## http/header.proto



<a name="http-Header"></a>

### Header



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| Vals | [Header.ValsEntry](#http-Header-ValsEntry) | repeated |  |






<a name="http-Header-ValsEntry"></a>

### Header.ValsEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [StringValues](#http-StringValues) |  |  |





 

 

 

 



<a name="http_method-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## http/method.proto


 


<a name="http-Method"></a>

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


 

 

 



<a name="http_query-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## http/query.proto



<a name="http-Query"></a>

### Query



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| Vals | [Query.ValsEntry](#http-Query-ValsEntry) | repeated |  |






<a name="http-Query-ValsEntry"></a>

### Query.ValsEntry



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| key | [string](#string) |  |  |
| value | [StringValues](#http-StringValues) |  |  |





 

 

 

 



<a name="http_url-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## http/url.proto



<a name="http-Url"></a>

### Url



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| scheme | [string](#string) |  |  |
| authority | [Authority](#http-Authority) |  |  |
| path | [string](#string) |  |  |
| raw_path | [string](#string) |  |  |
| query | [Query](#http-Query) |  |  |
| raw_query | [string](#string) |  |  |
| fragment | [string](#string) |  |  |
| raw_fragment | [string](#string) |  |  |





 

 

 

 



<a name="http_version-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## http/version.proto



<a name="http-Version"></a>

### Version



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| proto | [string](#string) |  |  |
| major | [int32](#int32) |  |  |
| minor | [int32](#int32) |  |  |





 

 

 

 



<a name="http_request-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## http/request.proto



<a name="http-Request"></a>

### Request



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| method | [Method](#http-Method) |  |  |
| url | [Url](#http-Url) |  |  |
| version | [Version](#http-Version) |  |  |
| header | [Header](#http-Header) |  |  |
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

