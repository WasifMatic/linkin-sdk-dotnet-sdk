
# Card from Request

Representation of card details as received in the request.

*This model accepts additional fields of type JsonValue.*

## Structure

`CardFromRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Expiry` | `string` | Optional | The year and month, in ISO-8601 `YYYY-MM` date format. See [Internet date and time format](https://tools.ietf.org/html/rfc3339#section-5.6).<br><br>**Constraints**: *Minimum Length*: `7`, *Maximum Length*: `7`, *Pattern*: `^[0-9]{4}-(0[1-9]\|1[0-2])$` |
| `LastDigits` | `string` | Optional | The last digits of the payment card.<br><br>**Constraints**: *Minimum Length*: `2`, *Maximum Length*: `4`, *Pattern*: `[0-9]{2,}` |
| `AdditionalProperties` | `JsonValue this[string key]` | Optional | - |

## Example (as JSON)

```json
{
  "expiry": "expiry6",
  "last_digits": "last_digits2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

