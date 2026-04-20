
# Refund Status

The status of the refund.

*This model accepts additional fields of type JsonValue.*

## Enumeration

`RefundStatus`

## Fields

| Name | Description |
|  --- | --- |
| `Cancelled` | The refund was cancelled. |
| `Failed` | The refund could not be processed. |
| `Pending` | The refund is pending. For more information, see status_details.reason. |
| `Completed` | The funds for this transaction were debited to the customer's account. |

