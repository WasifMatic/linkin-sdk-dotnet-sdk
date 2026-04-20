
# Store Information

The store information.

*This model accepts additional fields of type JsonValue.*

## Structure

`StoreInformation`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `StoreId` | `string` | Optional | The ID of a store for a merchant in the system of record.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `100`, *Pattern*: `^[a-zA-Z0-9]*$` |
| `TerminalId` | `string` | Optional | The terminal ID for the checkout stand in a merchant store.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `60`, *Pattern*: `^[a-zA-Z0-9]*$` |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "store_id": "store_id6",
  "terminal_id": "terminal_id0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

