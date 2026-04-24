# ncsdk.ChannelManagementApi

All requests use the primary/backup domains configured by the caller.

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_tag_to_channels**](ChannelManagementApi.md#add_tag_to_channels) | **POST** /v4/channel/tag/add | Add tag to channel
[**add_user_channel_tags**](ChannelManagementApi.md#add_user_channel_tags) | **POST** /v4/user/channel/tag/add | Add user channel tag
[**get_channel_attribute**](ChannelManagementApi.md#get_channel_attribute) | **POST** /v4/channel/attribute/get | Get channel attributes
[**get_channel_push_notification**](ChannelManagementApi.md#get_channel_push_notification) | **POST** /v4/channel/push/get | Get channel DND
[**get_channel_type_notification**](ChannelManagementApi.md#get_channel_type_notification) | **POST** /v4/channel-type/push/get | Get DND by channel type
[**list_channels_by_tag**](ChannelManagementApi.md#list_channels_by_tag) | **POST** /v4/channel/tag/list | Get channels by tag
[**list_user_channel_tags**](ChannelManagementApi.md#list_user_channel_tags) | **POST** /v4/user/channel/tag/list | List user channel tags
[**remove_tag_from_channels**](ChannelManagementApi.md#remove_tag_from_channels) | **POST** /v4/channel/tag/delete | Remove tag from channel
[**remove_user_channel_tags**](ChannelManagementApi.md#remove_user_channel_tags) | **POST** /v4/user/channel/tag/remove | Remove user channel tag
[**set_channel_pin**](ChannelManagementApi.md#set_channel_pin) | **POST** /v4/channel/pin/set | Pin a channel
[**set_channel_push_notification**](ChannelManagementApi.md#set_channel_push_notification) | **POST** /v4/channel/push/set | Set channel DND
[**set_channel_type_notification**](ChannelManagementApi.md#set_channel_type_notification) | **POST** /v4/channel-type/push/set | Set DND by channel type


# **add_tag_to_channels**
> CodeOnlyResponse add_tag_to_channels(channel_tag_add_request)

Add tag to channel

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import os
import ncsdk
from ncsdk.models.channel_tag_add_request import ChannelTagAddRequest
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
    api_instance = ncsdk.ChannelManagementApi(api_client)
    
    channel_tag_add_request = ncsdk.ChannelTagAddRequest() # ChannelTagAddRequest | 
    

    try:
        # Add tag to channel
        api_response = api_instance.add_tag_to_channels(channel_tag_add_request)
        print("The response of ChannelManagementApi->add_tag_to_channels:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChannelManagementApi->add_tag_to_channels: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channel_tag_add_request** | [**ChannelTagAddRequest**](ChannelTagAddRequest.md)|  | 


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

# **add_user_channel_tags**
> CodeOnlyResponse add_user_channel_tags(user_channel_tag_add_request)

Add user channel tag

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.user_channel_tag_add_request import UserChannelTagAddRequest
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
    api_instance = ncsdk.ChannelManagementApi(api_client)
    
    user_channel_tag_add_request = ncsdk.UserChannelTagAddRequest() # UserChannelTagAddRequest | 
    

    try:
        # Add user channel tag
        api_response = api_instance.add_user_channel_tags(user_channel_tag_add_request)
        print("The response of ChannelManagementApi->add_user_channel_tags:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChannelManagementApi->add_user_channel_tags: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_channel_tag_add_request** | [**UserChannelTagAddRequest**](UserChannelTagAddRequest.md)|  | 


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

# **get_channel_attribute**
> ChannelAttributeGetResponse get_channel_attribute(channel_attribute_get_request)

Get channel attributes

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.channel_attribute_get_request import ChannelAttributeGetRequest
from ncsdk.models.channel_attribute_get_response import ChannelAttributeGetResponse
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
    api_instance = ncsdk.ChannelManagementApi(api_client)
    
    channel_attribute_get_request = ncsdk.ChannelAttributeGetRequest() # ChannelAttributeGetRequest | 
    

    try:
        # Get channel attributes
        api_response = api_instance.get_channel_attribute(channel_attribute_get_request)
        print("The response of ChannelManagementApi->get_channel_attribute:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChannelManagementApi->get_channel_attribute: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channel_attribute_get_request** | [**ChannelAttributeGetRequest**](ChannelAttributeGetRequest.md)|  | 


### Return type

[**ChannelAttributeGetResponse**](ChannelAttributeGetResponse.md)

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

# **get_channel_push_notification**
> ChannelPushGetResponse get_channel_push_notification(channel_push_get_request)

Get channel DND

Rate limit: 100/sec. The public endpoint list currently publishes this capability as `/v4/channel/notification/get`.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.channel_push_get_request import ChannelPushGetRequest
from ncsdk.models.channel_push_get_response import ChannelPushGetResponse
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
    api_instance = ncsdk.ChannelManagementApi(api_client)
    
    channel_push_get_request = ncsdk.ChannelPushGetRequest() # ChannelPushGetRequest | 
    

    try:
        # Get channel DND
        api_response = api_instance.get_channel_push_notification(channel_push_get_request)
        print("The response of ChannelManagementApi->get_channel_push_notification:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChannelManagementApi->get_channel_push_notification: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channel_push_get_request** | [**ChannelPushGetRequest**](ChannelPushGetRequest.md)|  | 


### Return type

[**ChannelPushGetResponse**](ChannelPushGetResponse.md)

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

# **get_channel_type_notification**
> ChannelTypeNotificationGetResponse get_channel_type_notification(channel_type_notification_get_request)

Get DND by channel type

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.channel_type_notification_get_request import ChannelTypeNotificationGetRequest
from ncsdk.models.channel_type_notification_get_response import ChannelTypeNotificationGetResponse
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
    api_instance = ncsdk.ChannelManagementApi(api_client)
    
    channel_type_notification_get_request = ncsdk.ChannelTypeNotificationGetRequest() # ChannelTypeNotificationGetRequest | 
    

    try:
        # Get DND by channel type
        api_response = api_instance.get_channel_type_notification(channel_type_notification_get_request)
        print("The response of ChannelManagementApi->get_channel_type_notification:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChannelManagementApi->get_channel_type_notification: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channel_type_notification_get_request** | [**ChannelTypeNotificationGetRequest**](ChannelTypeNotificationGetRequest.md)|  | 


### Return type

[**ChannelTypeNotificationGetResponse**](ChannelTypeNotificationGetResponse.md)

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

# **list_channels_by_tag**
> ChannelTagListResponse list_channels_by_tag(channel_tag_list_request)

Get channels by tag

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.channel_tag_list_request import ChannelTagListRequest
from ncsdk.models.channel_tag_list_response import ChannelTagListResponse
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
    api_instance = ncsdk.ChannelManagementApi(api_client)
    
    channel_tag_list_request = ncsdk.ChannelTagListRequest() # ChannelTagListRequest | 
    

    try:
        # Get channels by tag
        api_response = api_instance.list_channels_by_tag(channel_tag_list_request)
        print("The response of ChannelManagementApi->list_channels_by_tag:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChannelManagementApi->list_channels_by_tag: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channel_tag_list_request** | [**ChannelTagListRequest**](ChannelTagListRequest.md)|  | 


### Return type

[**ChannelTagListResponse**](ChannelTagListResponse.md)

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

# **list_user_channel_tags**
> UserChannelTagListResponse list_user_channel_tags(user_channel_tag_list_request)

List user channel tags

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.user_channel_tag_list_request import UserChannelTagListRequest
from ncsdk.models.user_channel_tag_list_response import UserChannelTagListResponse
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
    api_instance = ncsdk.ChannelManagementApi(api_client)
    
    user_channel_tag_list_request = ncsdk.UserChannelTagListRequest() # UserChannelTagListRequest | 
    

    try:
        # List user channel tags
        api_response = api_instance.list_user_channel_tags(user_channel_tag_list_request)
        print("The response of ChannelManagementApi->list_user_channel_tags:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChannelManagementApi->list_user_channel_tags: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_channel_tag_list_request** | [**UserChannelTagListRequest**](UserChannelTagListRequest.md)|  | 


### Return type

[**UserChannelTagListResponse**](UserChannelTagListResponse.md)

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

# **remove_tag_from_channels**
> CodeOnlyResponse remove_tag_from_channels(channel_tag_remove_request)

Remove tag from channel

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.channel_tag_remove_request import ChannelTagRemoveRequest
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
    api_instance = ncsdk.ChannelManagementApi(api_client)
    
    channel_tag_remove_request = ncsdk.ChannelTagRemoveRequest() # ChannelTagRemoveRequest | 
    

    try:
        # Remove tag from channel
        api_response = api_instance.remove_tag_from_channels(channel_tag_remove_request)
        print("The response of ChannelManagementApi->remove_tag_from_channels:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChannelManagementApi->remove_tag_from_channels: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channel_tag_remove_request** | [**ChannelTagRemoveRequest**](ChannelTagRemoveRequest.md)|  | 


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

# **remove_user_channel_tags**
> CodeOnlyResponse remove_user_channel_tags(user_channel_tag_remove_request)

Remove user channel tag

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.user_channel_tag_remove_request import UserChannelTagRemoveRequest
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
    api_instance = ncsdk.ChannelManagementApi(api_client)
    
    user_channel_tag_remove_request = ncsdk.UserChannelTagRemoveRequest() # UserChannelTagRemoveRequest | 
    

    try:
        # Remove user channel tag
        api_response = api_instance.remove_user_channel_tags(user_channel_tag_remove_request)
        print("The response of ChannelManagementApi->remove_user_channel_tags:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChannelManagementApi->remove_user_channel_tags: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_channel_tag_remove_request** | [**UserChannelTagRemoveRequest**](UserChannelTagRemoveRequest.md)|  | 


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

# **set_channel_pin**
> CodeOnlyResponse set_channel_pin(channel_pin_set_request)

Pin a channel

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.channel_pin_set_request import ChannelPinSetRequest
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
    api_instance = ncsdk.ChannelManagementApi(api_client)
    
    channel_pin_set_request = ncsdk.ChannelPinSetRequest() # ChannelPinSetRequest | 
    

    try:
        # Pin a channel
        api_response = api_instance.set_channel_pin(channel_pin_set_request)
        print("The response of ChannelManagementApi->set_channel_pin:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChannelManagementApi->set_channel_pin: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channel_pin_set_request** | [**ChannelPinSetRequest**](ChannelPinSetRequest.md)|  | 


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

# **set_channel_push_notification**
> CodeOnlyResponse set_channel_push_notification(channel_push_set_request)

Set channel DND

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.channel_push_set_request import ChannelPushSetRequest
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
    api_instance = ncsdk.ChannelManagementApi(api_client)
    
    channel_push_set_request = ncsdk.ChannelPushSetRequest() # ChannelPushSetRequest | 
    

    try:
        # Set channel DND
        api_response = api_instance.set_channel_push_notification(channel_push_set_request)
        print("The response of ChannelManagementApi->set_channel_push_notification:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChannelManagementApi->set_channel_push_notification: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channel_push_set_request** | [**ChannelPushSetRequest**](ChannelPushSetRequest.md)|  | 


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

# **set_channel_type_notification**
> CodeOnlyResponse set_channel_type_notification(channel_type_notification_set_request)

Set DND by channel type

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.channel_type_notification_set_request import ChannelTypeNotificationSetRequest
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
    api_instance = ncsdk.ChannelManagementApi(api_client)
    
    channel_type_notification_set_request = ncsdk.ChannelTypeNotificationSetRequest() # ChannelTypeNotificationSetRequest | 
    

    try:
        # Set DND by channel type
        api_response = api_instance.set_channel_type_notification(channel_type_notification_set_request)
        print("The response of ChannelManagementApi->set_channel_type_notification:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChannelManagementApi->set_channel_type_notification: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channel_type_notification_set_request** | [**ChannelTypeNotificationSetRequest**](ChannelTypeNotificationSetRequest.md)|  | 


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

