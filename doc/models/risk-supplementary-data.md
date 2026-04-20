
# Risk Supplementary Data

Additional information necessary to evaluate the risk profile of a transaction.

*This model accepts additional fields of type JsonValue.*

## Structure

`RiskSupplementaryData`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Customer` | [`ParticipantMetadata`](../../doc/models/participant-metadata.md) | Optional | Profile information of the sender or receiver. |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "customer": {
    "ip_address": "ip_address0",
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

