# ncsdk.GroupChannelModerationApi

All requests use the primary/backup domains configured by the caller.

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_group_channel_allowed_sender_list**](GroupChannelModerationApi.md#add_group_channel_allowed_sender_list) | **POST** /v4/group-channel/allowed-sender-list/add | Add to allowed senders list
[**add_group_channel_freeze_list**](GroupChannelModerationApi.md#add_group_channel_freeze_list) | **POST** /v4/group-channel/freeze-list/add | Freeze a group
[**add_group_channel_user_mute_list**](GroupChannelModerationApi.md#add_group_channel_user_mute_list) | **POST** /v4/group-channel/user/mute-list/add | Mute a group member
[**get_group_channel_allowed_sender_list**](GroupChannelModerationApi.md#get_group_channel_allowed_sender_list) | **POST** /v4/group-channel/allowed-sender-list/get | Query allowed senders list
[**get_group_channel_freeze_list**](GroupChannelModerationApi.md#get_group_channel_freeze_list) | **POST** /v4/group-channel/freeze-list/get | Query group freeze status
[**get_group_channel_user_mute_list**](GroupChannelModerationApi.md#get_group_channel_user_mute_list) | **POST** /v4/group-channel/user/mute-list/get | List muted group members
[**remove_group_channel_allowed_sender_list**](GroupChannelModerationApi.md#remove_group_channel_allowed_sender_list) | **POST** /v4/group-channel/allowed-sender-list/remove | Remove from allowed senders list
[**remove_group_channel_freeze_list**](GroupChannelModerationApi.md#remove_group_channel_freeze_list) | **POST** /v4/group-channel/freeze-list/remove | Unfreeze a group
[**remove_group_channel_user_mute_list**](GroupChannelModerationApi.md#remove_group_channel_user_mute_list) | **POST** /v4/group-channel/user/mute-list/remove | Unmute a group member


# **add_group_channel_allowed_sender_list**
> CodeOnlyResponse add_group_channel_allowed_sender_list(group_channel_allowed_sender_list_update_request)

Add to allowed senders list

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import os
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_allowed_sender_list_update_request import GroupChannelAllowedSenderListUpdateRequest
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
    api_instance = ncsdk.GroupChannelModerationApi(api_client)
    
    group_channel_allowed_sender_list_update_request = ncsdk.GroupChannelAllowedSenderListUpdateRequest() # GroupChannelAllowedSenderListUpdateRequest | 
    

    try:
        # Add to allowed senders list
        api_response = api_instance.add_group_channel_allowed_sender_list(group_channel_allowed_sender_list_update_request)
        print("The response of GroupChannelModerationApi->add_group_channel_allowed_sender_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelModerationApi->add_group_channel_allowed_sender_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_allowed_sender_list_update_request** | [**GroupChannelAllowedSenderListUpdateRequest**](GroupChannelAllowedSenderListUpdateRequest.md)|  | 


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

# **add_group_channel_freeze_list**
> CodeOnlyResponse add_group_channel_freeze_list(group_channel_freeze_list_update_request)

Freeze a group

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_freeze_list_update_request import GroupChannelFreezeListUpdateRequest
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
    api_instance = ncsdk.GroupChannelModerationApi(api_client)
    
    group_channel_freeze_list_update_request = ncsdk.GroupChannelFreezeListUpdateRequest() # GroupChannelFreezeListUpdateRequest | 
    

    try:
        # Freeze a group
        api_response = api_instance.add_group_channel_freeze_list(group_channel_freeze_list_update_request)
        print("The response of GroupChannelModerationApi->add_group_channel_freeze_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelModerationApi->add_group_channel_freeze_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_freeze_list_update_request** | [**GroupChannelFreezeListUpdateRequest**](GroupChannelFreezeListUpdateRequest.md)|  | 


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

# **add_group_channel_user_mute_list**
> CodeOnlyResponse add_group_channel_user_mute_list(group_channel_user_mute_list_add_request)

Mute a group member

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_user_mute_list_add_request import GroupChannelUserMuteListAddRequest
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
    api_instance = ncsdk.GroupChannelModerationApi(api_client)
    
    group_channel_user_mute_list_add_request = ncsdk.GroupChannelUserMuteListAddRequest() # GroupChannelUserMuteListAddRequest | 
    

    try:
        # Mute a group member
        api_response = api_instance.add_group_channel_user_mute_list(group_channel_user_mute_list_add_request)
        print("The response of GroupChannelModerationApi->add_group_channel_user_mute_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelModerationApi->add_group_channel_user_mute_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_user_mute_list_add_request** | [**GroupChannelUserMuteListAddRequest**](GroupChannelUserMuteListAddRequest.md)|  | 


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

# **get_group_channel_allowed_sender_list**
> GroupChannelAllowedSenderListGetResponse get_group_channel_allowed_sender_list(group_channel_allowed_sender_list_get_request)

Query allowed senders list

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.group_channel_allowed_sender_list_get_request import GroupChannelAllowedSenderListGetRequest
from ncsdk.models.group_channel_allowed_sender_list_get_response import GroupChannelAllowedSenderListGetResponse
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
    api_instance = ncsdk.GroupChannelModerationApi(api_client)
    
    group_channel_allowed_sender_list_get_request = ncsdk.GroupChannelAllowedSenderListGetRequest() # GroupChannelAllowedSenderListGetRequest | 
    

    try:
        # Query allowed senders list
        api_response = api_instance.get_group_channel_allowed_sender_list(group_channel_allowed_sender_list_get_request)
        print("The response of GroupChannelModerationApi->get_group_channel_allowed_sender_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelModerationApi->get_group_channel_allowed_sender_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_allowed_sender_list_get_request** | [**GroupChannelAllowedSenderListGetRequest**](GroupChannelAllowedSenderListGetRequest.md)|  | 


### Return type

[**GroupChannelAllowedSenderListGetResponse**](GroupChannelAllowedSenderListGetResponse.md)

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

# **get_group_channel_freeze_list**
> GroupChannelFreezeListGetResponse get_group_channel_freeze_list(group_channel_freeze_list_get_request)

Query group freeze status

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.group_channel_freeze_list_get_request import GroupChannelFreezeListGetRequest
from ncsdk.models.group_channel_freeze_list_get_response import GroupChannelFreezeListGetResponse
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
    api_instance = ncsdk.GroupChannelModerationApi(api_client)
    
    group_channel_freeze_list_get_request = ncsdk.GroupChannelFreezeListGetRequest() # GroupChannelFreezeListGetRequest | 
    

    try:
        # Query group freeze status
        api_response = api_instance.get_group_channel_freeze_list(group_channel_freeze_list_get_request)
        print("The response of GroupChannelModerationApi->get_group_channel_freeze_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelModerationApi->get_group_channel_freeze_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_freeze_list_get_request** | [**GroupChannelFreezeListGetRequest**](GroupChannelFreezeListGetRequest.md)|  | 


### Return type

[**GroupChannelFreezeListGetResponse**](GroupChannelFreezeListGetResponse.md)

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

# **get_group_channel_user_mute_list**
> GroupChannelUserMuteListGetResponse get_group_channel_user_mute_list(group_channel_user_mute_list_get_request)

List muted group members

Rate limit: 100/sec. The public endpoint list currently publishes this capability as `/v4/group-channel/user/mute-list-get`.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.group_channel_user_mute_list_get_request import GroupChannelUserMuteListGetRequest
from ncsdk.models.group_channel_user_mute_list_get_response import GroupChannelUserMuteListGetResponse
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
    api_instance = ncsdk.GroupChannelModerationApi(api_client)
    
    group_channel_user_mute_list_get_request = ncsdk.GroupChannelUserMuteListGetRequest() # GroupChannelUserMuteListGetRequest | 
    

    try:
        # List muted group members
        api_response = api_instance.get_group_channel_user_mute_list(group_channel_user_mute_list_get_request)
        print("The response of GroupChannelModerationApi->get_group_channel_user_mute_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelModerationApi->get_group_channel_user_mute_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_user_mute_list_get_request** | [**GroupChannelUserMuteListGetRequest**](GroupChannelUserMuteListGetRequest.md)|  | 


### Return type

[**GroupChannelUserMuteListGetResponse**](GroupChannelUserMuteListGetResponse.md)

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

# **remove_group_channel_allowed_sender_list**
> CodeOnlyResponse remove_group_channel_allowed_sender_list(group_channel_allowed_sender_list_update_request)

Remove from allowed senders list

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_allowed_sender_list_update_request import GroupChannelAllowedSenderListUpdateRequest
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
    api_instance = ncsdk.GroupChannelModerationApi(api_client)
    
    group_channel_allowed_sender_list_update_request = ncsdk.GroupChannelAllowedSenderListUpdateRequest() # GroupChannelAllowedSenderListUpdateRequest | 
    

    try:
        # Remove from allowed senders list
        api_response = api_instance.remove_group_channel_allowed_sender_list(group_channel_allowed_sender_list_update_request)
        print("The response of GroupChannelModerationApi->remove_group_channel_allowed_sender_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelModerationApi->remove_group_channel_allowed_sender_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_allowed_sender_list_update_request** | [**GroupChannelAllowedSenderListUpdateRequest**](GroupChannelAllowedSenderListUpdateRequest.md)|  | 


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

# **remove_group_channel_freeze_list**
> CodeOnlyResponse remove_group_channel_freeze_list(group_channel_freeze_list_update_request)

Unfreeze a group

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_freeze_list_update_request import GroupChannelFreezeListUpdateRequest
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
    api_instance = ncsdk.GroupChannelModerationApi(api_client)
    
    group_channel_freeze_list_update_request = ncsdk.GroupChannelFreezeListUpdateRequest() # GroupChannelFreezeListUpdateRequest | 
    

    try:
        # Unfreeze a group
        api_response = api_instance.remove_group_channel_freeze_list(group_channel_freeze_list_update_request)
        print("The response of GroupChannelModerationApi->remove_group_channel_freeze_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelModerationApi->remove_group_channel_freeze_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_freeze_list_update_request** | [**GroupChannelFreezeListUpdateRequest**](GroupChannelFreezeListUpdateRequest.md)|  | 


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

# **remove_group_channel_user_mute_list**
> CodeOnlyResponse remove_group_channel_user_mute_list(group_channel_user_mute_list_remove_request)

Unmute a group member

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_user_mute_list_remove_request import GroupChannelUserMuteListRemoveRequest
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
    api_instance = ncsdk.GroupChannelModerationApi(api_client)
    
    group_channel_user_mute_list_remove_request = ncsdk.GroupChannelUserMuteListRemoveRequest() # GroupChannelUserMuteListRemoveRequest | 
    

    try:
        # Unmute a group member
        api_response = api_instance.remove_group_channel_user_mute_list(group_channel_user_mute_list_remove_request)
        print("The response of GroupChannelModerationApi->remove_group_channel_user_mute_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelModerationApi->remove_group_channel_user_mute_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_user_mute_list_remove_request** | [**GroupChannelUserMuteListRemoveRequest**](GroupChannelUserMuteListRemoveRequest.md)|  | 


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

