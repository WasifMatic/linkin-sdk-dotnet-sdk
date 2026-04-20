
# Cart Information

The cart information.

*This model accepts additional fields of type JsonValue.*

## Structure

`CartInformation`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `ItemDetails` | [`List<ItemDetails>`](../../doc/models/item-details.md) | Optional | An array of item details.<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `32767` |
| `TaxInclusive` | `bool?` | Optional | Indicates whether the item amount or the shipping amount already includes tax.<br><br>**Default**: `false` |
| `PaypalInvoiceId` | `string` | Optional | The ID of the invoice. Appears for only PayPal-generated invoices.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `127`, *Pattern*: `^[a-zA-Z0-9_'\-., ":;\!?]*$` |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "tax_inclusive": false,
  "item_details": [
    {
      "item_code": "item_code0",
      "item_name": "item_name8",
      "item_description": "item_description4",
      "item_options": "item_options2",
      "item_quantity": "item_quantity2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "paypal_invoice_id": "paypal_invoice_id2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

