
# Card Experience Context

Customizes the payer experience during the 3DS Approval for payment.

*This model accepts additional fields of type JsonValue.*

## Structure

`CardExperienceContext`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `ReturnUrl` | `string` | Optional | Describes the URL. |
| `CancelUrl` | `string` | Optional | Describes the URL. |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "return_url": "return_url2",
  "cancel_url": "cancel_url0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

