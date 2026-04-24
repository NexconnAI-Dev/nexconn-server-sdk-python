# ncsdk.UserManagementApi

All requests use the primary/backup domains configured by the caller.

Method | HTTP request | Description
------------- | ------------- | -------------
[**ban_users**](UserManagementApi.md#ban_users) | **POST** /v4/user/ban | Ban a user
[**batch_get_user_tags**](UserManagementApi.md#batch_get_user_tags) | **POST** /v4/user/tag/batch/get | Get user tags
[**batch_set_user_tags**](UserManagementApi.md#batch_set_user_tags) | **POST** /v4/user/tag/batch/set | Batch set user tags
[**expire_access_token**](UserManagementApi.md#expire_access_token) | **POST** /v4/auth/access-token/expire | Expire an access token
[**get_user**](UserManagementApi.md#get_user) | **POST** /v4/user/get | Get user info
[**get_user_connection_status**](UserManagementApi.md#get_user_connection_status) | **POST** /v4/user/connection-status/get | Check user online status
[**issue_access_token**](UserManagementApi.md#issue_access_token) | **POST** /v4/auth/access-token/issue | Register a user
[**list_banned_users**](UserManagementApi.md#list_banned_users) | **POST** /v4/user/ban/list | List banned users
[**list_channel_type_mute**](UserManagementApi.md#list_channel_type_mute) | **POST** /v4/channel-type/mute/list | List muted direct channel users
[**list_soft_deleted_users**](UserManagementApi.md#list_soft_deleted_users) | **POST** /v4/user/soft-deleted/list | Query soft-deleted users
[**restore_users**](UserManagementApi.md#restore_users) | **POST** /v4/user/restore | Restore a user
[**set_channel_type_mute**](UserManagementApi.md#set_channel_type_mute) | **POST** /v4/channel-type/mute/set | Mute a user in direct channels
[**soft_delete_users**](UserManagementApi.md#soft_delete_users) | **POST** /v4/user/soft-delete | Soft-delete a user
[**unban_users**](UserManagementApi.md#unban_users) | **POST** /v4/user/unban | Unban a user
[**update_user**](UserManagementApi.md#update_user) | **POST** /v4/user/update | Update user info


# **ban_users**
> CodeOnlyResponse ban_users(user_ban_request)

Ban a user

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import os
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.user_ban_request import UserBanRequest
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
    api_instance = ncsdk.UserManagementApi(api_client)
    
    user_ban_request = ncsdk.UserBanRequest() # UserBanRequest | 
    

    try:
        # Ban a user
        api_response = api_instance.ban_users(user_ban_request)
        print("The response of UserManagementApi->ban_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserManagementApi->ban_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_ban_request** | [**UserBanRequest**](UserBanRequest.md)|  | 


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

# **batch_get_user_tags**
> UserTagBatchGetResponse batch_get_user_tags(user_tag_batch_get_request)

Get user tags

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.user_tag_batch_get_request import UserTagBatchGetRequest
from ncsdk.models.user_tag_batch_get_response import UserTagBatchGetResponse
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
    api_instance = ncsdk.UserManagementApi(api_client)
    
    user_tag_batch_get_request = ncsdk.UserTagBatchGetRequest() # UserTagBatchGetRequest | 
    

    try:
        # Get user tags
        api_response = api_instance.batch_get_user_tags(user_tag_batch_get_request)
        print("The response of UserManagementApi->batch_get_user_tags:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserManagementApi->batch_get_user_tags: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_tag_batch_get_request** | [**UserTagBatchGetRequest**](UserTagBatchGetRequest.md)|  | 


### Return type

[**UserTagBatchGetResponse**](UserTagBatchGetResponse.md)

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

# **batch_set_user_tags**
> CodeOnlyResponse batch_set_user_tags(user_tag_batch_set_request)

Batch set user tags

Rate limit: 10/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.user_tag_batch_set_request import UserTagBatchSetRequest
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
    api_instance = ncsdk.UserManagementApi(api_client)
    
    user_tag_batch_set_request = ncsdk.UserTagBatchSetRequest() # UserTagBatchSetRequest | 
    

    try:
        # Batch set user tags
        api_response = api_instance.batch_set_user_tags(user_tag_batch_set_request)
        print("The response of UserManagementApi->batch_set_user_tags:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserManagementApi->batch_set_user_tags: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_tag_batch_set_request** | [**UserTagBatchSetRequest**](UserTagBatchSetRequest.md)|  | 


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

# **expire_access_token**
> CodeOnlyResponse expire_access_token(access_token_expire_request)

Expire an access token

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.access_token_expire_request import AccessTokenExpireRequest
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
    api_instance = ncsdk.UserManagementApi(api_client)
    
    access_token_expire_request = ncsdk.AccessTokenExpireRequest() # AccessTokenExpireRequest | 
    

    try:
        # Expire an access token
        api_response = api_instance.expire_access_token(access_token_expire_request)
        print("The response of UserManagementApi->expire_access_token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserManagementApi->expire_access_token: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **access_token_expire_request** | [**AccessTokenExpireRequest**](AccessTokenExpireRequest.md)|  | 


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

# **get_user**
> UserGetResponse get_user(user_get_request)

Get user info

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.user_get_request import UserGetRequest
from ncsdk.models.user_get_response import UserGetResponse
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
    api_instance = ncsdk.UserManagementApi(api_client)
    
    user_get_request = ncsdk.UserGetRequest() # UserGetRequest | 
    

    try:
        # Get user info
        api_response = api_instance.get_user(user_get_request)
        print("The response of UserManagementApi->get_user:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserManagementApi->get_user: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_get_request** | [**UserGetRequest**](UserGetRequest.md)|  | 


### Return type

[**UserGetResponse**](UserGetResponse.md)

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

# **get_user_connection_status**
> UserConnectionStatusResponse get_user_connection_status(user_connection_status_request)

Check user online status

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.user_connection_status_request import UserConnectionStatusRequest
from ncsdk.models.user_connection_status_response import UserConnectionStatusResponse
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
    api_instance = ncsdk.UserManagementApi(api_client)
    
    user_connection_status_request = ncsdk.UserConnectionStatusRequest() # UserConnectionStatusRequest | 
    

    try:
        # Check user online status
        api_response = api_instance.get_user_connection_status(user_connection_status_request)
        print("The response of UserManagementApi->get_user_connection_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserManagementApi->get_user_connection_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_connection_status_request** | [**UserConnectionStatusRequest**](UserConnectionStatusRequest.md)|  | 


### Return type

[**UserConnectionStatusResponse**](UserConnectionStatusResponse.md)

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

# **issue_access_token**
> AccessTokenIssueResponse issue_access_token(access_token_issue_request)

Register a user

Rate limit: 200/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.access_token_issue_request import AccessTokenIssueRequest
from ncsdk.models.access_token_issue_response import AccessTokenIssueResponse
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
    api_instance = ncsdk.UserManagementApi(api_client)
    
    access_token_issue_request = ncsdk.AccessTokenIssueRequest() # AccessTokenIssueRequest | 
    

    try:
        # Register a user
        api_response = api_instance.issue_access_token(access_token_issue_request)
        print("The response of UserManagementApi->issue_access_token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserManagementApi->issue_access_token: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **access_token_issue_request** | [**AccessTokenIssueRequest**](AccessTokenIssueRequest.md)|  | 


### Return type

[**AccessTokenIssueResponse**](AccessTokenIssueResponse.md)

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

# **list_banned_users**
> UserBanListResponse list_banned_users(user_ban_list_request)

List banned users

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.user_ban_list_request import UserBanListRequest
from ncsdk.models.user_ban_list_response import UserBanListResponse
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
    api_instance = ncsdk.UserManagementApi(api_client)
    
    user_ban_list_request = ncsdk.UserBanListRequest() # UserBanListRequest | 
    

    try:
        # List banned users
        api_response = api_instance.list_banned_users(user_ban_list_request)
        print("The response of UserManagementApi->list_banned_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserManagementApi->list_banned_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_ban_list_request** | [**UserBanListRequest**](UserBanListRequest.md)|  | 


### Return type

[**UserBanListResponse**](UserBanListResponse.md)

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

# **list_channel_type_mute**
> ChannelTypeMuteListResponse list_channel_type_mute(channel_type_mute_list_request)

List muted direct channel users

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.channel_type_mute_list_request import ChannelTypeMuteListRequest
from ncsdk.models.channel_type_mute_list_response import ChannelTypeMuteListResponse
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
    api_instance = ncsdk.UserManagementApi(api_client)
    
    channel_type_mute_list_request = ncsdk.ChannelTypeMuteListRequest() # ChannelTypeMuteListRequest | 
    

    try:
        # List muted direct channel users
        api_response = api_instance.list_channel_type_mute(channel_type_mute_list_request)
        print("The response of UserManagementApi->list_channel_type_mute:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserManagementApi->list_channel_type_mute: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channel_type_mute_list_request** | [**ChannelTypeMuteListRequest**](ChannelTypeMuteListRequest.md)|  | 


### Return type

[**ChannelTypeMuteListResponse**](ChannelTypeMuteListResponse.md)

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

# **list_soft_deleted_users**
> UserSoftDeletedListResponse list_soft_deleted_users(user_soft_deleted_list_request)

Query soft-deleted users

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.user_soft_deleted_list_request import UserSoftDeletedListRequest
from ncsdk.models.user_soft_deleted_list_response import UserSoftDeletedListResponse
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
    api_instance = ncsdk.UserManagementApi(api_client)
    
    user_soft_deleted_list_request = ncsdk.UserSoftDeletedListRequest() # UserSoftDeletedListRequest | 
    

    try:
        # Query soft-deleted users
        api_response = api_instance.list_soft_deleted_users(user_soft_deleted_list_request)
        print("The response of UserManagementApi->list_soft_deleted_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserManagementApi->list_soft_deleted_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_soft_deleted_list_request** | [**UserSoftDeletedListRequest**](UserSoftDeletedListRequest.md)|  | 


### Return type

[**UserSoftDeletedListResponse**](UserSoftDeletedListResponse.md)

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

# **restore_users**
> UserOperationResponse restore_users(user_ids_max100_request)

Restore a user

Rate limit: 100 users/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.user_ids_max100_request import UserIdsMax100Request
from ncsdk.models.user_operation_response import UserOperationResponse
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
    api_instance = ncsdk.UserManagementApi(api_client)
    
    user_ids_max100_request = ncsdk.UserIdsMax100Request() # UserIdsMax100Request | 
    

    try:
        # Restore a user
        api_response = api_instance.restore_users(user_ids_max100_request)
        print("The response of UserManagementApi->restore_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserManagementApi->restore_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_ids_max100_request** | [**UserIdsMax100Request**](UserIdsMax100Request.md)|  | 


### Return type

[**UserOperationResponse**](UserOperationResponse.md)

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

# **set_channel_type_mute**
> CodeOnlyResponse set_channel_type_mute(channel_type_mute_set_request)

Mute a user in direct channels

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.channel_type_mute_set_request import ChannelTypeMuteSetRequest
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
    api_instance = ncsdk.UserManagementApi(api_client)
    
    channel_type_mute_set_request = ncsdk.ChannelTypeMuteSetRequest() # ChannelTypeMuteSetRequest | 
    

    try:
        # Mute a user in direct channels
        api_response = api_instance.set_channel_type_mute(channel_type_mute_set_request)
        print("The response of UserManagementApi->set_channel_type_mute:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserManagementApi->set_channel_type_mute: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **channel_type_mute_set_request** | [**ChannelTypeMuteSetRequest**](ChannelTypeMuteSetRequest.md)|  | 


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

# **soft_delete_users**
> UserOperationResponse soft_delete_users(user_ids_max100_request)

Soft-delete a user

Rate limit: 100 users/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.user_ids_max100_request import UserIdsMax100Request
from ncsdk.models.user_operation_response import UserOperationResponse
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
    api_instance = ncsdk.UserManagementApi(api_client)
    
    user_ids_max100_request = ncsdk.UserIdsMax100Request() # UserIdsMax100Request | 
    

    try:
        # Soft-delete a user
        api_response = api_instance.soft_delete_users(user_ids_max100_request)
        print("The response of UserManagementApi->soft_delete_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserManagementApi->soft_delete_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_ids_max100_request** | [**UserIdsMax100Request**](UserIdsMax100Request.md)|  | 


### Return type

[**UserOperationResponse**](UserOperationResponse.md)

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

# **unban_users**
> CodeOnlyResponse unban_users(user_ids_max20_request)

Unban a user

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.user_ids_max20_request import UserIdsMax20Request
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
    api_instance = ncsdk.UserManagementApi(api_client)
    
    user_ids_max20_request = ncsdk.UserIdsMax20Request() # UserIdsMax20Request | 
    

    try:
        # Unban a user
        api_response = api_instance.unban_users(user_ids_max20_request)
        print("The response of UserManagementApi->unban_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserManagementApi->unban_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_ids_max20_request** | [**UserIdsMax20Request**](UserIdsMax20Request.md)|  | 


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

# **update_user**
> CodeOnlyResponse update_user(user_update_request)

Update user info

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.user_update_request import UserUpdateRequest
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
    api_instance = ncsdk.UserManagementApi(api_client)
    
    user_update_request = ncsdk.UserUpdateRequest() # UserUpdateRequest | 
    

    try:
        # Update user info
        api_response = api_instance.update_user(user_update_request)
        print("The response of UserManagementApi->update_user:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserManagementApi->update_user: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_update_request** | [**UserUpdateRequest**](UserUpdateRequest.md)|  | 


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

