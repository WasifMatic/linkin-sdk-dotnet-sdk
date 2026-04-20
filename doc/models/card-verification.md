
# Card Verification

The API caller can opt in to verify the card through PayPal offered verification services (e.g. Smart Dollar Auth, 3DS).

*This model accepts additional fields of type JsonValue.*

## Structure

`CardVerification`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Method` | [`OrdersCardVerificationMethod?`](../../doc/models/orders-card-verification-method.md) | Optional | The method used for card verification.<br><br>**Default**: `OrdersCardVerificationMethod.SCA_WHEN_REQUIRED`<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `255`, *Pattern*: `^[0-9A-Z_]+$` |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "method": "SCA_WHEN_REQUIRED",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

