
# Update Pricing Scheme

The update pricing scheme request details.

*This model accepts additional fields of type JsonValue.*

## Structure

`UpdatePricingScheme`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `BillingCycleSequence` | `int` | Required | The billing cycle sequence.<br><br>**Constraints**: `>= 1`, `<= 99` |
| `PricingScheme` | [`SubscriptionPricingScheme`](../../doc/models/subscription-pricing-scheme.md) | Required | The pricing scheme details. |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "billing_cycle_sequence": 99,
  "pricing_scheme": {
    "version": 10,
    "fixed_price": {
      "currency_code": "currency_code4",
      "value": "value0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    "pricing_model": "VOLUME",
    "tiers": [
      {
        "starting_quantity": "starting_quantity8",
        "ending_quantity": "ending_quantity6",
        "amount": {
          "currency_code": "currency_code6",
          "value": "value0",
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        },
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      {
        "starting_quantity": "starting_quantity8",
        "ending_quantity": "ending_quantity6",
        "amount": {
          "currency_code": "currency_code6",
          "value": "value0",
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        },
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      {
        "starting_quantity": "starting_quantity8",
        "ending_quantity": "ending_quantity6",
        "amount": {
          "currency_code": "currency_code6",
          "value": "value0",
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
    ],
    "create_time": "create_time4",
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

