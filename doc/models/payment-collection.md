
# Payment Collection

The collection of payments, or transactions, for a purchase unit in an order. For example, authorized payments, captured payments, and refunds.

*This model accepts additional fields of type JsonValue.*

## Structure

`PaymentCollection`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Authorizations` | [`List<AuthorizationWithAdditionalData>`](../../doc/models/authorization-with-additional-data.md) | Optional | An array of authorized payments for a purchase unit. A purchase unit can have zero or more authorized payments. |
| `Captures` | [`List<OrdersCapture>`](../../doc/models/orders-capture.md) | Optional | An array of captured payments for a purchase unit. A purchase unit can have zero or more captured payments. |
| `Refunds` | [`List<Refund>`](../../doc/models/refund.md) | Optional | An array of refunds for a purchase unit. A purchase unit can have zero or more refunds. |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "authorizations": [
    {
      "status": "DENIED",
      "status_details": {
        "reason": "PENDING_REVIEW",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "id": "id2",
      "amount": {
        "currency_code": "currency_code6",
        "value": "value0",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "invoice_id": "invoice_id2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "status": "DENIED",
      "status_details": {
        "reason": "PENDING_REVIEW",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "id": "id2",
      "amount": {
        "currency_code": "currency_code6",
        "value": "value0",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "invoice_id": "invoice_id2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "status": "DENIED",
      "status_details": {
        "reason": "PENDING_REVIEW",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "id": "id2",
      "amount": {
        "currency_code": "currency_code6",
        "value": "value0",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "invoice_id": "invoice_id2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "captures": [
    {
      "status": "REFUNDED",
      "status_details": {
        "reason": "VERIFICATION_REQUIRED",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "id": "id4",
      "amount": {
        "currency_code": "currency_code6",
        "value": "value0",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "invoice_id": "invoice_id4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "status": "REFUNDED",
      "status_details": {
        "reason": "VERIFICATION_REQUIRED",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "id": "id4",
      "amount": {
        "currency_code": "currency_code6",
        "value": "value0",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "invoice_id": "invoice_id4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "refunds": [
    {
      "status": "CANCELLED",
      "status_details": {
        "reason": "ECHECK",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "id": "id8",
      "amount": {
        "currency_code": "currency_code6",
        "value": "value0",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "invoice_id": "invoice_id8",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "status": "CANCELLED",
      "status_details": {
        "reason": "ECHECK",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "id": "id8",
      "amount": {
        "currency_code": "currency_code6",
        "value": "value0",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "invoice_id": "invoice_id8",
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

