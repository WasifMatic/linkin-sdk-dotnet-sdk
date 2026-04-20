
# Mobile Web Context

Buyer's mobile web browser context to app switch to the PayPal consumer app.

*This model accepts additional fields of type JsonValue.*

## Structure

`MobileWebContext`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `ReturnFlow` | [`MobileReturnFlow?`](../../doc/models/mobile-return-flow.md) | Optional | Merchant preference on how the buyer can navigate back to merchant website post approving the transaction on the PayPal App.<br><br>**Default**: `MobileReturnFlow.AUTO`<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `6`, *Pattern*: `^[A-Z_]+$` |
| `BuyerUserAgent` | `string` | Optional | User agent from the request originating from the buyer's device. This will be used to identify the buyer's operating system and browser versions. NOTE: Merchants must not alter or modify the buyer's device user agent.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `512`, *Pattern*: `^.*$` |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "return_flow": "AUTO",
  "buyer_user_agent": "buyer_user_agent8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

