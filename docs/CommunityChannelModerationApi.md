# ncsdk.CommunityChannelModerationApi

All requests use the primary/backup domains configured by the caller.

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_community_channel_allowed_sender_list**](CommunityChannelModerationApi.md#add_community_channel_allowed_sender_list) | **POST** /v4/community-channel/allowed-sender-list/add | Add community channel allowed sender list
[**add_community_channel_muted_users**](CommunityChannelModerationApi.md#add_community_channel_muted_users) | **POST** /v4/community-channel/mute-list/add | Add community-channel muted users
[**get_community_channel_freeze_list**](CommunityChannelModerationApi.md#get_community_channel_freeze_list) | **POST** /v4/community-channel/freeze-list/get | Get community channel freeze status
[**list_community_channel_allowed_sender_list**](CommunityChannelModerationApi.md#list_community_channel_allowed_sender_list) | **POST** /v4/community-channel/allowed-sender-list/get | List community channel allowed sender list
[**list_community_channel_muted_users**](CommunityChannelModerationApi.md#list_community_channel_muted_users) | **POST** /v4/community-channel/mute-list/get | List community-channel muted users
[**remove_community_channel_allowed_sender_list**](CommunityChannelModerationApi.md#remove_community_channel_allowed_sender_list) | **POST** /v4/community-channel/allowed-sender-list/remove | Remove community channel allowed sender list
[**remove_community_channel_muted_users**](CommunityChannelModerationApi.md#remove_community_channel_muted_users) | **POST** /v4/community-channel/mute-list/remove | Remove community-channel muted users
[**set_community_channel_freeze_list**](CommunityChannelModerationApi.md#set_community_channel_freeze_list) | **POST** /v4/community-channel/freeze-list/set | Set community channel freeze list


# **add_community_channel_allowed_sender_list**
> CodeOnlyResponse add_community_channel_allowed_sender_list(community_channel_allowed_sender_list_update_request)

Add community channel allowed sender list

### Example

* Api Key Authentication (NexconnSignature):

```python
import os
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_allowed_sender_list_update_request import CommunityChannelAllowedSenderListUpdateRequest
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
    api_instance = ncsdk.CommunityChannelModerationApi(api_client)
    
    community_channel_allowed_sender_list_update_request = ncsdk.CommunityChannelAllowedSenderListUpdateRequest() # CommunityChannelAllowedSenderListUpdateRequest | 
    

    try:
        # Add community channel allowed sender list
        api_response = api_instance.add_community_channel_allowed_sender_list(community_channel_allowed_sender_list_update_request)
        print("The response of CommunityChannelModerationApi->add_community_channel_allowed_sender_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelModerationApi->add_community_channel_allowed_sender_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_allowed_sender_list_update_request** | [**CommunityChannelAllowedSenderListUpdateRequest**](CommunityChannelAllowedSenderListUpdateRequest.md)|  | 


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

# **add_community_channel_muted_users**
> CodeOnlyResponse add_community_channel_muted_users(community_channel_mute_list_add_request)

Add community-channel muted users

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_mute_list_add_request import CommunityChannelMuteListAddRequest
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
    api_instance = ncsdk.CommunityChannelModerationApi(api_client)
    
    community_channel_mute_list_add_request = ncsdk.CommunityChannelMuteListAddRequest() # CommunityChannelMuteListAddRequest | 
    

    try:
        # Add community-channel muted users
        api_response = api_instance.add_community_channel_muted_users(community_channel_mute_list_add_request)
        print("The response of CommunityChannelModerationApi->add_community_channel_muted_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelModerationApi->add_community_channel_muted_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_mute_list_add_request** | [**CommunityChannelMuteListAddRequest**](CommunityChannelMuteListAddRequest.md)|  | 


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

# **get_community_channel_freeze_list**
> CommunityChannelFreezeListGetResponse get_community_channel_freeze_list(community_channel_freeze_list_get_request)

Get community channel freeze status

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.community_channel_freeze_list_get_request import CommunityChannelFreezeListGetRequest
from ncsdk.models.community_channel_freeze_list_get_response import CommunityChannelFreezeListGetResponse
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
    api_instance = ncsdk.CommunityChannelModerationApi(api_client)
    
    community_channel_freeze_list_get_request = ncsdk.CommunityChannelFreezeListGetRequest() # CommunityChannelFreezeListGetRequest | 
    

    try:
        # Get community channel freeze status
        api_response = api_instance.get_community_channel_freeze_list(community_channel_freeze_list_get_request)
        print("The response of CommunityChannelModerationApi->get_community_channel_freeze_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelModerationApi->get_community_channel_freeze_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_freeze_list_get_request** | [**CommunityChannelFreezeListGetRequest**](CommunityChannelFreezeListGetRequest.md)|  | 


### Return type

[**CommunityChannelFreezeListGetResponse**](CommunityChannelFreezeListGetResponse.md)

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

# **list_community_channel_allowed_sender_list**
> CommunityChannelAllowedSenderListGetResponse list_community_channel_allowed_sender_list(community_channel_allowed_sender_list_get_request)

List community channel allowed sender list

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.community_channel_allowed_sender_list_get_request import CommunityChannelAllowedSenderListGetRequest
from ncsdk.models.community_channel_allowed_sender_list_get_response import CommunityChannelAllowedSenderListGetResponse
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
    api_instance = ncsdk.CommunityChannelModerationApi(api_client)
    
    community_channel_allowed_sender_list_get_request = ncsdk.CommunityChannelAllowedSenderListGetRequest() # CommunityChannelAllowedSenderListGetRequest | 
    

    try:
        # List community channel allowed sender list
        api_response = api_instance.list_community_channel_allowed_sender_list(community_channel_allowed_sender_list_get_request)
        print("The response of CommunityChannelModerationApi->list_community_channel_allowed_sender_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelModerationApi->list_community_channel_allowed_sender_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_allowed_sender_list_get_request** | [**CommunityChannelAllowedSenderListGetRequest**](CommunityChannelAllowedSenderListGetRequest.md)|  | 


### Return type

[**CommunityChannelAllowedSenderListGetResponse**](CommunityChannelAllowedSenderListGetResponse.md)

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

# **list_community_channel_muted_users**
> CommunityChannelMuteListGetResponse list_community_channel_muted_users(community_channel_mute_list_get_request)

List community-channel muted users

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.community_channel_mute_list_get_request import CommunityChannelMuteListGetRequest
from ncsdk.models.community_channel_mute_list_get_response import CommunityChannelMuteListGetResponse
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
    api_instance = ncsdk.CommunityChannelModerationApi(api_client)
    
    community_channel_mute_list_get_request = ncsdk.CommunityChannelMuteListGetRequest() # CommunityChannelMuteListGetRequest | 
    

    try:
        # List community-channel muted users
        api_response = api_instance.list_community_channel_muted_users(community_channel_mute_list_get_request)
        print("The response of CommunityChannelModerationApi->list_community_channel_muted_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelModerationApi->list_community_channel_muted_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_mute_list_get_request** | [**CommunityChannelMuteListGetRequest**](CommunityChannelMuteListGetRequest.md)|  | 


### Return type

[**CommunityChannelMuteListGetResponse**](CommunityChannelMuteListGetResponse.md)

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

# **remove_community_channel_allowed_sender_list**
> CodeOnlyResponse remove_community_channel_allowed_sender_list(community_channel_allowed_sender_list_update_request)

Remove community channel allowed sender list

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_allowed_sender_list_update_request import CommunityChannelAllowedSenderListUpdateRequest
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
    api_instance = ncsdk.CommunityChannelModerationApi(api_client)
    
    community_channel_allowed_sender_list_update_request = ncsdk.CommunityChannelAllowedSenderListUpdateRequest() # CommunityChannelAllowedSenderListUpdateRequest | 
    

    try:
        # Remove community channel allowed sender list
        api_response = api_instance.remove_community_channel_allowed_sender_list(community_channel_allowed_sender_list_update_request)
        print("The response of CommunityChannelModerationApi->remove_community_channel_allowed_sender_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelModerationApi->remove_community_channel_allowed_sender_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_allowed_sender_list_update_request** | [**CommunityChannelAllowedSenderListUpdateRequest**](CommunityChannelAllowedSenderListUpdateRequest.md)|  | 


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

# **remove_community_channel_muted_users**
> CodeOnlyResponse remove_community_channel_muted_users(community_channel_mute_list_remove_request)

Remove community-channel muted users

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_mute_list_remove_request import CommunityChannelMuteListRemoveRequest
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
    api_instance = ncsdk.CommunityChannelModerationApi(api_client)
    
    community_channel_mute_list_remove_request = ncsdk.CommunityChannelMuteListRemoveRequest() # CommunityChannelMuteListRemoveRequest | 
    

    try:
        # Remove community-channel muted users
        api_response = api_instance.remove_community_channel_muted_users(community_channel_mute_list_remove_request)
        print("The response of CommunityChannelModerationApi->remove_community_channel_muted_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelModerationApi->remove_community_channel_muted_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_mute_list_remove_request** | [**CommunityChannelMuteListRemoveRequest**](CommunityChannelMuteListRemoveRequest.md)|  | 


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

# **set_community_channel_freeze_list**
> CodeOnlyResponse set_community_channel_freeze_list(community_channel_freeze_list_set_request)

Set community channel freeze list

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_freeze_list_set_request import CommunityChannelFreezeListSetRequest
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
    api_instance = ncsdk.CommunityChannelModerationApi(api_client)
    
    community_channel_freeze_list_set_request = ncsdk.CommunityChannelFreezeListSetRequest() # CommunityChannelFreezeListSetRequest | 
    

    try:
        # Set community channel freeze list
        api_response = api_instance.set_community_channel_freeze_list(community_channel_freeze_list_set_request)
        print("The response of CommunityChannelModerationApi->set_community_channel_freeze_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelModerationApi->set_community_channel_freeze_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_freeze_list_set_request** | [**CommunityChannelFreezeListSetRequest**](CommunityChannelFreezeListSetRequest.md)|  | 


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

