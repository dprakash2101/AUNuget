# EFCrud.RolesApi

All URIs are relative to *https://localhost:7217*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_roles_add_employee_role_post**](RolesApi.md#api_roles_add_employee_role_post) | **POST** /api/Roles/Add-EmployeeRole | 
[**api_roles_add_roles_post**](RolesApi.md#api_roles_add_roles_post) | **POST** /api/Roles/Add-roles | 
[**api_roles_delete_emp_role_delete**](RolesApi.md#api_roles_delete_emp_role_delete) | **DELETE** /api/Roles/Delete-EmpRole | 
[**api_roles_show_employee_roles_get**](RolesApi.md#api_roles_show_employee_roles_get) | **GET** /api/Roles/Show-EmployeeRoles | 
[**api_roles_show_roles_get**](RolesApi.md#api_roles_show_roles_get) | **GET** /api/Roles/Show-roles | 


# **api_roles_add_employee_role_post**
> api_roles_add_employee_role_post(name=name, role=role)



### Example

* Api Key Authentication (oauth2):

```python
import time
import os
import EFCrud
from EFCrud.models.user_roles import UserRoles
from EFCrud.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://localhost:7217
# See configuration.py for a list of all supported configuration parameters.
configuration = EFCrud.Configuration(
    host = "https://localhost:7217"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: oauth2
configuration.api_key['oauth2'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['oauth2'] = 'Bearer'

# Enter a context with an instance of the API client
with EFCrud.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = EFCrud.RolesApi(api_client)
    name = 'name_example' # str |  (optional)
    role = EFCrud.UserRoles() # UserRoles |  (optional)

    try:
        api_instance.api_roles_add_employee_role_post(name=name, role=role)
    except Exception as e:
        print("Exception when calling RolesApi->api_roles_add_employee_role_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | [optional] 
 **role** | [**UserRoles**](.md)|  | [optional] 

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
**200** | Success |  -  |
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_roles_add_roles_post**
> api_roles_add_roles_post(roles=roles)



### Example

* Api Key Authentication (oauth2):

```python
import time
import os
import EFCrud
from EFCrud.models.roles import Roles
from EFCrud.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://localhost:7217
# See configuration.py for a list of all supported configuration parameters.
configuration = EFCrud.Configuration(
    host = "https://localhost:7217"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: oauth2
configuration.api_key['oauth2'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['oauth2'] = 'Bearer'

# Enter a context with an instance of the API client
with EFCrud.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = EFCrud.RolesApi(api_client)
    roles = EFCrud.Roles() # Roles |  (optional)

    try:
        api_instance.api_roles_add_roles_post(roles=roles)
    except Exception as e:
        print("Exception when calling RolesApi->api_roles_add_roles_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **roles** | [**Roles**](Roles.md)|  | [optional] 

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
**200** | Success |  -  |
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_roles_delete_emp_role_delete**
> api_roles_delete_emp_role_delete(name=name, role=role)



### Example

* Api Key Authentication (oauth2):

```python
import time
import os
import EFCrud
from EFCrud.models.user_roles import UserRoles
from EFCrud.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://localhost:7217
# See configuration.py for a list of all supported configuration parameters.
configuration = EFCrud.Configuration(
    host = "https://localhost:7217"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: oauth2
configuration.api_key['oauth2'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['oauth2'] = 'Bearer'

# Enter a context with an instance of the API client
with EFCrud.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = EFCrud.RolesApi(api_client)
    name = 'name_example' # str |  (optional)
    role = EFCrud.UserRoles() # UserRoles |  (optional)

    try:
        api_instance.api_roles_delete_emp_role_delete(name=name, role=role)
    except Exception as e:
        print("Exception when calling RolesApi->api_roles_delete_emp_role_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | [optional] 
 **role** | [**UserRoles**](.md)|  | [optional] 

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
**200** | Success |  -  |
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_roles_show_employee_roles_get**
> api_roles_show_employee_roles_get()



### Example

* Api Key Authentication (oauth2):

```python
import time
import os
import EFCrud
from EFCrud.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://localhost:7217
# See configuration.py for a list of all supported configuration parameters.
configuration = EFCrud.Configuration(
    host = "https://localhost:7217"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: oauth2
configuration.api_key['oauth2'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['oauth2'] = 'Bearer'

# Enter a context with an instance of the API client
with EFCrud.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = EFCrud.RolesApi(api_client)

    try:
        api_instance.api_roles_show_employee_roles_get()
    except Exception as e:
        print("Exception when calling RolesApi->api_roles_show_employee_roles_get: %s\n" % e)
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
**200** | Success |  -  |
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_roles_show_roles_get**
> api_roles_show_roles_get()



### Example

* Api Key Authentication (oauth2):

```python
import time
import os
import EFCrud
from EFCrud.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://localhost:7217
# See configuration.py for a list of all supported configuration parameters.
configuration = EFCrud.Configuration(
    host = "https://localhost:7217"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: oauth2
configuration.api_key['oauth2'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['oauth2'] = 'Bearer'

# Enter a context with an instance of the API client
with EFCrud.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = EFCrud.RolesApi(api_client)

    try:
        api_instance.api_roles_show_roles_get()
    except Exception as e:
        print("Exception when calling RolesApi->api_roles_show_roles_get: %s\n" % e)
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
**200** | Success |  -  |
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

