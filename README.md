# Global LEI & Corporate Tax ID Validator API — .NET / C# Client

[![NuGet version](https://img.shields.io/nuget/v/RapidApi.LeiValidatorClient.svg)](https://www.nuget.org/packages/RapidApi.LeiValidatorClient/)
[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/57865358-8bafe64c-1441-4fe3-ba7a-2d60bdeb7dc5)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![RapidAPI Listing](https://img.shields.io/badge/RapidAPI-Dedicated%20Listing-blueviolet)](https://rapidapi.com/noor-mkdad-apis-noor-mkdad-apis-default/api/global-lei-corporate-tax-id-validator-api)

Official zero-dependency .NET / C# client for **Global LEI & Corporate Tax ID Validator API**.

> Sub-5ms edge validation for ISO 17442 LEI (MOD 97-10), US EIN (IRS Campuses), Australian ABN/ACN (MOD-89), and UK Companies House CRN.

> 🔑 **Get your Dedicated API Key:** [Subscribe to Global LEI & Corporate Tax ID Validator API on RapidAPI](https://rapidapi.com/noor-mkdad-apis-noor-mkdad-apis-default/api/global-lei-corporate-tax-id-validator-api)

---

## 🚀 Installation

```bash
dotnet add package RapidApi.LeiValidatorClient
```

---

## ⚡ Quickstart

```csharp
using System;
using System.Threading.Tasks;
using RapidApi.LeiValidator;

class Program
{
    static async Task Main()
    {
        using var client = new LeiValidatorClient(new RapidApiConfig
        {
            ApiKey = "YOUR_RAPIDAPI_KEY" // Get key from https://rapidapi.com/noor-mkdad-apis-noor-mkdad-apis-default/api/global-lei-corporate-tax-id-validator-api
        });

        var result = await client.ValidateAsync(new
        {
            // Enter validation payload
        });

        Console.WriteLine($"Success: {result.Success}");
    }
}
```

---

## 🔗 Links
- 📖 [RapidAPI Documentation & Key](https://rapidapi.com/noor-mkdad-apis-noor-mkdad-apis-default/api/global-lei-corporate-tax-id-validator-api)

## 📄 License
MIT © Noor Mkdad
