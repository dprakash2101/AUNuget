# EFCrud.Api.FeaturesApi

All URIs are relative to *https://localhost:7217*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**ApiFeaturesIdDelete**](FeaturesApi.md#apifeaturesiddelete) | **DELETE** /api/Features/{id} |  |
| [**ApiFeaturesIdPut**](FeaturesApi.md#apifeaturesidput) | **PUT** /api/Features/{id} |  |

<a id="apifeaturesiddelete"></a>
# **ApiFeaturesIdDelete**
> void ApiFeaturesIdDelete (int id, bool? isdeleted = null, bool? isactive = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using EFCrud.Api;
using EFCrud.Client;
using EFCrud.Model;

namespace Example
{
    public class ApiFeaturesIdDeleteExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://localhost:7217";
            // Configure API key authorization: oauth2
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new FeaturesApi(config);
            var id = 56;  // int | 
            var isdeleted = true;  // bool? |  (optional) 
            var isactive = true;  // bool? |  (optional) 

            try
            {
                apiInstance.ApiFeaturesIdDelete(id, isdeleted, isactive);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling FeaturesApi.ApiFeaturesIdDelete: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiFeaturesIdDeleteWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.ApiFeaturesIdDeleteWithHttpInfo(id, isdeleted, isactive);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling FeaturesApi.ApiFeaturesIdDeleteWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **int** |  |  |
| **isdeleted** | **bool?** |  | [optional]  |
| **isactive** | **bool?** |  | [optional]  |

### Return type

void (empty response body)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apifeaturesidput"></a>
# **ApiFeaturesIdPut**
> void ApiFeaturesIdPut (int id, bool? isman = null, bool? issup = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using EFCrud.Api;
using EFCrud.Client;
using EFCrud.Model;

namespace Example
{
    public class ApiFeaturesIdPutExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://localhost:7217";
            // Configure API key authorization: oauth2
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new FeaturesApi(config);
            var id = 56;  // int | 
            var isman = true;  // bool? |  (optional) 
            var issup = true;  // bool? |  (optional) 

            try
            {
                apiInstance.ApiFeaturesIdPut(id, isman, issup);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling FeaturesApi.ApiFeaturesIdPut: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiFeaturesIdPutWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.ApiFeaturesIdPutWithHttpInfo(id, isman, issup);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling FeaturesApi.ApiFeaturesIdPutWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **int** |  |  |
| **isman** | **bool?** |  | [optional]  |
| **issup** | **bool?** |  | [optional]  |

### Return type

void (empty response body)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

