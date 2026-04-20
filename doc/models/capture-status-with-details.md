
# Capture Status with Details

The status and status details of a captured payment.

*This model accepts additional fields of type JsonValue.*

## Structure

`CaptureStatusWithDetails`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Status` | [`CaptureStatus?`](../../doc/models/capture-status.md) | Optional | The status of the captured payment. |
| `StatusDetails` | [`CaptureStatusDetails`](../../doc/models/capture-status-details.md) | Optional | The details of the captured payment status. |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "status": "COMPLETED",
  "status_details": {
    "reason": "VERIFICATION_REQUIRED",
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

