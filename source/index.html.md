---
title: DA GLHF - Calendar REST API 

language_tabs: # must be one of https://git.io/vQNgJ
  - shell

toc_footers:
  - Ria Florensi Azhar - DA GLHF - 2019

search: true
---

# Introduction
Halo ini Project Slate DA-GLHF. Walau dokumentasi ini masih banyak kekurangan, mohon maaf yaa, semoga lain kali lebih baik lagi. Mohon bantuannya. Mangatss

**Version:** 1.0.0 

# Get Target Calendar
Ini api untuk mendapatkan nama hari dan pekan keberapa apabila diberikan input berupa tanggal.

### HTTP Request

> To get target calendar, use this code

```shell
curl "http://localhost:8080/get/detail/{target}"
```

`GET http://localhost:8080/get/detail/{target}`

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| target | path | target | Yes | string |

### Response

> Response Success Example

```
{
  "body": {},
  "statusCode": "100 CONTINUE",
  "statusCodeValue": 0
}
```

**HTTP Response Code**

<table>
  <thead>
    <tr>
      <td>Code</td>
      <td>Description</td>
    </tr>
  </thead>
  <tbody>
    <tr style="color:green;">
      <td>200</td>
      <td>OK</td>
    </tr>
    <tr style="color:red;">
      <td>401</td>
      <td>Unauthorize</td>
    </tr>
    <tr style="color:red;">
      <td>403</td>
      <td>Forbidden</td>
    </tr>
    <tr style="color:red;">
      <td>404</td>
      <td>Not Found</td>
    </tr>
  </tbody>
</table>

**Response Entity**
<table>
  <thead>
    <tr>
      <th>Properties</th>
      <th>Type</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>body</td>
      <td>Object</td>
    </tr>
    <tr>
      <td>statusCode</td>
      <td>Enum <br/> 
      ```- 100 CONTINUE```<br/>
          ```- 101 SWITCHING_PROTOCOLS```<br/>
          ```- 102 PROCESSING```<br/>
          ```- 103 CHECKPOINT```<br/>
          ```- 200 OK```<br/>
          ```- 201 CREATED```<br/>
          ```- 202 ACCEPTED```<br/>
          ```- 203 NON_AUTHORITATIVE_INFORMATION```<br/>
          ```- 204 NO_CONTENT```<br/>
          ```- 205 RESET_CONTENT```<br/>
          ```- 206 PARTIAL_CONTENT```<br/>
          ```- 207 MULTI_STATUS```<br/>
          ```- 208 ALREADY_REPORTED```<br/>
          ```- 226 IM_USED```<br/>
          ```- 300 MULTIPLE_CHOICES```<br/>
          ```- 301 MOVED_PERMANENTLY```<br/>
          ```- 302 FOUND```<br/>
          ```- 302 MOVED_TEMPORARILY```<br/>
          ```- 303 SEE_OTHER```<br/>
          ```- 304 NOT_MODIFIED```<br/>
          ```- 305 USE_PROXY```<br/>
          ```- 307 TEMPORARY_REDIRECT```<br/>
          ```- 308 PERMANENT_REDIRECT```<br/>
          ```- 400 BAD_REQUEST```<br/>
          ```- 401 UNAUTHORIZED```<br/>
          ```- 402 PAYMENT_REQUIRED```<br/>
          ```- 403 FORBIDDEN```<br/>
          ```- 404 NOT_FOUND```<br/>
          ```- 405 METHOD_NOT_ALLOWED```<br/>
          ```- 406 NOT_ACCEPTABLE```<br/>
          ```- 407 PROXY_AUTHENTICATION_REQUIRED```<br/>
          ```- 408 REQUEST_TIMEOUT```<br/>
          ```- 409 CONFLICT```<br/>
          ```- 410 GONE```<br/>
          ```- 411 LENGTH_REQUIRED```<br/>
          ```- 412 PRECONDITION_FAILED```<br/>
          ```- 413 PAYLOAD_TOO_LARGE```<br/>
          ```- 413 REQUEST_ENTITY_TOO_LARGE```<br/>
          ```- 414 URI_TOO_LONG```<br/>
          ```- 414 REQUEST_URI_TOO_LONG```<br/>
          ```- 415 UNSUPPORTED_MEDIA_TYPE```<br/>
          ```- 416 REQUESTED_RANGE_NOT_SATISFIABLE```<br/>
          ```- 417 EXPECTATION_FAILED```<br/>
          ```- 418 I_AM_A_TEAPOT```<br/>
          ```- 419 INSUFFICIENT_SPACE_ON_RESOURCE```<br/>
          ```- 420 METHOD_FAILURE```<br/>
          ```- 421 DESTINATION_LOCKED```<br/>
          ```- 422 UNPROCESSABLE_ENTITY```<br/>
          ```- 423 LOCKED```<br/>
          ```- 424 FAILED_DEPENDENCY```<br/>
          ```- 425 TOO_EARLY```<br/>
          ```- 426 UPGRADE_REQUIRED```<br/>
          ```- 428 PRECONDITION_REQUIRED```<br/>
          ```- 429 TOO_MANY_REQUESTS```<br/>
          ```- 431 REQUEST_HEADER_FIELDS_TOO_LARGE```<br/>
          ```- 451 UNAVAILABLE_FOR_LEGAL_REASONS```<br/>
          ```- 500 INTERNAL_SERVER_ERROR```<br/>
          ```- 501 NOT_IMPLEMENTED```<br/>
          ```- 502 BAD_GATEWAY```<br/>
          ```- 503 SERVICE_UNAVAILABLE```<br/>
          ```- 504 GATEWAY_TIMEOUT```<br/>
          ```- 505 HTTP_VERSION_NOT_SUPPORTED```<br/>
          ```- 506 VARIANT_ALSO_NEGOTIATES```<br/>
          ```- 507 INSUFFICIENT_STORAGE```<br/>
          ```- 508 LOOP_DETECTED```<br/>
          ```- 509 BANDWIDTH_LIMIT_EXCEEDED```<br/>
          ```- 510 NOT_EXTENDED```<br/>
          ```- 511 NETWORK_AUTHENTICATION_REQUIRED```<br/>
    </td>
    </tr>
    <tr>
      <td>statusCodeValue</td>
      <td>integer</td>
    </tr>
  </tbody>
</table>

