# EFCrud.Api.AuthApi

All URIs are relative to *https://localhost:7217*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**ApiAuthLoginPost**](AuthApi.md#apiauthloginpost) | **POST** /api/Auth/login |  |
| [**ApiAuthRegisterPost**](AuthApi.md#apiauthregisterpost) | **POST** /api/Auth/register |  |

<a id="apiauthloginpost"></a>
# **ApiAuthLoginPost**
> User ApiAuthLoginPost (Userdto? userdto = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using EFCrud.Api;
using EFCrud.Client;
using EFCrud.Model;

namespace Example
{
    public class ApiAuthLoginPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://localhost:7217";
            var apiInstance = new AuthApi(config);
            var userdto = new Userdto?(); // Userdto? |  (optional) 

            try
            {
                User result = apiInstance.ApiAuthLoginPost(userdto);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AuthApi.ApiAuthLoginPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiAuthLoginPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<User> response = apiInstance.ApiAuthLoginPostWithHttpInfo(userdto);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AuthApi.ApiAuthLoginPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **userdto** | [**Userdto?**](Userdto?.md) |  | [optional]  |

### Return type

[**User**](User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiauthregisterpost"></a>
# **ApiAuthRegisterPost**
> User ApiAuthRegisterPost (string? role = null, Userdto? userdto = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using EFCrud.Api;
using EFCrud.Client;
using EFCrud.Model;

namespace Example
{
    public class ApiAuthRegisterPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://localhost:7217";
            var apiInstance = new AuthApi(config);
            var role = "role_example";  // string? |  (optional) 
            var userdto = new Userdto?(); // Userdto? |  (optional) 

            try
            {
                User result = apiInstance.ApiAuthRegisterPost(role, userdto);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling AuthApi.ApiAuthRegisterPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiAuthRegisterPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<User> response = apiInstance.ApiAuthRegisterPostWithHttpInfo(role, userdto);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling AuthApi.ApiAuthRegisterPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **role** | **string?** |  | [optional]  |
| **userdto** | [**Userdto?**](Userdto?.md) |  | [optional]  |

### Return type

[**User**](User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

