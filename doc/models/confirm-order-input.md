
# Confirm Order Input

Input structure for the method ConfirmOrder

## Structure

`ConfirmOrderInput`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `Id` | `string` | Required | The ID of the order for which the payer confirms their intent to pay.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `36`, *Pattern*: `^[A-Z0-9]+$` |
| `ContentType` | `string` | Required, Constant | **Value**: `"application/json"` |
| `PaypalClientMetadataId` | `string` | Optional | **Constraints**: *Minimum Length*: `1`, *Maximum Length*: `36` |
| `PaypalAuthAssertion` | `string` | Optional | An API-caller-provided JSON Web Token (JWT) assertion that identifies the merchant. For details, see PayPal-Auth-Assertion. |
| `Prefer` | `string` | Optional | The preferred server response upon successful completion of the request. Value is: return=minimal. The server returns a minimal response to optimize communication between the API caller and the server. A minimal response includes the id, status and HATEOAS links. return=representation. The server returns a complete resource representation, including the current state of the resource.<br><br>**Default**: `"return=minimal"`<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `25`, *Pattern*: `^[a-zA-Z=]*$` |
| `Body` | [`ConfirmOrderRequest`](../../doc/models/confirm-order-request.md) | Optional | - |

## Example

```csharp
using PaypalServerSdk.Standard.Models;
using PaypalServerSdk.Standard.Utilities;

ConfirmOrderInput confirmOrderInput = new ConfirmOrderInput
{
    Id = "id0",
    PaypalClientMetadataId = "PayPal-Client-Metadata-Id2",
    PaypalAuthAssertion = "PayPal-Auth-Assertion0",
    Prefer = "return=minimal",
    Body = new ConfirmOrderRequest
    {
        PaymentSource = new PaymentSource
        {
            Card = new CardRequest
            {
                Name = "name6",
                Number = "number6",
                Expiry = "expiry4",
                SecurityCode = "security_code8",
                BillingAddress = new Address
                {
                    CountryCode = "country_code8",
                    AddressLine1 = "address_line_12",
                    AddressLine2 = "address_line_28",
                    AdminArea2 = "admin_area_28",
                    AdminArea1 = "admin_area_14",
                    PostalCode = "postal_code0",
                    ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
                },
                ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
            },
            Token = new Token
            {
                Id = "id6",
                Type = TokenType.BillingAgreement,
                ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
            },
            Paypal = new PaypalWallet
            {
                VaultId = "vault_id0",
                EmailAddress = "email_address0",
                Name = new Name
                {
                    GivenName = "given_name2",
                    Surname = "surname8",
                    ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
                },
                Phone = new PhoneWithType
                {
                    PhoneNumber = new PhoneNumber
                    {
                        NationalNumber = "national_number6",
                        ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
                    },
                    PhoneType = PhoneType.Other,
                    ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
                },
                BirthDate = "birth_date8",
                ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
            },
            Bancontact = new BancontactPaymentRequest
            {
                Name = "name0",
                CountryCode = "country_code0",
                ExperienceContext = new ExperienceContext
                {
                    BrandName = "brand_name2",
                    Locale = "locale6",
                    ShippingPreference = ExperienceContextShippingPreference.NoShipping,
                    ReturnUrl = "return_url4",
                    CancelUrl = "cancel_url6",
                    ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
                },
                ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
            },
            Blik = new BlikPaymentRequest
            {
                Name = "name2",
                CountryCode = "country_code2",
                Email = "email4",
                ExperienceContext = new BlikExperienceContext
                {
                    BrandName = "brand_name2",
                    Locale = "locale6",
                    ShippingPreference = ExperienceContextShippingPreference.NoShipping,
                    ReturnUrl = "return_url4",
                    CancelUrl = "cancel_url6",
                    ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
                },
                Level0 = new BlikLevel0PaymentObject
                {
                    AuthCode = "auth_code8",
                    ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
                },
                OneClick = new BlikOneClickPaymentRequest
                {
                    ConsumerReference = "consumer_reference2",
                    AuthCode = "auth_code0",
                    AliasLabel = "alias_label6",
                    AliasKey = "alias_key4",
                    ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
                },
                ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
            },
            ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
        },
        ApplicationContext = new OrderConfirmApplicationContext
        {
            BrandName = "brand_name8",
            Locale = "locale2",
            ReturnUrl = "return_url0",
            CancelUrl = "cancel_url2",
            StoredPaymentSource = new StoredPaymentSource
            {
                PaymentInitiator = PaymentInitiator.Customer,
                PaymentType = StoredPaymentSourcePaymentType.Recurring,
                Usage = StoredPaymentSourceUsageType.First,
                PreviousNetworkTransactionReference = new NetworkTransaction
                {
                    Id = "id6",
                    Date = "date2",
                    Network = CardBrand.Confidis,
                    AcquirerReferenceNumber = "acquirer_reference_number8",
                    ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
                },
                ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
            },
            ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
        },
        ["exampleAdditionalProperty"] = ApiHelper.JsonDeserialize<JsonValue>("{\"key1\":\"val1\",\"key2\":\"val2\"}"),
    },
};
```

