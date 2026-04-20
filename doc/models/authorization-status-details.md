
# Authorization Status Details

The details of the authorized payment status.

*This model accepts additional fields of type JsonValue.*

## Structure

`AuthorizationStatusDetails`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Reason` | [`AuthorizationIncompleteReason?`](../../doc/models/authorization-incomplete-reason.md) | Optional | The reason why the authorized status is `PENDING`.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `64`, *Pattern*: `^[A-Z_]+$` |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "reason": "PENDING_REVIEW",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

