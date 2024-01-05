# EFCrud.EmployeesApi

All URIs are relative to *https://localhost:7217*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_employees_get**](EmployeesApi.md#api_employees_get) | **GET** /api/Employees | 
[**api_employees_id_delete**](EmployeesApi.md#api_employees_id_delete) | **DELETE** /api/Employees/{id} | 
[**api_employees_id_get**](EmployeesApi.md#api_employees_id_get) | **GET** /api/Employees/{id} | 
[**api_employees_id_put**](EmployeesApi.md#api_employees_id_put) | **PUT** /api/Employees/{id} | 
[**api_employees_post**](EmployeesApi.md#api_employees_post) | **POST** /api/Employees | 


# **api_employees_get**
> List[Employee] api_employees_get(name=name, role=role)



### Example

* Api Key Authentication (oauth2):

```python
import time
import os
import EFCrud
from EFCrud.models.employee import Employee
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
    api_instance = EFCrud.EmployeesApi(api_client)
    name = 'name_example' # str |  (optional)
    role = EFCrud.UserRoles() # UserRoles |  (optional)

    try:
        api_response = api_instance.api_employees_get(name=name, role=role)
        print("The response of EmployeesApi->api_employees_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmployeesApi->api_employees_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  | [optional] 
 **role** | [**UserRoles**](.md)|  | [optional] 

### Return type

[**List[Employee]**](Employee.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_employees_id_delete**
> api_employees_id_delete(id)



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
    api_instance = EFCrud.EmployeesApi(api_client)
    id = 56 # int | 

    try:
        api_instance.api_employees_id_delete(id)
    except Exception as e:
        print("Exception when calling EmployeesApi->api_employees_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 

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

# **api_employees_id_get**
> Employee api_employees_id_get(id)



### Example

* Api Key Authentication (oauth2):

```python
import time
import os
import EFCrud
from EFCrud.models.employee import Employee
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
    api_instance = EFCrud.EmployeesApi(api_client)
    id = 56 # int | 

    try:
        api_response = api_instance.api_employees_id_get(id)
        print("The response of EmployeesApi->api_employees_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmployeesApi->api_employees_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 

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
**200** | Success |  -  |
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **api_employees_id_put**
> api_employees_id_put(id, employee=employee)



### Example

* Api Key Authentication (oauth2):

```python
import time
import os
import EFCrud
from EFCrud.models.employee import Employee
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
    api_instance = EFCrud.EmployeesApi(api_client)
    id = 56 # int | 
    employee = EFCrud.Employee() # Employee |  (optional)

    try:
        api_instance.api_employees_id_put(id, employee=employee)
    except Exception as e:
        print("Exception when calling EmployeesApi->api_employees_id_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 
 **employee** | [**Employee**](Employee.md)|  | [optional] 

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

# **api_employees_post**
> Employee api_employees_post(employee=employee)



### Example

* Api Key Authentication (oauth2):

```python
import time
import os
import EFCrud
from EFCrud.models.employee import Employee
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
    api_instance = EFCrud.EmployeesApi(api_client)
    employee = EFCrud.Employee() # Employee |  (optional)

    try:
        api_response = api_instance.api_employees_post(employee=employee)
        print("The response of EmployeesApi->api_employees_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmployeesApi->api_employees_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **employee** | [**Employee**](Employee.md)|  | [optional] 

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
**200** | Success |  -  |
**401** | Unauthorized |  -  |
**403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

