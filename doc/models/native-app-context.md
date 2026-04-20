
# Native App Context

Merchant provided, buyer's native app preferences to app switch to the PayPal consumer app.

*This model accepts additional fields of type JsonValue.*

## Structure

`NativeAppContext`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `OsType` | [`OsType?`](../../doc/models/os-type.md) | Optional | Operating System type of the device that the buyer is using.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `7`, *Pattern*: `^[A-Z_]+$` |
| `OsVersion` | `string` | Optional | Operating System version of the device that the buyer is using.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `64`, *Pattern*: `^.*$` |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "os_type": "ANDROID",
  "os_version": "os_version0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

