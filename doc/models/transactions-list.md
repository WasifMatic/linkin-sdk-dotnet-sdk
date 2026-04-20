
# Transactions List

The list transactions for a subscription request details.

*This model accepts additional fields of type JsonValue.*

## Structure

`TransactionsList`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Transactions` | [`List<SubscriptionTransactionDetails>`](../../doc/models/subscription-transaction-details.md) | Optional | An array of transactions.<br><br>**Constraints**: *Minimum Items*: `0`, *Maximum Items*: `32767` |
| `TotalItems` | `int?` | Optional | The total number of items.<br><br>**Constraints**: `>= 0`, `<= 500000000` |
| `TotalPages` | `int?` | Optional | The total number of pages.<br><br>**Constraints**: `>= 0`, `<= 100000000` |
| `Links` | [`List<LinkDescription>`](../../doc/models/link-description.md) | Optional | An array of request-related [HATEOAS links](/docs/api/reference/api-responses/#hateoas-links).<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `10` |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "transactions": [
    {
      "status": "PARTIALLY_REFUNDED",
      "id": "id8",
      "amount_with_breakdown": {
        "gross_amount": {
          "currency_code": "currency_code4",
          "value": "value0",
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        },
        "total_item_amount": {
          "currency_code": "currency_code8",
          "value": "value4",
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        },
        "fee_amount": {
          "currency_code": "currency_code2",
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
        "tax_amount": {
          "currency_code": "currency_code2",
          "value": "value8",
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        },
        "net_amount": {
          "currency_code": "currency_code6",
          "value": "value2",
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
      "payer_name": {
        "prefix": "prefix8",
        "given_name": "given_name2",
        "surname": "surname8",
        "middle_name": "middle_name0",
        "suffix": "suffix0",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "payer_email": "payer_email6",
      "time": "time8",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "total_items": 254,
  "total_pages": 34,
  "links": [
    {
      "href": "href6",
      "rel": "rel0",
      "method": "HEAD",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "href": "href6",
      "rel": "rel0",
      "method": "HEAD",
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

