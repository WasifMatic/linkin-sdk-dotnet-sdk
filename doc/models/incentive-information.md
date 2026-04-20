
# Incentive Information

The incentive details.

*This model accepts additional fields of type JsonValue.*

## Structure

`IncentiveInformation`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `IncentiveDetails` | [`List<IncentiveDetails>`](../../doc/models/incentive-details.md) | Optional | An array of incentive details.<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `32767` |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "incentive_details": [
    {
      "incentive_type": "incentive_type4",
      "incentive_code": "incentive_code0",
      "incentive_amount": {
        "currency_code": "currency_code4",
        "value": "value0",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "incentive_program_code": "incentive_program_code4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "incentive_type": "incentive_type4",
      "incentive_code": "incentive_code0",
      "incentive_amount": {
        "currency_code": "currency_code4",
        "value": "value0",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "incentive_program_code": "incentive_program_code4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "incentive_type": "incentive_type4",
      "incentive_code": "incentive_code0",
      "incentive_amount": {
        "currency_code": "currency_code4",
        "value": "value0",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "incentive_program_code": "incentive_program_code4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

