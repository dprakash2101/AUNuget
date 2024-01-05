# EFCrud.FeaturesApi

All URIs are relative to *https://localhost:7217*

Method | HTTP request | Description
------------- | ------------- | -------------
[**api_features_id_delete**](FeaturesApi.md#api_features_id_delete) | **DELETE** /api/Features/{id} | 
[**api_features_id_put**](FeaturesApi.md#api_features_id_put) | **PUT** /api/Features/{id} | 


# **api_features_id_delete**
> api_features_id_delete(id, isdeleted=isdeleted, isactive=isactive)



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
    api_instance = EFCrud.FeaturesApi(api_client)
    id = 56 # int | 
    isdeleted = True # bool |  (optional)
    isactive = True # bool |  (optional)

    try:
        api_instance.api_features_id_delete(id, isdeleted=isdeleted, isactive=isactive)
    except Exception as e:
        print("Exception when calling FeaturesApi->api_features_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 
 **isdeleted** | **bool**|  | [optional] 
 **isactive** | **bool**|  | [optional] 

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

# **api_features_id_put**
> api_features_id_put(id, isman=isman, issup=issup)



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
    api_instance = EFCrud.FeaturesApi(api_client)
    id = 56 # int | 
    isman = True # bool |  (optional)
    issup = True # bool |  (optional)

    try:
        api_instance.api_features_id_put(id, isman=isman, issup=issup)
    except Exception as e:
        print("Exception when calling FeaturesApi->api_features_id_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 
 **isman** | **bool**|  | [optional] 
 **issup** | **bool**|  | [optional] 

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

