# EFCrud.Api.EmployeesApi

All URIs are relative to *https://localhost:7217*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**ApiEmployeesGet**](EmployeesApi.md#apiemployeesget) | **GET** /api/Employees |  |
| [**ApiEmployeesIdDelete**](EmployeesApi.md#apiemployeesiddelete) | **DELETE** /api/Employees/{id} |  |
| [**ApiEmployeesIdGet**](EmployeesApi.md#apiemployeesidget) | **GET** /api/Employees/{id} |  |
| [**ApiEmployeesIdPut**](EmployeesApi.md#apiemployeesidput) | **PUT** /api/Employees/{id} |  |
| [**ApiEmployeesPost**](EmployeesApi.md#apiemployeespost) | **POST** /api/Employees |  |

<a id="apiemployeesget"></a>
# **ApiEmployeesGet**
> List&lt;Employee&gt; ApiEmployeesGet (string? name = null, UserRoles? role = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using EFCrud.Api;
using EFCrud.Client;
using EFCrud.Model;

namespace Example
{
    public class ApiEmployeesGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://localhost:7217";
            // Configure API key authorization: oauth2
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new EmployeesApi(config);
            var name = "name_example";  // string? |  (optional) 
            var role = new UserRoles?(); // UserRoles? |  (optional) 

            try
            {
                List<Employee> result = apiInstance.ApiEmployeesGet(name, role);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling EmployeesApi.ApiEmployeesGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiEmployeesGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<List<Employee>> response = apiInstance.ApiEmployeesGetWithHttpInfo(name, role);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling EmployeesApi.ApiEmployeesGetWithHttpInfo: " + e.Message);
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

[**List&lt;Employee&gt;**](Employee.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiemployeesiddelete"></a>
# **ApiEmployeesIdDelete**
> void ApiEmployeesIdDelete (int id)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using EFCrud.Api;
using EFCrud.Client;
using EFCrud.Model;

namespace Example
{
    public class ApiEmployeesIdDeleteExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://localhost:7217";
            // Configure API key authorization: oauth2
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new EmployeesApi(config);
            var id = 56;  // int | 

            try
            {
                apiInstance.ApiEmployeesIdDelete(id);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling EmployeesApi.ApiEmployeesIdDelete: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiEmployeesIdDeleteWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.ApiEmployeesIdDeleteWithHttpInfo(id);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling EmployeesApi.ApiEmployeesIdDeleteWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **int** |  |  |

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

<a id="apiemployeesidget"></a>
# **ApiEmployeesIdGet**
> Employee ApiEmployeesIdGet (int id)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using EFCrud.Api;
using EFCrud.Client;
using EFCrud.Model;

namespace Example
{
    public class ApiEmployeesIdGetExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://localhost:7217";
            // Configure API key authorization: oauth2
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new EmployeesApi(config);
            var id = 56;  // int | 

            try
            {
                Employee result = apiInstance.ApiEmployeesIdGet(id);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling EmployeesApi.ApiEmployeesIdGet: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiEmployeesIdGetWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<Employee> response = apiInstance.ApiEmployeesIdGetWithHttpInfo(id);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling EmployeesApi.ApiEmployeesIdGetWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **int** |  |  |

### Return type

[**Employee**](Employee.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="apiemployeesidput"></a>
# **ApiEmployeesIdPut**
> void ApiEmployeesIdPut (int id, Employee? employee = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using EFCrud.Api;
using EFCrud.Client;
using EFCrud.Model;

namespace Example
{
    public class ApiEmployeesIdPutExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://localhost:7217";
            // Configure API key authorization: oauth2
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new EmployeesApi(config);
            var id = 56;  // int | 
            var employee = new Employee?(); // Employee? |  (optional) 

            try
            {
                apiInstance.ApiEmployeesIdPut(id, employee);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling EmployeesApi.ApiEmployeesIdPut: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiEmployeesIdPutWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    apiInstance.ApiEmployeesIdPutWithHttpInfo(id, employee);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling EmployeesApi.ApiEmployeesIdPutWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **id** | **int** |  |  |
| **employee** | [**Employee?**](Employee?.md) |  | [optional]  |

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

<a id="apiemployeespost"></a>
# **ApiEmployeesPost**
> Employee ApiEmployeesPost (Employee? employee = null)



### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using EFCrud.Api;
using EFCrud.Client;
using EFCrud.Model;

namespace Example
{
    public class ApiEmployeesPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "https://localhost:7217";
            // Configure API key authorization: oauth2
            config.AddApiKey("Authorization", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Authorization", "Bearer");

            var apiInstance = new EmployeesApi(config);
            var employee = new Employee?(); // Employee? |  (optional) 

            try
            {
                Employee result = apiInstance.ApiEmployeesPost(employee);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling EmployeesApi.ApiEmployeesPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the ApiEmployeesPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    ApiResponse<Employee> response = apiInstance.ApiEmployeesPostWithHttpInfo(employee);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling EmployeesApi.ApiEmployeesPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **employee** | [**Employee?**](Employee?.md) |  | [optional]  |

### Return type

[**Employee**](Employee.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

