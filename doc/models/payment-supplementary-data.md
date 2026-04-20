
# Payment Supplementary Data

The supplementary data.

*This model accepts additional fields of type JsonValue.*

## Structure

`PaymentSupplementaryData`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `RelatedIds` | [`RelatedIdentifiers`](../../doc/models/related-identifiers.md) | Optional | Identifiers related to a specific resource. |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "related_ids": {
    "order_id": "order_id2",
    "authorization_id": "authorization_id0",
    "capture_id": "capture_id0",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

