
# Activate Subscription Input

Input structure for the method ActivateSubscription

## Structure

`ActivateSubscriptionInput`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Id` | `string` | Required | The ID of the subscription. |
| `ContentType` | `string` | Required, Constant | **Value**: `"application/json"` |
| `Body` | [`ActivateSubscriptionRequest`](../../doc/models/activate-subscription-request.md) | Optional | - |

## Example

```csharp
using PaypalServerSdk.Standard.Models;
using PaypalServerSdk.Standard.Utilities;

ActivateSubscriptionInput activateSubscriptionInput = new ActivateSubscriptionInput
{
    Id = "id0",
    Body = new ActivateSubscriptionRequest
    {
        Reason = "reason8",
        ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
    },
};
```

