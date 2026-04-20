
# Plan

The merchant level Recurring Billing plan metadata for the Billing Agreement.

*This model accepts additional fields of type JsonValue.*

## Structure

`Plan`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `BillingCycles` | [`List<BillingCycle>`](../../doc/models/billing-cycle.md) | Required | An array of billing cycles for trial billing and regular billing. A plan can have at most two trial cycles and only one regular cycle.<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `3` |
| `OneTimeCharges` | [`OneTimeCharge`](../../doc/models/one-time-charge.md) | Required | The one-time charge info at the time of checkout. |
| `Name` | `string` | Optional | Name of the recurring plan.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `127`, *Pattern*: `^[A-Za-z0-9() +',.:-]+$` |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "billing_cycles": [
    {
      "tenure_type": "REGULAR",
      "total_cycles": 1,
      "sequence": 1,
      "pricing_scheme": {
        "price": {
          "currency_code": "currency_code8",
          "value": "value4",
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        },
        "pricing_model": "AUTO_RELOAD",
        "reload_threshold_amount": {
          "currency_code": "currency_code0",
          "value": "value6",
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
      "start_date": "start_date6",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "one_time_charges": {
    "setup_fee": {
      "currency_code": "currency_code8",
      "value": "value4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    "shipping_amount": {
      "currency_code": "currency_code0",
      "value": "value6",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    "taxes": {
      "currency_code": "currency_code6",
      "value": "value2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    "product_price": {
      "currency_code": "currency_code6",
      "value": "value2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    "subtotal": {
      "currency_code": "currency_code2",
      "value": "value8",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    "total_amount": {
      "currency_code": "currency_code2",
      "value": "value8",
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
  "name": "name8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

