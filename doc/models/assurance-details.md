
# Assurance Details

Information about cardholder possession validation and cardholder identification and verifications (ID&V).

*This model accepts additional fields of type JsonValue.*

## Structure

`AssuranceDetails`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `AccountVerified` | `bool?` | Optional | If true, indicates that Cardholder possession validation has been performed on returned payment credential.<br><br>**Default**: `false` |
| `CardHolderAuthenticated` | `bool?` | Optional | If true, indicates that identification and verifications (ID&V) was performed on the returned payment credential.If false, the same risk-based authentication can be performed as you would for card transactions. This risk-based authentication can include, but not limited to, step-up with 3D Secure protocol if applicable.<br><br>**Default**: `false` |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "account_verified": false,
  "card_holder_authenticated": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

