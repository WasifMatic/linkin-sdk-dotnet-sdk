
# Error Details

The error details. Required for client-side `4XX` errors.

*This model accepts additional fields of type JsonValue.*

## Structure

`ErrorDetails`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Field` | `string` | Optional | The field that caused the error. If this field is in the body, set this value to the field's JSON pointer value. Required for client-side errors. |
| `MValue` | `string` | Optional | The value of the field that caused the error. |
| `Location` | `string` | Optional | The location of the field that caused the error. Value is `body`, `path`, or `query`.<br><br>**Default**: `"body"` |
| `Issue` | `string` | Required | The unique, fine-grained application-level error code. |
| `Links` | [`List<LinkDescription>`](../../doc/models/link-description.md) | Optional | An array of request-related [HATEOAS links](/api/rest/responses/#hateoas-links) that are either relevant to the issue by providing additional information or offering potential resolutions.<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `4` |
| `Description` | `string` | Optional | The human-readable description for an issue. The description can change over the lifetime of an API, so clients must not depend on this value. |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "location": "body",
  "issue": "issue8",
  "field": "field0",
  "value": "value8",
  "links": [
    {
      "href": "href6",
      "rel": "rel0",
      "method": "HEAD",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
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
  "description": "description4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

