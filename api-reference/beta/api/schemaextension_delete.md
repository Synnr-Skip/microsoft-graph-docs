# Delete schemaExtension

Delete the definition of a [schema extension](../resources/schemaExtension.md).

Only the app that created the schema extension (owner app) can delete it. 
>**Warning:** There is currently a [known issue](../../../concepts/extensibility_overview.md#known-limitations-for-extensions) where you lose access to your custom data once the schema extension is deleted. 

## Prerequisites
The following **scope** is required to execute this API: *Directory.AccessAsUser.All*

## HTTP request
<!-- { "blockType": "ignored" } -->
```http
DELETE /schemaExtensions/{id}
```

## Request headers
| Name      |Description|
|:----------|:----------|
| Authorization  | Bearer &lt;token&gt;. Required. |
| Content-Type   | application/json | 

## Request body
Do not supply a request body for this method.


## Response
If successful, this method returns `204, No Content` response code. It does not return anything in the response body.

## Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/beta/schemaExtensions/{id}
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## See also

- [Add custom data to resources using extensions](../../../concepts/extensibility_overview.md)
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->