
# Blik Level 0 Payment Object

Information used to pay using BLIK level_0 flow.

*This model accepts additional fields of type JsonValue.*

## Structure

`BlikLevel0PaymentObject`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `AuthCode` | `string` | Required | The 6-digit code used to authenticate a consumer within BLIK.<br><br>**Constraints**: *Minimum Length*: `6`, *Maximum Length*: `6`, *Pattern*: `^[0-9]{6}$` |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "auth_code": "auth_code6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

