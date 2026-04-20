
# Apple Pay Payment Data

Information about the decrypted apple pay payment data for the token like cryptogram, eci indicator.

*This model accepts additional fields of type JsonValue.*

## Structure

`ApplePayPaymentData`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Cryptogram` | `string` | Optional | Online payment cryptogram, as defined by 3D Secure. The pattern is defined by an external party and supports Unicode.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `2000`, *Pattern*: `^.*$` |
| `EciIndicator` | `string` | Optional | ECI indicator, as defined by 3- Secure. The pattern is defined by an external party and supports Unicode.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `256`, *Pattern*: `^.*$` |
| `EmvData` | `string` | Optional | Encoded Apple Pay EMV Payment Structure used for payments in China. The pattern is defined by an external party and supports Unicode.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `2000`, *Pattern*: `^.*$` |
| `Pin` | `string` | Optional | Bank Key encrypted Apple Pay PIN. The pattern is defined by an external party and supports Unicode.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `2000`, *Pattern*: `^.*$` |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "cryptogram": "cryptogram6",
  "eci_indicator": "eci_indicator0",
  "emv_data": "emv_data0",
  "pin": "pin4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

