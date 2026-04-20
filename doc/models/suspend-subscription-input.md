
# Suspend Subscription Input

Input structure for the method SuspendSubscription

## Structure

`SuspendSubscriptionInput`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Id` | `string` | Required | The ID of the subscription. |
| `ContentType` | `string` | Required, Constant | **Value**: `"application/json"` |
| `Body` | [`SuspendSubscription`](../../doc/models/suspend-subscription.md) | Optional | - |

## Example

```csharp
using PaypalServerSdk.Standard.Models;
using PaypalServerSdk.Standard.Utilities;

SuspendSubscriptionInput suspendSubscriptionInput = new SuspendSubscriptionInput
{
    Id = "id0",
    Body = new SuspendSubscription
    {
        Reason = "reason8",
        ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
    },
};
```

