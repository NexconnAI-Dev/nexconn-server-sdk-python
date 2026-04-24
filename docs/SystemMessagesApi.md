# ncsdk.SystemMessagesApi

All requests use the primary/backup domains configured by the caller.

Method | HTTP request | Description
------------- | ------------- | -------------
[**broadcast_message_online**](SystemMessagesApi.md#broadcast_message_online) | **POST** /v4/system-channel/message/broadcast-online | Broadcast to online users
[**broadcast_system_channel_message**](SystemMessagesApi.md#broadcast_system_channel_message) | **POST** /v4/system-channel/message/broadcast-all | Broadcast to all users (persistent)
[**delete_broadcast_message**](SystemMessagesApi.md#delete_broadcast_message) | **POST** /v4/system-channel/message/broadcast/delete | Recall broadcast to all users
[**send_system_channel_message**](SystemMessagesApi.md#send_system_channel_message) | **POST** /v4/system-channel/message/send | Send a system message
[**send_system_channel_push_by_package**](SystemMessagesApi.md#send_system_channel_push_by_package) | **POST** /v4/system-channel/app-package-users/send | Push by app package name
[**send_system_channel_push_by_tag**](SystemMessagesApi.md#send_system_channel_push_by_tag) | **POST** /v4/system-channel/tagged-users/send | Push to tagged users


# **broadcast_message_online**
> SingleMessageIdResponse broadcast_message_online(system_channel_broadcast_online_request)

Broadcast to online users

Rate limit: 60/min.

### Example

* Api Key Authentication (NexconnSignature):

```python
import os
import ncsdk
from ncsdk.models.single_message_id_response import SingleMessageIdResponse
from ncsdk.models.system_channel_broadcast_online_request import SystemChannelBroadcastOnlineRequest
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
    api_instance = ncsdk.SystemMessagesApi(api_client)
    
    system_channel_broadcast_online_request = ncsdk.SystemChannelBroadcastOnlineRequest() # SystemChannelBroadcastOnlineRequest | 
    

    try:
        # Broadcast to online users
        api_response = api_instance.broadcast_message_online(system_channel_broadcast_online_request)
        print("The response of SystemMessagesApi->broadcast_message_online:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SystemMessagesApi->broadcast_message_online: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **system_channel_broadcast_online_request** | [**SystemChannelBroadcastOnlineRequest**](SystemChannelBroadcastOnlineRequest.md)|  | 


### Return type

[**SingleMessageIdResponse**](SingleMessageIdResponse.md)

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

# **broadcast_system_channel_message**
> SingleMessageIdResponse broadcast_system_channel_message(system_channel_broadcast_all_request)

Broadcast to all users (persistent)

Rate limit: 2/hour, 3/day.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.single_message_id_response import SingleMessageIdResponse
from ncsdk.models.system_channel_broadcast_all_request import SystemChannelBroadcastAllRequest
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
    api_instance = ncsdk.SystemMessagesApi(api_client)
    
    system_channel_broadcast_all_request = ncsdk.SystemChannelBroadcastAllRequest() # SystemChannelBroadcastAllRequest | 
    

    try:
        # Broadcast to all users (persistent)
        api_response = api_instance.broadcast_system_channel_message(system_channel_broadcast_all_request)
        print("The response of SystemMessagesApi->broadcast_system_channel_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SystemMessagesApi->broadcast_system_channel_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **system_channel_broadcast_all_request** | [**SystemChannelBroadcastAllRequest**](SystemChannelBroadcastAllRequest.md)|  | 


### Return type

[**SingleMessageIdResponse**](SingleMessageIdResponse.md)

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

# **delete_broadcast_message**
> CodeOnlyResponse delete_broadcast_message(system_channel_broadcast_delete_request)

Recall broadcast to all users

Rate limit: 2/hour, 3/day.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.system_channel_broadcast_delete_request import SystemChannelBroadcastDeleteRequest
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
    api_instance = ncsdk.SystemMessagesApi(api_client)
    
    system_channel_broadcast_delete_request = ncsdk.SystemChannelBroadcastDeleteRequest() # SystemChannelBroadcastDeleteRequest | 
    

    try:
        # Recall broadcast to all users
        api_response = api_instance.delete_broadcast_message(system_channel_broadcast_delete_request)
        print("The response of SystemMessagesApi->delete_broadcast_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SystemMessagesApi->delete_broadcast_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **system_channel_broadcast_delete_request** | [**SystemChannelBroadcastDeleteRequest**](SystemChannelBroadcastDeleteRequest.md)|  | 


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

# **send_system_channel_message**
> UserMessageSendResponse send_system_channel_message(system_channel_message_send_request)

Send a system message

Rate limit: 100 msgs/sec (by recipient count).

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.system_channel_message_send_request import SystemChannelMessageSendRequest
from ncsdk.models.user_message_send_response import UserMessageSendResponse
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
    api_instance = ncsdk.SystemMessagesApi(api_client)
    
    system_channel_message_send_request = ncsdk.SystemChannelMessageSendRequest() # SystemChannelMessageSendRequest | 
    

    try:
        # Send a system message
        api_response = api_instance.send_system_channel_message(system_channel_message_send_request)
        print("The response of SystemMessagesApi->send_system_channel_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SystemMessagesApi->send_system_channel_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **system_channel_message_send_request** | [**SystemChannelMessageSendRequest**](SystemChannelMessageSendRequest.md)|  | 


### Return type

[**UserMessageSendResponse**](UserMessageSendResponse.md)

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

# **send_system_channel_push_by_package**
> SystemChannelPushResponse send_system_channel_push_by_package(system_channel_push_request)

Push by app package name

Rate limit: 2/hour, 3/day (shared).

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.system_channel_push_request import SystemChannelPushRequest
from ncsdk.models.system_channel_push_response import SystemChannelPushResponse
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
    api_instance = ncsdk.SystemMessagesApi(api_client)
    
    system_channel_push_request = ncsdk.SystemChannelPushRequest() # SystemChannelPushRequest | 
    

    try:
        # Push by app package name
        api_response = api_instance.send_system_channel_push_by_package(system_channel_push_request)
        print("The response of SystemMessagesApi->send_system_channel_push_by_package:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SystemMessagesApi->send_system_channel_push_by_package: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **system_channel_push_request** | [**SystemChannelPushRequest**](SystemChannelPushRequest.md)|  | 


### Return type

[**SystemChannelPushResponse**](SystemChannelPushResponse.md)

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

# **send_system_channel_push_by_tag**
> SystemChannelPushResponse send_system_channel_push_by_tag(system_channel_push_request)

Push to tagged users

Rate limit: 2/hour, 3/day (shared).

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.system_channel_push_request import SystemChannelPushRequest
from ncsdk.models.system_channel_push_response import SystemChannelPushResponse
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
    api_instance = ncsdk.SystemMessagesApi(api_client)
    
    system_channel_push_request = ncsdk.SystemChannelPushRequest() # SystemChannelPushRequest | 
    

    try:
        # Push to tagged users
        api_response = api_instance.send_system_channel_push_by_tag(system_channel_push_request)
        print("The response of SystemMessagesApi->send_system_channel_push_by_tag:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SystemMessagesApi->send_system_channel_push_by_tag: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **system_channel_push_request** | [**SystemChannelPushRequest**](SystemChannelPushRequest.md)|  | 


### Return type

[**SystemChannelPushResponse**](SystemChannelPushResponse.md)

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

