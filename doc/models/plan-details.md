
# Plan Details

The plan details.

*This model accepts additional fields of type JsonValue.*

## Structure

`PlanDetails`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `ProductId` | `string` | Optional | The ID for the product.<br><br>**Constraints**: *Minimum Length*: `22`, *Maximum Length*: `22`, *Pattern*: `^PROD-[A-Z0-9]*$` |
| `Name` | `string` | Optional | The plan name.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `127`, *Pattern*: `^.*$` |
| `Description` | `string` | Optional | The detailed description of the plan.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `127`, *Pattern*: `^.*$` |
| `BillingCycles` | [`List<SubscriptionBillingCycle>`](../../doc/models/subscription-billing-cycle.md) | Optional | An array of billing cycles for trial billing and regular billing. A plan can have at most two trial cycles and only one regular cycle.<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `12` |
| `PaymentPreferences` | [`PaymentPreferences`](../../doc/models/payment-preferences.md) | Optional | The payment preferences for a subscription. |
| `MerchantPreferences` | [`MerchantPreferences`](../../doc/models/merchant-preferences.md) | Optional | The merchant preferences for a subscription. |
| `Taxes` | [`Taxes`](../../doc/models/taxes.md) | Optional | The tax details. |
| `QuantitySupported` | `bool?` | Optional | Indicates whether you can subscribe to this plan by providing a quantity for the goods or service.<br><br>**Default**: `false` |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "quantity_supported": false,
  "product_id": "product_id6",
  "name": "name8",
  "description": "description2",
  "billing_cycles": [
    {
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
      "frequency": {
        "interval_unit": "DAY",
        "interval_count": 94,
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "tenure_type": "REGULAR",
      "sequence": 8,
      "total_cycles": 198,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
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
      "frequency": {
        "interval_unit": "DAY",
        "interval_count": 94,
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "tenure_type": "REGULAR",
      "sequence": 8,
      "total_cycles": 198,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
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
      "frequency": {
        "interval_unit": "DAY",
        "interval_count": 94,
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "tenure_type": "REGULAR",
      "sequence": 8,
      "total_cycles": 198,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "payment_preferences": {
    "auto_bill_outstanding": false,
    "setup_fee": {
      "currency_code": "currency_code8",
      "value": "value4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    "setup_fee_failure_action": "CONTINUE",
    "payment_failure_threshold": 104,
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

