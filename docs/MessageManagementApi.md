# ncsdk.MessageManagementApi

All requests use the primary/backup domains configured by the caller.

Method | HTTP request | Description
------------- | ------------- | -------------
[**broadcast_open_channel_message**](MessageManagementApi.md#broadcast_open_channel_message) | **POST** /v4/open-channel/message/broadcast | Broadcast to all open channels
[**delete_channel_message_history**](MessageManagementApi.md#delete_channel_message_history) | **POST** /v4/channel/message/history/delete | Delete server-side channel message history
[**delete_channel_type_message_metadata**](MessageManagementApi.md#delete_channel_type_message_metadata) | **POST** /v4/channel-type/message/metadata/delete | Delete message metadata
[**delete_community_channel_message_metadata**](MessageManagementApi.md#delete_community_channel_message_metadata) | **POST** /v4/community-channel/message/metadata/delete | Delete community-channel message metadata keys
[**delete_message**](MessageManagementApi.md#delete_message) | **POST** /v4/message/delete | Delete a message (recall)
[**list_channel_type_message_metadata**](MessageManagementApi.md#list_channel_type_message_metadata) | **POST** /v4/channel-type/message/metadata/list | Get message metadata
[**list_community_channel_message_metadata**](MessageManagementApi.md#list_community_channel_message_metadata) | **POST** /v4/community-channel/message/metadata/list | List community-channel message metadata
[**send_community_channel_message**](MessageManagementApi.md#send_community_channel_message) | **POST** /v4/community-channel/message/send | Send a community channel message
[**send_direct_channel_message**](MessageManagementApi.md#send_direct_channel_message) | **POST** /v4/direct-channel/message/send | Send a direct message
[**send_direct_channel_stream_message**](MessageManagementApi.md#send_direct_channel_stream_message) | **POST** /v4/direct-channel/message/stream/send | Send a direct channel stream message
[**send_group_channel_message**](MessageManagementApi.md#send_group_channel_message) | **POST** /v4/group-channel/message/send | Send a group message
[**send_group_channel_stream_message**](MessageManagementApi.md#send_group_channel_stream_message) | **POST** /v4/group-channel/message/stream/send | Send a group channel stream message
[**send_open_channel_message**](MessageManagementApi.md#send_open_channel_message) | **POST** /v4/open-channel/message/send | Send an open channel message
[**set_channel_type_message_metadata**](MessageManagementApi.md#set_channel_type_message_metadata) | **POST** /v4/channel-type/message/metadata/set | Set message metadata
[**set_community_channel_message_metadata**](MessageManagementApi.md#set_community_channel_message_metadata) | **POST** /v4/community-channel/message/metadata/set | Set community-channel message metadata
[**update_community_channel_message**](MessageManagementApi.md#update_community_channel_message) | **POST** /v4/community-channel/message/update | Update community-channel message
[**update_direct_channel_message**](MessageManagementApi.md#update_direct_channel_message) | **POST** /v4/direct-channel/message/update | Update direct-channel message
[**update_group_channel_message**](MessageManagementApi.md#update_group_channel_message) | **POST** /v4/group-channel/message/update | Update group-channel message


# **broadcast_open_channel_message**
> CodeOnlyResponse broadcast_open_channel_message(open_channel_broadcast_request)

Broadcast to all open channels

Rate limit: 1/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import os
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_broadcast_request import OpenChannelBroadcastRequest
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    open_channel_broadcast_request = ncsdk.OpenChannelBroadcastRequest() # OpenChannelBroadcastRequest | 
    

    try:
        # Broadcast to all open channels
        api_response = api_instance.broadcast_open_channel_message(open_channel_broadcast_request)
        print("The response of MessageManagementApi->broadcast_open_channel_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->broadcast_open_channel_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_broadcast_request** | [**OpenChannelBroadcastRequest**](OpenChannelBroadcastRequest.md)|  | 


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

# **delete_channel_message_history**
> CodeOnlyResponse delete_channel_message_history(channel_message_history_delete_request)

Delete server-side channel message history

Rate limit: 100/sec. Server path `/v4/channel/message/history/delete` (`HistoryCleanInput`).

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.channel_message_history_delete_request import ChannelMessageHistoryDeleteRequest
from ncsdk.models.code_only_response import CodeOnlyResponse
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    channel_message_history_delete_request = ncsdk.ChannelMessageHistoryDeleteRequest() # ChannelMessageHistoryDeleteRequest | 
    

    try:
        # Delete server-side channel message history
        api_response = api_instance.delete_channel_message_history(channel_message_history_delete_request)
        print("The response of MessageManagementApi->delete_channel_message_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->delete_channel_message_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channel_message_history_delete_request** | [**ChannelMessageHistoryDeleteRequest**](ChannelMessageHistoryDeleteRequest.md)|  | 


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

# **delete_channel_type_message_metadata**
> CodeOnlyResponse delete_channel_type_message_metadata(channel_type_message_metadata_delete_request)

Delete message metadata

Rate limit: 100/sec (max 20 for group messages).

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.channel_type_message_metadata_delete_request import ChannelTypeMessageMetadataDeleteRequest
from ncsdk.models.code_only_response import CodeOnlyResponse
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    channel_type_message_metadata_delete_request = ncsdk.ChannelTypeMessageMetadataDeleteRequest() # ChannelTypeMessageMetadataDeleteRequest | 
    

    try:
        # Delete message metadata
        api_response = api_instance.delete_channel_type_message_metadata(channel_type_message_metadata_delete_request)
        print("The response of MessageManagementApi->delete_channel_type_message_metadata:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->delete_channel_type_message_metadata: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channel_type_message_metadata_delete_request** | [**ChannelTypeMessageMetadataDeleteRequest**](ChannelTypeMessageMetadataDeleteRequest.md)|  | 


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

# **delete_community_channel_message_metadata**
> CodeOnlyResponse delete_community_channel_message_metadata(community_channel_message_metadata_delete_request)

Delete community-channel message metadata keys

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_message_metadata_delete_request import CommunityChannelMessageMetadataDeleteRequest
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    community_channel_message_metadata_delete_request = ncsdk.CommunityChannelMessageMetadataDeleteRequest() # CommunityChannelMessageMetadataDeleteRequest | 
    

    try:
        # Delete community-channel message metadata keys
        api_response = api_instance.delete_community_channel_message_metadata(community_channel_message_metadata_delete_request)
        print("The response of MessageManagementApi->delete_community_channel_message_metadata:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->delete_community_channel_message_metadata: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_message_metadata_delete_request** | [**CommunityChannelMessageMetadataDeleteRequest**](CommunityChannelMessageMetadataDeleteRequest.md)|  | 


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

# **delete_message**
> CodeOnlyResponse delete_message(message_delete_request)

Delete a message (recall)

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.message_delete_request import MessageDeleteRequest
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    message_delete_request = ncsdk.MessageDeleteRequest() # MessageDeleteRequest | 
    

    try:
        # Delete a message (recall)
        api_response = api_instance.delete_message(message_delete_request)
        print("The response of MessageManagementApi->delete_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->delete_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_delete_request** | [**MessageDeleteRequest**](MessageDeleteRequest.md)|  | 


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

# **list_channel_type_message_metadata**
> ChannelTypeMessageMetadataListResponse list_channel_type_message_metadata(channel_type_message_metadata_list_request)

Get message metadata

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.channel_type_message_metadata_list_request import ChannelTypeMessageMetadataListRequest
from ncsdk.models.channel_type_message_metadata_list_response import ChannelTypeMessageMetadataListResponse
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    channel_type_message_metadata_list_request = ncsdk.ChannelTypeMessageMetadataListRequest() # ChannelTypeMessageMetadataListRequest | 
    

    try:
        # Get message metadata
        api_response = api_instance.list_channel_type_message_metadata(channel_type_message_metadata_list_request)
        print("The response of MessageManagementApi->list_channel_type_message_metadata:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->list_channel_type_message_metadata: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channel_type_message_metadata_list_request** | [**ChannelTypeMessageMetadataListRequest**](ChannelTypeMessageMetadataListRequest.md)|  | 


### Return type

[**ChannelTypeMessageMetadataListResponse**](ChannelTypeMessageMetadataListResponse.md)

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

# **list_community_channel_message_metadata**
> CommunityChannelMessageMetadataListResponse list_community_channel_message_metadata(community_channel_message_metadata_list_request)

List community-channel message metadata

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.community_channel_message_metadata_list_request import CommunityChannelMessageMetadataListRequest
from ncsdk.models.community_channel_message_metadata_list_response import CommunityChannelMessageMetadataListResponse
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    community_channel_message_metadata_list_request = ncsdk.CommunityChannelMessageMetadataListRequest() # CommunityChannelMessageMetadataListRequest | 
    

    try:
        # List community-channel message metadata
        api_response = api_instance.list_community_channel_message_metadata(community_channel_message_metadata_list_request)
        print("The response of MessageManagementApi->list_community_channel_message_metadata:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->list_community_channel_message_metadata: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_message_metadata_list_request** | [**CommunityChannelMessageMetadataListRequest**](CommunityChannelMessageMetadataListRequest.md)|  | 


### Return type

[**CommunityChannelMessageMetadataListResponse**](CommunityChannelMessageMetadataListResponse.md)

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

# **send_community_channel_message**
> ChannelMessageSendResponse send_community_channel_message(community_channel_message_send_request)

Send a community channel message

Rate limit: 100/sec (by target group count); 20/sec per channel.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.channel_message_send_response import ChannelMessageSendResponse
from ncsdk.models.community_channel_message_send_request import CommunityChannelMessageSendRequest
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    community_channel_message_send_request = ncsdk.CommunityChannelMessageSendRequest() # CommunityChannelMessageSendRequest | 
    

    try:
        # Send a community channel message
        api_response = api_instance.send_community_channel_message(community_channel_message_send_request)
        print("The response of MessageManagementApi->send_community_channel_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->send_community_channel_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_message_send_request** | [**CommunityChannelMessageSendRequest**](CommunityChannelMessageSendRequest.md)|  | 


### Return type

[**ChannelMessageSendResponse**](ChannelMessageSendResponse.md)

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

# **send_direct_channel_message**
> UserMessageSendResponse send_direct_channel_message(direct_channel_message_send_request)

Send a direct message

Rate limit: 6,000 msgs/min (by recipient count).

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.direct_channel_message_send_request import DirectChannelMessageSendRequest
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    direct_channel_message_send_request = ncsdk.DirectChannelMessageSendRequest() # DirectChannelMessageSendRequest | 
    

    try:
        # Send a direct message
        api_response = api_instance.send_direct_channel_message(direct_channel_message_send_request)
        print("The response of MessageManagementApi->send_direct_channel_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->send_direct_channel_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **direct_channel_message_send_request** | [**DirectChannelMessageSendRequest**](DirectChannelMessageSendRequest.md)|  | 


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

# **send_direct_channel_stream_message**
> StreamMessageSendResponse send_direct_channel_stream_message(direct_channel_stream_message_send_request)

Send a direct channel stream message

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.direct_channel_stream_message_send_request import DirectChannelStreamMessageSendRequest
from ncsdk.models.stream_message_send_response import StreamMessageSendResponse
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    direct_channel_stream_message_send_request = ncsdk.DirectChannelStreamMessageSendRequest() # DirectChannelStreamMessageSendRequest | 
    

    try:
        # Send a direct channel stream message
        api_response = api_instance.send_direct_channel_stream_message(direct_channel_stream_message_send_request)
        print("The response of MessageManagementApi->send_direct_channel_stream_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->send_direct_channel_stream_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **direct_channel_stream_message_send_request** | [**DirectChannelStreamMessageSendRequest**](DirectChannelStreamMessageSendRequest.md)|  | 


### Return type

[**StreamMessageSendResponse**](StreamMessageSendResponse.md)

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

# **send_group_channel_message**
> ChannelMessageSendResponse send_group_channel_message(group_channel_message_send_request)

Send a group message

Rate limit: 20/sec (by target group count).

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.channel_message_send_response import ChannelMessageSendResponse
from ncsdk.models.group_channel_message_send_request import GroupChannelMessageSendRequest
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    group_channel_message_send_request = ncsdk.GroupChannelMessageSendRequest() # GroupChannelMessageSendRequest | 
    

    try:
        # Send a group message
        api_response = api_instance.send_group_channel_message(group_channel_message_send_request)
        print("The response of MessageManagementApi->send_group_channel_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->send_group_channel_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_message_send_request** | [**GroupChannelMessageSendRequest**](GroupChannelMessageSendRequest.md)|  | 


### Return type

[**ChannelMessageSendResponse**](ChannelMessageSendResponse.md)

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

# **send_group_channel_stream_message**
> StreamMessageSendResponse send_group_channel_stream_message(group_channel_stream_message_send_request)

Send a group channel stream message

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.group_channel_stream_message_send_request import GroupChannelStreamMessageSendRequest
from ncsdk.models.stream_message_send_response import StreamMessageSendResponse
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    group_channel_stream_message_send_request = ncsdk.GroupChannelStreamMessageSendRequest() # GroupChannelStreamMessageSendRequest | 
    

    try:
        # Send a group channel stream message
        api_response = api_instance.send_group_channel_stream_message(group_channel_stream_message_send_request)
        print("The response of MessageManagementApi->send_group_channel_stream_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->send_group_channel_stream_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_stream_message_send_request** | [**GroupChannelStreamMessageSendRequest**](GroupChannelStreamMessageSendRequest.md)|  | 


### Return type

[**StreamMessageSendResponse**](StreamMessageSendResponse.md)

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

# **send_open_channel_message**
> ChannelMessageSendResponse send_open_channel_message(open_channel_message_send_request)

Send an open channel message

Rate limit: 100/sec (by target open channel count).

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.channel_message_send_response import ChannelMessageSendResponse
from ncsdk.models.open_channel_message_send_request import OpenChannelMessageSendRequest
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    open_channel_message_send_request = ncsdk.OpenChannelMessageSendRequest() # OpenChannelMessageSendRequest | 
    

    try:
        # Send an open channel message
        api_response = api_instance.send_open_channel_message(open_channel_message_send_request)
        print("The response of MessageManagementApi->send_open_channel_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->send_open_channel_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_message_send_request** | [**OpenChannelMessageSendRequest**](OpenChannelMessageSendRequest.md)|  | 


### Return type

[**ChannelMessageSendResponse**](ChannelMessageSendResponse.md)

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

# **set_channel_type_message_metadata**
> CodeOnlyResponse set_channel_type_message_metadata(message_metadata_set_request)

Set message metadata

Rate limit: 100/sec (max 20 for group messages).

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.message_metadata_set_request import MessageMetadataSetRequest
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    message_metadata_set_request = ncsdk.MessageMetadataSetRequest() # MessageMetadataSetRequest | 
    

    try:
        # Set message metadata
        api_response = api_instance.set_channel_type_message_metadata(message_metadata_set_request)
        print("The response of MessageManagementApi->set_channel_type_message_metadata:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->set_channel_type_message_metadata: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_metadata_set_request** | [**MessageMetadataSetRequest**](MessageMetadataSetRequest.md)|  | 


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

# **set_community_channel_message_metadata**
> CodeOnlyResponse set_community_channel_message_metadata(community_channel_message_metadata_set_request)

Set community-channel message metadata

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_message_metadata_set_request import CommunityChannelMessageMetadataSetRequest
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    community_channel_message_metadata_set_request = ncsdk.CommunityChannelMessageMetadataSetRequest() # CommunityChannelMessageMetadataSetRequest | 
    

    try:
        # Set community-channel message metadata
        api_response = api_instance.set_community_channel_message_metadata(community_channel_message_metadata_set_request)
        print("The response of MessageManagementApi->set_community_channel_message_metadata:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->set_community_channel_message_metadata: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_message_metadata_set_request** | [**CommunityChannelMessageMetadataSetRequest**](CommunityChannelMessageMetadataSetRequest.md)|  | 


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

# **update_community_channel_message**
> CodeOnlyResponse update_community_channel_message(community_channel_message_update_request)

Update community-channel message

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_message_update_request import CommunityChannelMessageUpdateRequest
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    community_channel_message_update_request = ncsdk.CommunityChannelMessageUpdateRequest() # CommunityChannelMessageUpdateRequest | 
    

    try:
        # Update community-channel message
        api_response = api_instance.update_community_channel_message(community_channel_message_update_request)
        print("The response of MessageManagementApi->update_community_channel_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->update_community_channel_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_message_update_request** | [**CommunityChannelMessageUpdateRequest**](CommunityChannelMessageUpdateRequest.md)|  | 


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

# **update_direct_channel_message**
> CodeOnlyResponse update_direct_channel_message(direct_channel_message_update_request)

Update direct-channel message

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.direct_channel_message_update_request import DirectChannelMessageUpdateRequest
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    direct_channel_message_update_request = ncsdk.DirectChannelMessageUpdateRequest() # DirectChannelMessageUpdateRequest | 
    

    try:
        # Update direct-channel message
        api_response = api_instance.update_direct_channel_message(direct_channel_message_update_request)
        print("The response of MessageManagementApi->update_direct_channel_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->update_direct_channel_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **direct_channel_message_update_request** | [**DirectChannelMessageUpdateRequest**](DirectChannelMessageUpdateRequest.md)|  | 


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

# **update_group_channel_message**
> CodeOnlyResponse update_group_channel_message(group_channel_message_update_request)

Update group-channel message

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_message_update_request import GroupChannelMessageUpdateRequest
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
    api_instance = ncsdk.MessageManagementApi(api_client)
    
    group_channel_message_update_request = ncsdk.GroupChannelMessageUpdateRequest() # GroupChannelMessageUpdateRequest | 
    

    try:
        # Update group-channel message
        api_response = api_instance.update_group_channel_message(group_channel_message_update_request)
        print("The response of MessageManagementApi->update_group_channel_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageManagementApi->update_group_channel_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_message_update_request** | [**GroupChannelMessageUpdateRequest**](GroupChannelMessageUpdateRequest.md)|  | 


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

