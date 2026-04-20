
# Create Payment Token Input

Input structure for the method CreatePaymentToken

## Structure

`CreatePaymentTokenInput`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `ContentType` | `string` | Required, Constant | **Value**: `"application/json"` |
| `Body` | [`PaymentTokenRequest`](../../doc/models/payment-token-request.md) | Required | Payment Token creation with a financial instrument and an optional customer_id. |
| `PaypalRequestId` | `string` | Optional | The server stores keys for 3 hours.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `108`, *Pattern*: `^.*$` |

## Example

```csharp
using PaypalServerSdk.Standard.Models;
using PaypalServerSdk.Standard.Utilities;

CreatePaymentTokenInput createPaymentTokenInput = new CreatePaymentTokenInput
{
    Body = new PaymentTokenRequest
    {
        PaymentSource = new PaymentTokenRequestPaymentSource
        {
            Card = new PaymentTokenRequestCard
            {
                Name = "name6",
                Number = "number6",
                Expiry = "expiry4",
                SecurityCode = "security_code8",
                Brand = CardBrand.CbNationale,
                ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
            },
            Token = new VaultTokenRequest
            {
                Id = "id6",
                Type = VaultTokenRequestType.SetupToken,
                ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
            },
            ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
        },
        Customer = new Customer
        {
            Id = "id0",
            MerchantCustomerId = "merchant_customer_id2",
            ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
        },
        ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
    },
    PaypalRequestId = "PayPal-Request-Id6",
};
```

