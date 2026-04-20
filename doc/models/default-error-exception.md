
# Default Error Exception

The error details.

*This model accepts additional fields of type JsonValue.*

## Structure

`DefaultErrorException`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Name` | `string` | Required | The human-readable, unique name of the error. |
| `MessageProperty` | `string` | Required | The message that describes the error. |
| `DebugId` | `string` | Required | The PayPal internal ID. Used for correlation purposes. |
| `InformationLink` | `string` | Optional | The information link, or URI, that shows detailed information about this error for the developer. |
| `Details` | [`List<TransactionSearchErrorDetails>`](../../doc/models/transaction-search-error-details.md) | Optional | An array of additional details about the error. |
| `Links` | [`List<LinkDescription>`](../../doc/models/link-description.md) | Optional | An array of request-related [HATEOAS links](/docs/api/reference/api-responses/#hateoas-links). |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "name": "name2",
  "message": "message2",
  "debug_id": "debug_id8",
  "information_link": "information_link4",
  "details": [
    {
      "field": "field4",
      "value": "value2",
      "location": "location4",
      "issue": "issue6",
      "description": "description0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "links": [
    {
      "href": "href6",
      "rel": "rel0",
      "method": "HEAD",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

