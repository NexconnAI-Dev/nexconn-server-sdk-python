# ncsdk.UserBlocklistApi

All requests use the primary/backup domains configured by the caller.

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_user_blocklist**](UserBlocklistApi.md#add_user_blocklist) | **POST** /v4/user/blocklist/add | Add to blocklist
[**get_user_blocklist**](UserBlocklistApi.md#get_user_blocklist) | **POST** /v4/user/blocklist/get | Get blocklist
[**remove_user_blocklist**](UserBlocklistApi.md#remove_user_blocklist) | **POST** /v4/user/blocklist/remove | Remove from blocklist


# **add_user_blocklist**
> CodeOnlyResponse add_user_blocklist(user_blocklist_add_request)

Add to blocklist

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import os
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.user_blocklist_add_request import UserBlocklistAddRequest
from ncsdk.rest import ApiException
from pprint import pprint

# Configure primary/backup domains before sending requests.
# See configuration.py for a list of all supported configuration parameters.
configuration = ncsdk.Configuration()

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: NexconnSignature
configuration.api_key['NexconnSignature'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['NexconnSignature'] = 'Bearer'

# Enter a context with an instance of the API client
with ncsdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ncsdk.UserBlocklistApi(api_client)
    
    user_blocklist_add_request = ncsdk.UserBlocklistAddRequest() # UserBlocklistAddRequest | 
    

    try:
        # Add to blocklist
        api_response = api_instance.add_user_blocklist(user_blocklist_add_request)
        print("The response of UserBlocklistApi->add_user_blocklist:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserBlocklistApi->add_user_blocklist: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_blocklist_add_request** | [**UserBlocklistAddRequest**](UserBlocklistAddRequest.md)|  | 


### Return type

[**CodeOnlyResponse**](CodeOnlyResponse.md)

### Authorization

[NexconnSignature](../README.md#NexconnSignature)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_user_blocklist**
> UserBlocklistGetResponse get_user_blocklist(user_blocklist_get_request)

Get blocklist

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.user_blocklist_get_request import UserBlocklistGetRequest
from ncsdk.models.user_blocklist_get_response import UserBlocklistGetResponse
from ncsdk.rest import ApiException
from pprint import pprint

# Configure primary/backup domains before sending requests.
# See configuration.py for a list of all supported configuration parameters.
configuration = ncsdk.Configuration()

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: NexconnSignature
configuration.api_key['NexconnSignature'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['NexconnSignature'] = 'Bearer'

# Enter a context with an instance of the API client
with ncsdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ncsdk.UserBlocklistApi(api_client)
    
    user_blocklist_get_request = ncsdk.UserBlocklistGetRequest() # UserBlocklistGetRequest | 
    

    try:
        # Get blocklist
        api_response = api_instance.get_user_blocklist(user_blocklist_get_request)
        print("The response of UserBlocklistApi->get_user_blocklist:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserBlocklistApi->get_user_blocklist: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_blocklist_get_request** | [**UserBlocklistGetRequest**](UserBlocklistGetRequest.md)|  | 


### Return type

[**UserBlocklistGetResponse**](UserBlocklistGetResponse.md)

### Authorization

[NexconnSignature](../README.md#NexconnSignature)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **remove_user_blocklist**
> CodeOnlyResponse remove_user_blocklist(user_blocklist_remove_request)

Remove from blocklist

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.user_blocklist_remove_request import UserBlocklistRemoveRequest
from ncsdk.rest import ApiException
from pprint import pprint

# Configure primary/backup domains before sending requests.
# See configuration.py for a list of all supported configuration parameters.
configuration = ncsdk.Configuration()

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: NexconnSignature
configuration.api_key['NexconnSignature'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['NexconnSignature'] = 'Bearer'

# Enter a context with an instance of the API client
with ncsdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ncsdk.UserBlocklistApi(api_client)
    
    user_blocklist_remove_request = ncsdk.UserBlocklistRemoveRequest() # UserBlocklistRemoveRequest | 
    

    try:
        # Remove from blocklist
        api_response = api_instance.remove_user_blocklist(user_blocklist_remove_request)
        print("The response of UserBlocklistApi->remove_user_blocklist:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserBlocklistApi->remove_user_blocklist: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_blocklist_remove_request** | [**UserBlocklistRemoveRequest**](UserBlocklistRemoveRequest.md)|  | 


### Return type

[**CodeOnlyResponse**](CodeOnlyResponse.md)

### Authorization

[NexconnSignature](../README.md#NexconnSignature)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

