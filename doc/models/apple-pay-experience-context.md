
# Apple Pay Experience Context

Customizes the payer experience during the approval process for the payment.

*This model accepts additional fields of type JsonValue.*

## Structure

`ApplePayExperienceContext`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `ReturnUrl` | `string` | Required | Describes the URL. |
| `CancelUrl` | `string` | Required | Describes the URL. |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "return_url": "return_url6",
  "cancel_url": "cancel_url8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

