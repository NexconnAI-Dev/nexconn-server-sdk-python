# ncsdk.OpenChannelParticipantsModerationApi

All requests use the primary/backup domains configured by the caller.

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_open_channel_freeze_list**](OpenChannelParticipantsModerationApi.md#add_open_channel_freeze_list) | **POST** /v4/open-channel/freeze-list/add | Freeze an open channel
[**add_open_channel_global_mute_list**](OpenChannelParticipantsModerationApi.md#add_open_channel_global_mute_list) | **POST** /v4/open-channel/global-mute-list/add | Mute a user globally
[**add_open_channel_participant_allowed_sender_list**](OpenChannelParticipantsModerationApi.md#add_open_channel_participant_allowed_sender_list) | **POST** /v4/open-channel/participant/allowed-sender-list/add | Add to allowed senders list
[**add_open_channel_participant_ban_list**](OpenChannelParticipantsModerationApi.md#add_open_channel_participant_ban_list) | **POST** /v4/open-channel/participant/ban-list/add | Ban a participant
[**add_open_channel_participant_mute_list**](OpenChannelParticipantsModerationApi.md#add_open_channel_participant_mute_list) | **POST** /v4/open-channel/participant/mute-list/add | Mute a participant
[**check_open_channel_freeze**](OpenChannelParticipantsModerationApi.md#check_open_channel_freeze) | **POST** /v4/open-channel/freeze/check | Check open channel freeze status
[**check_open_channel_participants_exist**](OpenChannelParticipantsModerationApi.md#check_open_channel_participants_exist) | **POST** /v4/open-channel/participant/exist | Batch check participants
[**get_open_channel_global_mute_list**](OpenChannelParticipantsModerationApi.md#get_open_channel_global_mute_list) | **POST** /v4/open-channel/global-mute-list/get | List globally muted users
[**get_open_channel_participant_allowed_sender_list**](OpenChannelParticipantsModerationApi.md#get_open_channel_participant_allowed_sender_list) | **POST** /v4/open-channel/participant/allowed-sender-list/get | Query allowed senders list
[**get_open_channel_participant_ban_list**](OpenChannelParticipantsModerationApi.md#get_open_channel_participant_ban_list) | **POST** /v4/open-channel/participant/ban-list/get | List banned participants
[**get_open_channel_participant_mute_list**](OpenChannelParticipantsModerationApi.md#get_open_channel_participant_mute_list) | **POST** /v4/open-channel/participant/mute-list/get | List muted participants
[**list_frozen_open_channels**](OpenChannelParticipantsModerationApi.md#list_frozen_open_channels) | **POST** /v4/open-channel/freeze-list/get | List frozen open channels
[**list_open_channel_participants**](OpenChannelParticipantsModerationApi.md#list_open_channel_participants) | **POST** /v4/open-channel/participant/list | List participants
[**remove_open_channel_freeze_list**](OpenChannelParticipantsModerationApi.md#remove_open_channel_freeze_list) | **POST** /v4/open-channel/freeze-list/remove | Unfreeze an open channel
[**remove_open_channel_global_mute_list**](OpenChannelParticipantsModerationApi.md#remove_open_channel_global_mute_list) | **POST** /v4/open-channel/global-mute-list/remove | Unmute a user globally
[**remove_open_channel_participant_allowed_sender_list**](OpenChannelParticipantsModerationApi.md#remove_open_channel_participant_allowed_sender_list) | **POST** /v4/open-channel/participant/allowed-sender-list/remove | Remove from allowed senders list
[**remove_open_channel_participant_ban_list**](OpenChannelParticipantsModerationApi.md#remove_open_channel_participant_ban_list) | **POST** /v4/open-channel/participant/ban-list/remove | Unban a participant
[**remove_open_channel_participant_mute_list**](OpenChannelParticipantsModerationApi.md#remove_open_channel_participant_mute_list) | **POST** /v4/open-channel/participant/mute-list/remove | Unmute a participant


# **add_open_channel_freeze_list**
> CodeOnlyResponse add_open_channel_freeze_list(open_channel_freeze_list_update_request)

Freeze an open channel

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import os
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_freeze_list_update_request import OpenChannelFreezeListUpdateRequest
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_freeze_list_update_request = ncsdk.OpenChannelFreezeListUpdateRequest() # OpenChannelFreezeListUpdateRequest | 
    

    try:
        # Freeze an open channel
        api_response = api_instance.add_open_channel_freeze_list(open_channel_freeze_list_update_request)
        print("The response of OpenChannelParticipantsModerationApi->add_open_channel_freeze_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->add_open_channel_freeze_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_freeze_list_update_request** | [**OpenChannelFreezeListUpdateRequest**](OpenChannelFreezeListUpdateRequest.md)|  | 


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

# **add_open_channel_global_mute_list**
> CodeOnlyResponse add_open_channel_global_mute_list(open_channel_global_mute_list_add_request)

Mute a user globally

Rate limit: 100/sec. The public endpoint list currently publishes this capability as `/v4/open-channel/participant/global-mute-list/add`.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_global_mute_list_add_request import OpenChannelGlobalMuteListAddRequest
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_global_mute_list_add_request = ncsdk.OpenChannelGlobalMuteListAddRequest() # OpenChannelGlobalMuteListAddRequest | 
    

    try:
        # Mute a user globally
        api_response = api_instance.add_open_channel_global_mute_list(open_channel_global_mute_list_add_request)
        print("The response of OpenChannelParticipantsModerationApi->add_open_channel_global_mute_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->add_open_channel_global_mute_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_global_mute_list_add_request** | [**OpenChannelGlobalMuteListAddRequest**](OpenChannelGlobalMuteListAddRequest.md)|  | 


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

# **add_open_channel_participant_allowed_sender_list**
> CodeOnlyResponse add_open_channel_participant_allowed_sender_list(open_channel_allowed_sender_list_update_request)

Add to allowed senders list

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_allowed_sender_list_update_request import OpenChannelAllowedSenderListUpdateRequest
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_allowed_sender_list_update_request = ncsdk.OpenChannelAllowedSenderListUpdateRequest() # OpenChannelAllowedSenderListUpdateRequest | 
    

    try:
        # Add to allowed senders list
        api_response = api_instance.add_open_channel_participant_allowed_sender_list(open_channel_allowed_sender_list_update_request)
        print("The response of OpenChannelParticipantsModerationApi->add_open_channel_participant_allowed_sender_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->add_open_channel_participant_allowed_sender_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_allowed_sender_list_update_request** | [**OpenChannelAllowedSenderListUpdateRequest**](OpenChannelAllowedSenderListUpdateRequest.md)|  | 


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

# **add_open_channel_participant_ban_list**
> CodeOnlyResponse add_open_channel_participant_ban_list(open_channel_participant_mute_list_add_request)

Ban a participant

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_participant_mute_list_add_request import OpenChannelParticipantMuteListAddRequest
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_participant_mute_list_add_request = ncsdk.OpenChannelParticipantMuteListAddRequest() # OpenChannelParticipantMuteListAddRequest | 
    

    try:
        # Ban a participant
        api_response = api_instance.add_open_channel_participant_ban_list(open_channel_participant_mute_list_add_request)
        print("The response of OpenChannelParticipantsModerationApi->add_open_channel_participant_ban_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->add_open_channel_participant_ban_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_participant_mute_list_add_request** | [**OpenChannelParticipantMuteListAddRequest**](OpenChannelParticipantMuteListAddRequest.md)|  | 


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

# **add_open_channel_participant_mute_list**
> CodeOnlyResponse add_open_channel_participant_mute_list(open_channel_participant_mute_list_add_request)

Mute a participant

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_participant_mute_list_add_request import OpenChannelParticipantMuteListAddRequest
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_participant_mute_list_add_request = ncsdk.OpenChannelParticipantMuteListAddRequest() # OpenChannelParticipantMuteListAddRequest | 
    

    try:
        # Mute a participant
        api_response = api_instance.add_open_channel_participant_mute_list(open_channel_participant_mute_list_add_request)
        print("The response of OpenChannelParticipantsModerationApi->add_open_channel_participant_mute_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->add_open_channel_participant_mute_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_participant_mute_list_add_request** | [**OpenChannelParticipantMuteListAddRequest**](OpenChannelParticipantMuteListAddRequest.md)|  | 


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

# **check_open_channel_freeze**
> OpenChannelFreezeCheckResponse check_open_channel_freeze(open_channel_freeze_check_request)

Check open channel freeze status

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.open_channel_freeze_check_request import OpenChannelFreezeCheckRequest
from ncsdk.models.open_channel_freeze_check_response import OpenChannelFreezeCheckResponse
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_freeze_check_request = ncsdk.OpenChannelFreezeCheckRequest() # OpenChannelFreezeCheckRequest | 
    

    try:
        # Check open channel freeze status
        api_response = api_instance.check_open_channel_freeze(open_channel_freeze_check_request)
        print("The response of OpenChannelParticipantsModerationApi->check_open_channel_freeze:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->check_open_channel_freeze: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_freeze_check_request** | [**OpenChannelFreezeCheckRequest**](OpenChannelFreezeCheckRequest.md)|  | 


### Return type

[**OpenChannelFreezeCheckResponse**](OpenChannelFreezeCheckResponse.md)

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

# **check_open_channel_participants_exist**
> OpenChannelParticipantExistResponse check_open_channel_participants_exist(open_channel_participant_exist_request)

Batch check participants

Rate limit: 100/sec. The same endpoint is also documented for single-user participant checks.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.open_channel_participant_exist_request import OpenChannelParticipantExistRequest
from ncsdk.models.open_channel_participant_exist_response import OpenChannelParticipantExistResponse
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_participant_exist_request = ncsdk.OpenChannelParticipantExistRequest() # OpenChannelParticipantExistRequest | 
    

    try:
        # Batch check participants
        api_response = api_instance.check_open_channel_participants_exist(open_channel_participant_exist_request)
        print("The response of OpenChannelParticipantsModerationApi->check_open_channel_participants_exist:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->check_open_channel_participants_exist: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_participant_exist_request** | [**OpenChannelParticipantExistRequest**](OpenChannelParticipantExistRequest.md)|  | 


### Return type

[**OpenChannelParticipantExistResponse**](OpenChannelParticipantExistResponse.md)

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

# **get_open_channel_global_mute_list**
> OpenChannelParticipantMuteListGetResponse get_open_channel_global_mute_list()

List globally muted users

Rate limit: 100/sec. The public endpoint list currently publishes this capability as `/v4/open-channel/participant/global-mute-list/get`.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.open_channel_participant_mute_list_get_response import OpenChannelParticipantMuteListGetResponse
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    

    try:
        # List globally muted users
        api_response = api_instance.get_open_channel_global_mute_list()
        print("The response of OpenChannelParticipantsModerationApi->get_open_channel_global_mute_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->get_open_channel_global_mute_list: %s\n" % e)
```



### Parameters

This endpoint does not require a request body.

### Return type

[**OpenChannelParticipantMuteListGetResponse**](OpenChannelParticipantMuteListGetResponse.md)

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

# **get_open_channel_participant_allowed_sender_list**
> OpenChannelAllowedSenderListGetResponse get_open_channel_participant_allowed_sender_list(open_channel_participant_list_by_channel_request)

Query allowed senders list

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.open_channel_allowed_sender_list_get_response import OpenChannelAllowedSenderListGetResponse
from ncsdk.models.open_channel_participant_list_by_channel_request import OpenChannelParticipantListByChannelRequest
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_participant_list_by_channel_request = ncsdk.OpenChannelParticipantListByChannelRequest() # OpenChannelParticipantListByChannelRequest | 
    

    try:
        # Query allowed senders list
        api_response = api_instance.get_open_channel_participant_allowed_sender_list(open_channel_participant_list_by_channel_request)
        print("The response of OpenChannelParticipantsModerationApi->get_open_channel_participant_allowed_sender_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->get_open_channel_participant_allowed_sender_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_participant_list_by_channel_request** | [**OpenChannelParticipantListByChannelRequest**](OpenChannelParticipantListByChannelRequest.md)|  | 


### Return type

[**OpenChannelAllowedSenderListGetResponse**](OpenChannelAllowedSenderListGetResponse.md)

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

# **get_open_channel_participant_ban_list**
> OpenChannelParticipantBanListGetResponse get_open_channel_participant_ban_list(open_channel_participant_list_by_channel_request)

List banned participants

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.open_channel_participant_ban_list_get_response import OpenChannelParticipantBanListGetResponse
from ncsdk.models.open_channel_participant_list_by_channel_request import OpenChannelParticipantListByChannelRequest
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_participant_list_by_channel_request = ncsdk.OpenChannelParticipantListByChannelRequest() # OpenChannelParticipantListByChannelRequest | 
    

    try:
        # List banned participants
        api_response = api_instance.get_open_channel_participant_ban_list(open_channel_participant_list_by_channel_request)
        print("The response of OpenChannelParticipantsModerationApi->get_open_channel_participant_ban_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->get_open_channel_participant_ban_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_participant_list_by_channel_request** | [**OpenChannelParticipantListByChannelRequest**](OpenChannelParticipantListByChannelRequest.md)|  | 


### Return type

[**OpenChannelParticipantBanListGetResponse**](OpenChannelParticipantBanListGetResponse.md)

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

# **get_open_channel_participant_mute_list**
> OpenChannelParticipantMuteListGetResponse get_open_channel_participant_mute_list(open_channel_participant_list_by_channel_request)

List muted participants

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.open_channel_participant_list_by_channel_request import OpenChannelParticipantListByChannelRequest
from ncsdk.models.open_channel_participant_mute_list_get_response import OpenChannelParticipantMuteListGetResponse
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_participant_list_by_channel_request = ncsdk.OpenChannelParticipantListByChannelRequest() # OpenChannelParticipantListByChannelRequest | 
    

    try:
        # List muted participants
        api_response = api_instance.get_open_channel_participant_mute_list(open_channel_participant_list_by_channel_request)
        print("The response of OpenChannelParticipantsModerationApi->get_open_channel_participant_mute_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->get_open_channel_participant_mute_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_participant_list_by_channel_request** | [**OpenChannelParticipantListByChannelRequest**](OpenChannelParticipantListByChannelRequest.md)|  | 


### Return type

[**OpenChannelParticipantMuteListGetResponse**](OpenChannelParticipantMuteListGetResponse.md)

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

# **list_frozen_open_channels**
> OpenChannelFreezeListGetResponse list_frozen_open_channels(open_channel_freeze_list_get_request)

List frozen open channels

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.open_channel_freeze_list_get_request import OpenChannelFreezeListGetRequest
from ncsdk.models.open_channel_freeze_list_get_response import OpenChannelFreezeListGetResponse
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_freeze_list_get_request = ncsdk.OpenChannelFreezeListGetRequest() # OpenChannelFreezeListGetRequest | 
    

    try:
        # List frozen open channels
        api_response = api_instance.list_frozen_open_channels(open_channel_freeze_list_get_request)
        print("The response of OpenChannelParticipantsModerationApi->list_frozen_open_channels:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->list_frozen_open_channels: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_freeze_list_get_request** | [**OpenChannelFreezeListGetRequest**](OpenChannelFreezeListGetRequest.md)|  | 


### Return type

[**OpenChannelFreezeListGetResponse**](OpenChannelFreezeListGetResponse.md)

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

# **list_open_channel_participants**
> OpenChannelParticipantListResponse list_open_channel_participants(open_channel_participant_list_request)

List participants

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.open_channel_participant_list_request import OpenChannelParticipantListRequest
from ncsdk.models.open_channel_participant_list_response import OpenChannelParticipantListResponse
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_participant_list_request = ncsdk.OpenChannelParticipantListRequest() # OpenChannelParticipantListRequest | 
    

    try:
        # List participants
        api_response = api_instance.list_open_channel_participants(open_channel_participant_list_request)
        print("The response of OpenChannelParticipantsModerationApi->list_open_channel_participants:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->list_open_channel_participants: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_participant_list_request** | [**OpenChannelParticipantListRequest**](OpenChannelParticipantListRequest.md)|  | 


### Return type

[**OpenChannelParticipantListResponse**](OpenChannelParticipantListResponse.md)

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

# **remove_open_channel_freeze_list**
> CodeOnlyResponse remove_open_channel_freeze_list(open_channel_freeze_list_update_request)

Unfreeze an open channel

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_freeze_list_update_request import OpenChannelFreezeListUpdateRequest
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_freeze_list_update_request = ncsdk.OpenChannelFreezeListUpdateRequest() # OpenChannelFreezeListUpdateRequest | 
    

    try:
        # Unfreeze an open channel
        api_response = api_instance.remove_open_channel_freeze_list(open_channel_freeze_list_update_request)
        print("The response of OpenChannelParticipantsModerationApi->remove_open_channel_freeze_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->remove_open_channel_freeze_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_freeze_list_update_request** | [**OpenChannelFreezeListUpdateRequest**](OpenChannelFreezeListUpdateRequest.md)|  | 


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

# **remove_open_channel_global_mute_list**
> CodeOnlyResponse remove_open_channel_global_mute_list(open_channel_global_mute_list_remove_request)

Unmute a user globally

Rate limit: 100/sec. The public endpoint list currently publishes this capability as `/v4/open-channel/participant/global-mute-list/remove`.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_global_mute_list_remove_request import OpenChannelGlobalMuteListRemoveRequest
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_global_mute_list_remove_request = ncsdk.OpenChannelGlobalMuteListRemoveRequest() # OpenChannelGlobalMuteListRemoveRequest | 
    

    try:
        # Unmute a user globally
        api_response = api_instance.remove_open_channel_global_mute_list(open_channel_global_mute_list_remove_request)
        print("The response of OpenChannelParticipantsModerationApi->remove_open_channel_global_mute_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->remove_open_channel_global_mute_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_global_mute_list_remove_request** | [**OpenChannelGlobalMuteListRemoveRequest**](OpenChannelGlobalMuteListRemoveRequest.md)|  | 


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

# **remove_open_channel_participant_allowed_sender_list**
> CodeOnlyResponse remove_open_channel_participant_allowed_sender_list(open_channel_allowed_sender_list_update_request)

Remove from allowed senders list

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_allowed_sender_list_update_request import OpenChannelAllowedSenderListUpdateRequest
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_allowed_sender_list_update_request = ncsdk.OpenChannelAllowedSenderListUpdateRequest() # OpenChannelAllowedSenderListUpdateRequest | 
    

    try:
        # Remove from allowed senders list
        api_response = api_instance.remove_open_channel_participant_allowed_sender_list(open_channel_allowed_sender_list_update_request)
        print("The response of OpenChannelParticipantsModerationApi->remove_open_channel_participant_allowed_sender_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->remove_open_channel_participant_allowed_sender_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_allowed_sender_list_update_request** | [**OpenChannelAllowedSenderListUpdateRequest**](OpenChannelAllowedSenderListUpdateRequest.md)|  | 


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

# **remove_open_channel_participant_ban_list**
> CodeOnlyResponse remove_open_channel_participant_ban_list(open_channel_participant_mute_list_remove_request)

Unban a participant

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_participant_mute_list_remove_request import OpenChannelParticipantMuteListRemoveRequest
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_participant_mute_list_remove_request = ncsdk.OpenChannelParticipantMuteListRemoveRequest() # OpenChannelParticipantMuteListRemoveRequest | 
    

    try:
        # Unban a participant
        api_response = api_instance.remove_open_channel_participant_ban_list(open_channel_participant_mute_list_remove_request)
        print("The response of OpenChannelParticipantsModerationApi->remove_open_channel_participant_ban_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->remove_open_channel_participant_ban_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_participant_mute_list_remove_request** | [**OpenChannelParticipantMuteListRemoveRequest**](OpenChannelParticipantMuteListRemoveRequest.md)|  | 


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

# **remove_open_channel_participant_mute_list**
> CodeOnlyResponse remove_open_channel_participant_mute_list(open_channel_participant_mute_list_remove_request)

Unmute a participant

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_participant_mute_list_remove_request import OpenChannelParticipantMuteListRemoveRequest
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
    api_instance = ncsdk.OpenChannelParticipantsModerationApi(api_client)
    
    open_channel_participant_mute_list_remove_request = ncsdk.OpenChannelParticipantMuteListRemoveRequest() # OpenChannelParticipantMuteListRemoveRequest | 
    

    try:
        # Unmute a participant
        api_response = api_instance.remove_open_channel_participant_mute_list(open_channel_participant_mute_list_remove_request)
        print("The response of OpenChannelParticipantsModerationApi->remove_open_channel_participant_mute_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelParticipantsModerationApi->remove_open_channel_participant_mute_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_participant_mute_list_remove_request** | [**OpenChannelParticipantMuteListRemoveRequest**](OpenChannelParticipantMuteListRemoveRequest.md)|  | 


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

