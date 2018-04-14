# Create bookingBusiness

Use this API to create a new bookingBusiness.
## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) |    |
|Delegated (personal Microsoft account) |    |
|Application |  | 

## HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer {code}|

## Request body
In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.


## Response
If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.

## Example
##### Request
The following is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_bookingbusiness_from_bookingbusinesses"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Content-type: application/json
Content-length: 441

{
  "businessType": "businessType-value",
  "address": {
    "type": "type-value",
    "postOfficeBox": "postOfficeBox-value",
    "street": "street-value",
    "city": "city-value",
    "state": "state-value",
    "countryOrRegion": "countryOrRegion-value",
    "postalCode": "postalCode-value"
  },
  "phone": "phone-value",
  "email": "email-value",
  "webSiteUrl": "webSiteUrl-value",
  "defaultCurrencyIso": "defaultCurrencyIso-value"
}
```
In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.
##### Response
The following is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 441

{
  "businessType": "businessType-value",
  "address": {
    "type": "type-value",
    "postOfficeBox": "postOfficeBox-value",
    "street": "street-value",
    "city": "city-value",
    "state": "state-value",
    "countryOrRegion": "countryOrRegion-value",
    "postalCode": "postalCode-value"
  },
  "phone": "phone-value",
  "email": "email-value",
  "webSiteUrl": "webSiteUrl-value",
  "defaultCurrencyIso": "defaultCurrencyIso-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->