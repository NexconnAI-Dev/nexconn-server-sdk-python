# ncsdk.OpenChannelManagementApi

All requests use the primary/backup domains configured by the caller.

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_open_channel**](OpenChannelManagementApi.md#create_open_channel) | **POST** /v4/open-channel/create | Create an open channel
[**destroy_open_channels**](OpenChannelManagementApi.md#destroy_open_channels) | **POST** /v4/open-channel/destroy | Destroy an open channel
[**get_open_channel**](OpenChannelManagementApi.md#get_open_channel) | **POST** /v4/open-channel/get | Get open channel info
[**set_open_channel_destroy_type**](OpenChannelManagementApi.md#set_open_channel_destroy_type) | **POST** /v4/open-channel/destroy-type/set | Set auto-destroy type


# **create_open_channel**
> CodeOnlyResponse create_open_channel(open_channel_create_request)

Create an open channel

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import os
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_create_request import OpenChannelCreateRequest
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
    api_instance = ncsdk.OpenChannelManagementApi(api_client)
    
    open_channel_create_request = ncsdk.OpenChannelCreateRequest() # OpenChannelCreateRequest | 
    

    try:
        # Create an open channel
        api_response = api_instance.create_open_channel(open_channel_create_request)
        print("The response of OpenChannelManagementApi->create_open_channel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelManagementApi->create_open_channel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_create_request** | [**OpenChannelCreateRequest**](OpenChannelCreateRequest.md)|  | 


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

# **destroy_open_channels**
> CodeOnlyResponse destroy_open_channels(open_channel_destroy_request)

Destroy an open channel

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_destroy_request import OpenChannelDestroyRequest
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
    api_instance = ncsdk.OpenChannelManagementApi(api_client)
    
    open_channel_destroy_request = ncsdk.OpenChannelDestroyRequest() # OpenChannelDestroyRequest | 
    

    try:
        # Destroy an open channel
        api_response = api_instance.destroy_open_channels(open_channel_destroy_request)
        print("The response of OpenChannelManagementApi->destroy_open_channels:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelManagementApi->destroy_open_channels: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_destroy_request** | [**OpenChannelDestroyRequest**](OpenChannelDestroyRequest.md)|  | 


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

# **get_open_channel**
> OpenChannelGetResponse get_open_channel(open_channel_get_request)

Get open channel info

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.open_channel_get_request import OpenChannelGetRequest
from ncsdk.models.open_channel_get_response import OpenChannelGetResponse
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
    api_instance = ncsdk.OpenChannelManagementApi(api_client)
    
    open_channel_get_request = ncsdk.OpenChannelGetRequest() # OpenChannelGetRequest | 
    

    try:
        # Get open channel info
        api_response = api_instance.get_open_channel(open_channel_get_request)
        print("The response of OpenChannelManagementApi->get_open_channel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelManagementApi->get_open_channel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_get_request** | [**OpenChannelGetRequest**](OpenChannelGetRequest.md)|  | 


### Return type

[**OpenChannelGetResponse**](OpenChannelGetResponse.md)

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

# **set_open_channel_destroy_type**
> CodeOnlyResponse set_open_channel_destroy_type(open_channel_destroy_type_set_request)

Set auto-destroy type

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_destroy_type_set_request import OpenChannelDestroyTypeSetRequest
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
    api_instance = ncsdk.OpenChannelManagementApi(api_client)
    
    open_channel_destroy_type_set_request = ncsdk.OpenChannelDestroyTypeSetRequest() # OpenChannelDestroyTypeSetRequest | 
    

    try:
        # Set auto-destroy type
        api_response = api_instance.set_open_channel_destroy_type(open_channel_destroy_type_set_request)
        print("The response of OpenChannelManagementApi->set_open_channel_destroy_type:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelManagementApi->set_open_channel_destroy_type: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_destroy_type_set_request** | [**OpenChannelDestroyTypeSetRequest**](OpenChannelDestroyTypeSetRequest.md)|  | 


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

