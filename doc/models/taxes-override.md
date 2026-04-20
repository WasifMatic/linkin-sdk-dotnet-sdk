
# Taxes Override

The tax details.

*This model accepts additional fields of type JsonValue.*

## Structure

`TaxesOverride`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Percentage` | `string` | Optional | The percentage, as a fixed-point, signed decimal number. For example, define a 19.99% interest rate as `19.99`.<br><br>**Constraints**: *Pattern*: `^((-?[0-9]+)\|(-?([0-9]+)?[.][0-9]+))$` |
| `Inclusive` | `bool?` | Optional | Indicates whether the tax was already included in the billing amount. |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "percentage": "percentage8",
  "inclusive": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

