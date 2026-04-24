# ncsdk.OpenChannelMessagePriorityApi

All requests use the primary/backup domains configured by the caller.

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_open_channel_low_priority_message_type_list**](OpenChannelMessagePriorityApi.md#add_open_channel_low_priority_message_type_list) | **POST** /v4/open-channel/low-priority-message-type-list/add | Add low-priority message types
[**get_open_channel_low_priority_message_type_list**](OpenChannelMessagePriorityApi.md#get_open_channel_low_priority_message_type_list) | **POST** /v4/open-channel/low-priority-message-type-list/get | Query low-priority message types
[**remove_open_channel_low_priority_message_type_list**](OpenChannelMessagePriorityApi.md#remove_open_channel_low_priority_message_type_list) | **POST** /v4/open-channel/low-priority-message-type-list/remove | Remove low-priority message types


# **add_open_channel_low_priority_message_type_list**
> CodeOnlyResponse add_open_channel_low_priority_message_type_list(open_channel_low_priority_message_type_list_request)

Add low-priority message types

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import os
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_low_priority_message_type_list_request import OpenChannelLowPriorityMessageTypeListRequest
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
    api_instance = ncsdk.OpenChannelMessagePriorityApi(api_client)
    
    open_channel_low_priority_message_type_list_request = ncsdk.OpenChannelLowPriorityMessageTypeListRequest() # OpenChannelLowPriorityMessageTypeListRequest | 
    

    try:
        # Add low-priority message types
        api_response = api_instance.add_open_channel_low_priority_message_type_list(open_channel_low_priority_message_type_list_request)
        print("The response of OpenChannelMessagePriorityApi->add_open_channel_low_priority_message_type_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelMessagePriorityApi->add_open_channel_low_priority_message_type_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_low_priority_message_type_list_request** | [**OpenChannelLowPriorityMessageTypeListRequest**](OpenChannelLowPriorityMessageTypeListRequest.md)|  | 


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

# **get_open_channel_low_priority_message_type_list**
> OpenChannelMessageTypeListResponse get_open_channel_low_priority_message_type_list()

Query low-priority message types

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.open_channel_message_type_list_response import OpenChannelMessageTypeListResponse
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
    api_instance = ncsdk.OpenChannelMessagePriorityApi(api_client)
    

    try:
        # Query low-priority message types
        api_response = api_instance.get_open_channel_low_priority_message_type_list()
        print("The response of OpenChannelMessagePriorityApi->get_open_channel_low_priority_message_type_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelMessagePriorityApi->get_open_channel_low_priority_message_type_list: %s\n" % e)
```



### Parameters

This endpoint does not require a request body.

### Return type

[**OpenChannelMessageTypeListResponse**](OpenChannelMessageTypeListResponse.md)

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

# **remove_open_channel_low_priority_message_type_list**
> CodeOnlyResponse remove_open_channel_low_priority_message_type_list(open_channel_low_priority_message_type_list_request)

Remove low-priority message types

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_low_priority_message_type_list_request import OpenChannelLowPriorityMessageTypeListRequest
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
    api_instance = ncsdk.OpenChannelMessagePriorityApi(api_client)
    
    open_channel_low_priority_message_type_list_request = ncsdk.OpenChannelLowPriorityMessageTypeListRequest() # OpenChannelLowPriorityMessageTypeListRequest | 
    

    try:
        # Remove low-priority message types
        api_response = api_instance.remove_open_channel_low_priority_message_type_list(open_channel_low_priority_message_type_list_request)
        print("The response of OpenChannelMessagePriorityApi->remove_open_channel_low_priority_message_type_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelMessagePriorityApi->remove_open_channel_low_priority_message_type_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_low_priority_message_type_list_request** | [**OpenChannelLowPriorityMessageTypeListRequest**](OpenChannelLowPriorityMessageTypeListRequest.md)|  | 


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

