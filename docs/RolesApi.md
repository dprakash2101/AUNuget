# EFCrud.Api.RolesApi

All URIs are relative to *https://localhost:7217*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**ApiRolesAddEmployeeRolePost**](RolesApi.md#apirolesaddemployeerolepost) | **POST** /api/Roles/Add-EmployeeRole |  |
| [**ApiRolesAddRolesPost**](RolesApi.md#apirolesaddrolespost) | **POST** /api/Roles/Add-roles |  |
| [**ApiRolesDeleteEmpRoleDelete**](RolesApi.md#apirolesdeleteemproledelete) | **DELETE** /api/Roles/Delete-EmpRole |  |
| [**ApiRolesShowEmployeeRolesGet**](RolesApi.md#apirolesshowemployeerolesget) | **GET** /api/Roles/Show-EmployeeRoles |  |
| [**ApiRolesShowRolesGet**](RolesApi.md#apirolesshowrolesget) | **GET** /api/Roles/Show-roles |  |

<a id="apirolesaddemployeerolepost"></a>
# **ApiRolesAddEmployeeRolePost**
> void ApiRolesAddEmployeeRolePost (string? name = null, UserRoles? role = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using EFCrud.Api;
using EFCrud.Client;
using EFCrud.Model;

namespace Example
{
    public class ApiRolesAddEmployeeRolePostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://localhost:7217";
            // Configure API key authorization: oauth2
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new RolesApi(config);
            var name = "name_example";  // string? |  (optional) 
            var role = new UserRoles?(); // UserRoles? |  (optional) 

            try
            {
                apiInstance.ApiRolesAddEmployeeRolePost(name, role);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling RolesApi.ApiRolesAddEmployeeRolePost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiRolesAddEmployeeRolePostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.ApiRolesAddEmployeeRolePostWithHttpInfo(name, role);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling RolesApi.ApiRolesAddEmployeeRolePostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **name** | **string?** |  | [optional]  |
| **role** | [**UserRoles?**](UserRoles?.md) |  | [optional]  |

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

<a id="apirolesaddrolespost"></a>
# **ApiRolesAddRolesPost**
> void ApiRolesAddRolesPost (Roles? roles = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using EFCrud.Api;
using EFCrud.Client;
using EFCrud.Model;

namespace Example
{
    public class ApiRolesAddRolesPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://localhost:7217";
            // Configure API key authorization: oauth2
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new RolesApi(config);
            var roles = new Roles?(); // Roles? |  (optional) 

            try
            {
                apiInstance.ApiRolesAddRolesPost(roles);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling RolesApi.ApiRolesAddRolesPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiRolesAddRolesPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.ApiRolesAddRolesPostWithHttpInfo(roles);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling RolesApi.ApiRolesAddRolesPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **roles** | [**Roles?**](Roles?.md) |  | [optional]  |

### Return type

void (empty response body)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apirolesdeleteemproledelete"></a>
# **ApiRolesDeleteEmpRoleDelete**
> void ApiRolesDeleteEmpRoleDelete (string? name = null, UserRoles? role = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using EFCrud.Api;
using EFCrud.Client;
using EFCrud.Model;

namespace Example
{
    public class ApiRolesDeleteEmpRoleDeleteExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://localhost:7217";
            // Configure API key authorization: oauth2
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new RolesApi(config);
            var name = "name_example";  // string? |  (optional) 
            var role = new UserRoles?(); // UserRoles? |  (optional) 

            try
            {
                apiInstance.ApiRolesDeleteEmpRoleDelete(name, role);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling RolesApi.ApiRolesDeleteEmpRoleDelete: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiRolesDeleteEmpRoleDeleteWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.ApiRolesDeleteEmpRoleDeleteWithHttpInfo(name, role);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling RolesApi.ApiRolesDeleteEmpRoleDeleteWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **name** | **string?** |  | [optional]  |
| **role** | [**UserRoles?**](UserRoles?.md) |  | [optional]  |

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

<a id="apirolesshowemployeerolesget"></a>
# **ApiRolesShowEmployeeRolesGet**
> void ApiRolesShowEmployeeRolesGet ()



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using EFCrud.Api;
using EFCrud.Client;
using EFCrud.Model;

namespace Example
{
    public class ApiRolesShowEmployeeRolesGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://localhost:7217";
            // Configure API key authorization: oauth2
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new RolesApi(config);

            try
            {
                apiInstance.ApiRolesShowEmployeeRolesGet();
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling RolesApi.ApiRolesShowEmployeeRolesGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiRolesShowEmployeeRolesGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.ApiRolesShowEmployeeRolesGetWithHttpInfo();
}
catch (ApiException e)
{
    Debug.Print("Exception when calling RolesApi.ApiRolesShowEmployeeRolesGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters
This endpoint does not need any parameter.
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

<a id="apirolesshowrolesget"></a>
# **ApiRolesShowRolesGet**
> void ApiRolesShowRolesGet ()



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using EFCrud.Api;
using EFCrud.Client;
using EFCrud.Model;

namespace Example
{
    public class ApiRolesShowRolesGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://localhost:7217";
            // Configure API key authorization: oauth2
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new RolesApi(config);

            try
            {
                apiInstance.ApiRolesShowRolesGet();
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling RolesApi.ApiRolesShowRolesGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiRolesShowRolesGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.ApiRolesShowRolesGetWithHttpInfo();
}
catch (ApiException e)
{
    Debug.Print("Exception when calling RolesApi.ApiRolesShowRolesGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters
This endpoint does not need any parameter.
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

