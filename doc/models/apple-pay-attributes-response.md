
# Apple Pay Attributes Response

Additional attributes associated with the use of Apple Pay.

*This model accepts additional fields of type JsonValue.*

## Structure

`ApplePayAttributesResponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Vault` | [`VaultResponse`](../../doc/models/vault-response.md) | Optional | The details about a saved payment source. |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "vault": {
    "id": "id6",
    "status": "APPROVED",
    "customer": {
      "id": "id0",
      "name": {
        "given_name": "given_name2",
        "surname": "surname8",
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
    "links": [
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
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

