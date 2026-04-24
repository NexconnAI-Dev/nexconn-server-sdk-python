# ncsdk.GroupChannelManagementApi

All requests use the primary/backup domains configured by the caller.

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_group_channel_admins**](GroupChannelManagementApi.md#add_group_channel_admins) | **POST** /v4/group-channel/admin/add | Add group admins
[**add_group_channel_member_favorites**](GroupChannelManagementApi.md#add_group_channel_member_favorites) | **POST** /v4/group-channel/member/favorites/add | Add favorite group members
[**batch_get_group_channel_members**](GroupChannelManagementApi.md#batch_get_group_channel_members) | **POST** /v4/group-channel/member/batch/get | Get specific group members
[**batch_get_group_channel_profiles**](GroupChannelManagementApi.md#batch_get_group_channel_profiles) | **POST** /v4/group-channel/profile/list | List group profiles
[**create_group_channel**](GroupChannelManagementApi.md#create_group_channel) | **POST** /v4/group-channel/create | Create a group
[**delete_group_channel_alias**](GroupChannelManagementApi.md#delete_group_channel_alias) | **POST** /v4/group-channel/alias/delete | Delete group alias
[**dismiss_group_channel**](GroupChannelManagementApi.md#dismiss_group_channel) | **POST** /v4/group-channel/dismiss | Dismiss a group
[**get_group_channel_alias**](GroupChannelManagementApi.md#get_group_channel_alias) | **POST** /v4/group-channel/alias/get | Get group alias
[**join_group_channel**](GroupChannelManagementApi.md#join_group_channel) | **POST** /v4/group-channel/join | Join a group
[**kick_user_from_all_group_channels**](GroupChannelManagementApi.md#kick_user_from_all_group_channels) | **POST** /v4/group-channel/member/kickout-all | Remove a user from all groups
[**list_group_channel_member_favorites**](GroupChannelManagementApi.md#list_group_channel_member_favorites) | **POST** /v4/group-channel/member/favorites/list | List favorite group members
[**list_group_channel_members**](GroupChannelManagementApi.md#list_group_channel_members) | **POST** /v4/group-channel/member/list | Query group members
[**list_group_channels**](GroupChannelManagementApi.md#list_group_channels) | **POST** /v4/group-channel/list | List group channels
[**list_user_joined_group_channels**](GroupChannelManagementApi.md#list_user_joined_group_channels) | **POST** /v4/group-channel/joined/list | Query user&#39;s groups
[**quit_group_channel**](GroupChannelManagementApi.md#quit_group_channel) | **POST** /v4/group-channel/leave | Leave a group
[**remove_group_channel_admins**](GroupChannelManagementApi.md#remove_group_channel_admins) | **POST** /v4/group-channel/admin/remove | Remove group admins
[**remove_group_channel_member_favorites**](GroupChannelManagementApi.md#remove_group_channel_member_favorites) | **POST** /v4/group-channel/member/favorites/remove | Remove favorite group members
[**set_group_channel_alias**](GroupChannelManagementApi.md#set_group_channel_alias) | **POST** /v4/group-channel/alias/set | Set group alias
[**set_group_channel_member**](GroupChannelManagementApi.md#set_group_channel_member) | **POST** /v4/group-channel/member/set | Set group member profile
[**transfer_group_channel_owner**](GroupChannelManagementApi.md#transfer_group_channel_owner) | **POST** /v4/group-channel/transfer/owner | Transfer group ownership
[**update_group_channel_profile**](GroupChannelManagementApi.md#update_group_channel_profile) | **POST** /v4/group-channel/profile/update | Update group info


# **add_group_channel_admins**
> CodeOnlyResponse add_group_channel_admins(group_channel_admin_users_request)

Add group admins

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import os
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_admin_users_request import GroupChannelAdminUsersRequest
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_admin_users_request = ncsdk.GroupChannelAdminUsersRequest() # GroupChannelAdminUsersRequest | 
    

    try:
        # Add group admins
        api_response = api_instance.add_group_channel_admins(group_channel_admin_users_request)
        print("The response of GroupChannelManagementApi->add_group_channel_admins:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->add_group_channel_admins: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_admin_users_request** | [**GroupChannelAdminUsersRequest**](GroupChannelAdminUsersRequest.md)|  | 


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

# **add_group_channel_member_favorites**
> CodeOnlyResponse add_group_channel_member_favorites(group_channel_member_favorites_update_request)

Add favorite group members

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_member_favorites_update_request import GroupChannelMemberFavoritesUpdateRequest
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_member_favorites_update_request = ncsdk.GroupChannelMemberFavoritesUpdateRequest() # GroupChannelMemberFavoritesUpdateRequest | 
    

    try:
        # Add favorite group members
        api_response = api_instance.add_group_channel_member_favorites(group_channel_member_favorites_update_request)
        print("The response of GroupChannelManagementApi->add_group_channel_member_favorites:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->add_group_channel_member_favorites: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_member_favorites_update_request** | [**GroupChannelMemberFavoritesUpdateRequest**](GroupChannelMemberFavoritesUpdateRequest.md)|  | 


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

# **batch_get_group_channel_members**
> GroupChannelMemberBatchGetResponse batch_get_group_channel_members(group_channel_member_batch_get_request)

Get specific group members

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.group_channel_member_batch_get_request import GroupChannelMemberBatchGetRequest
from ncsdk.models.group_channel_member_batch_get_response import GroupChannelMemberBatchGetResponse
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_member_batch_get_request = ncsdk.GroupChannelMemberBatchGetRequest() # GroupChannelMemberBatchGetRequest | 
    

    try:
        # Get specific group members
        api_response = api_instance.batch_get_group_channel_members(group_channel_member_batch_get_request)
        print("The response of GroupChannelManagementApi->batch_get_group_channel_members:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->batch_get_group_channel_members: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_member_batch_get_request** | [**GroupChannelMemberBatchGetRequest**](GroupChannelMemberBatchGetRequest.md)|  | 


### Return type

[**GroupChannelMemberBatchGetResponse**](GroupChannelMemberBatchGetResponse.md)

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

# **batch_get_group_channel_profiles**
> GroupChannelProfileListResponse batch_get_group_channel_profiles(group_channel_profile_list_request)

List group profiles

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.group_channel_profile_list_request import GroupChannelProfileListRequest
from ncsdk.models.group_channel_profile_list_response import GroupChannelProfileListResponse
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_profile_list_request = ncsdk.GroupChannelProfileListRequest() # GroupChannelProfileListRequest | 
    

    try:
        # List group profiles
        api_response = api_instance.batch_get_group_channel_profiles(group_channel_profile_list_request)
        print("The response of GroupChannelManagementApi->batch_get_group_channel_profiles:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->batch_get_group_channel_profiles: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_profile_list_request** | [**GroupChannelProfileListRequest**](GroupChannelProfileListRequest.md)|  | 


### Return type

[**GroupChannelProfileListResponse**](GroupChannelProfileListResponse.md)

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

# **create_group_channel**
> CodeOnlyResponse create_group_channel(group_channel_create_request)

Create a group

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_create_request import GroupChannelCreateRequest
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_create_request = ncsdk.GroupChannelCreateRequest() # GroupChannelCreateRequest | 
    

    try:
        # Create a group
        api_response = api_instance.create_group_channel(group_channel_create_request)
        print("The response of GroupChannelManagementApi->create_group_channel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->create_group_channel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_create_request** | [**GroupChannelCreateRequest**](GroupChannelCreateRequest.md)|  | 


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

# **delete_group_channel_alias**
> CodeOnlyResponse delete_group_channel_alias(group_channel_alias_get_request)

Delete group alias

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_alias_get_request import GroupChannelAliasGetRequest
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_alias_get_request = ncsdk.GroupChannelAliasGetRequest() # GroupChannelAliasGetRequest | 
    

    try:
        # Delete group alias
        api_response = api_instance.delete_group_channel_alias(group_channel_alias_get_request)
        print("The response of GroupChannelManagementApi->delete_group_channel_alias:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->delete_group_channel_alias: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_alias_get_request** | [**GroupChannelAliasGetRequest**](GroupChannelAliasGetRequest.md)|  | 


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

# **dismiss_group_channel**
> CodeOnlyResponse dismiss_group_channel(group_channel_dismiss_request)

Dismiss a group

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_dismiss_request import GroupChannelDismissRequest
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_dismiss_request = ncsdk.GroupChannelDismissRequest() # GroupChannelDismissRequest | 
    

    try:
        # Dismiss a group
        api_response = api_instance.dismiss_group_channel(group_channel_dismiss_request)
        print("The response of GroupChannelManagementApi->dismiss_group_channel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->dismiss_group_channel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_dismiss_request** | [**GroupChannelDismissRequest**](GroupChannelDismissRequest.md)|  | 


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

# **get_group_channel_alias**
> GroupChannelAliasGetResponse get_group_channel_alias(group_channel_alias_get_request)

Get group alias

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.group_channel_alias_get_request import GroupChannelAliasGetRequest
from ncsdk.models.group_channel_alias_get_response import GroupChannelAliasGetResponse
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_alias_get_request = ncsdk.GroupChannelAliasGetRequest() # GroupChannelAliasGetRequest | 
    

    try:
        # Get group alias
        api_response = api_instance.get_group_channel_alias(group_channel_alias_get_request)
        print("The response of GroupChannelManagementApi->get_group_channel_alias:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->get_group_channel_alias: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_alias_get_request** | [**GroupChannelAliasGetRequest**](GroupChannelAliasGetRequest.md)|  | 


### Return type

[**GroupChannelAliasGetResponse**](GroupChannelAliasGetResponse.md)

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

# **join_group_channel**
> GroupChannelJoinResponse join_group_channel(group_channel_join_request)

Join a group

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.group_channel_join_request import GroupChannelJoinRequest
from ncsdk.models.group_channel_join_response import GroupChannelJoinResponse
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_join_request = ncsdk.GroupChannelJoinRequest() # GroupChannelJoinRequest | 
    

    try:
        # Join a group
        api_response = api_instance.join_group_channel(group_channel_join_request)
        print("The response of GroupChannelManagementApi->join_group_channel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->join_group_channel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_join_request** | [**GroupChannelJoinRequest**](GroupChannelJoinRequest.md)|  | 


### Return type

[**GroupChannelJoinResponse**](GroupChannelJoinResponse.md)

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

# **kick_user_from_all_group_channels**
> CodeOnlyResponse kick_user_from_all_group_channels(group_channel_kick_user_from_all_request)

Remove a user from all groups

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_kick_user_from_all_request import GroupChannelKickUserFromAllRequest
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_kick_user_from_all_request = ncsdk.GroupChannelKickUserFromAllRequest() # GroupChannelKickUserFromAllRequest | 
    

    try:
        # Remove a user from all groups
        api_response = api_instance.kick_user_from_all_group_channels(group_channel_kick_user_from_all_request)
        print("The response of GroupChannelManagementApi->kick_user_from_all_group_channels:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->kick_user_from_all_group_channels: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_kick_user_from_all_request** | [**GroupChannelKickUserFromAllRequest**](GroupChannelKickUserFromAllRequest.md)|  | 


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

# **list_group_channel_member_favorites**
> GroupChannelMemberFavoritesListResponse list_group_channel_member_favorites(group_channel_member_favorites_list_request)

List favorite group members

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.group_channel_member_favorites_list_request import GroupChannelMemberFavoritesListRequest
from ncsdk.models.group_channel_member_favorites_list_response import GroupChannelMemberFavoritesListResponse
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_member_favorites_list_request = ncsdk.GroupChannelMemberFavoritesListRequest() # GroupChannelMemberFavoritesListRequest | 
    

    try:
        # List favorite group members
        api_response = api_instance.list_group_channel_member_favorites(group_channel_member_favorites_list_request)
        print("The response of GroupChannelManagementApi->list_group_channel_member_favorites:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->list_group_channel_member_favorites: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_member_favorites_list_request** | [**GroupChannelMemberFavoritesListRequest**](GroupChannelMemberFavoritesListRequest.md)|  | 


### Return type

[**GroupChannelMemberFavoritesListResponse**](GroupChannelMemberFavoritesListResponse.md)

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

# **list_group_channel_members**
> GroupChannelMemberListResponse list_group_channel_members(group_channel_member_list_request)

Query group members

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.group_channel_member_list_request import GroupChannelMemberListRequest
from ncsdk.models.group_channel_member_list_response import GroupChannelMemberListResponse
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_member_list_request = ncsdk.GroupChannelMemberListRequest() # GroupChannelMemberListRequest | 
    

    try:
        # Query group members
        api_response = api_instance.list_group_channel_members(group_channel_member_list_request)
        print("The response of GroupChannelManagementApi->list_group_channel_members:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->list_group_channel_members: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_member_list_request** | [**GroupChannelMemberListRequest**](GroupChannelMemberListRequest.md)|  | 


### Return type

[**GroupChannelMemberListResponse**](GroupChannelMemberListResponse.md)

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

# **list_group_channels**
> GroupChannelListResponse list_group_channels(group_channel_list_request)

List group channels

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.group_channel_list_request import GroupChannelListRequest
from ncsdk.models.group_channel_list_response import GroupChannelListResponse
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_list_request = ncsdk.GroupChannelListRequest() # GroupChannelListRequest | 
    

    try:
        # List group channels
        api_response = api_instance.list_group_channels(group_channel_list_request)
        print("The response of GroupChannelManagementApi->list_group_channels:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->list_group_channels: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_list_request** | [**GroupChannelListRequest**](GroupChannelListRequest.md)|  | 


### Return type

[**GroupChannelListResponse**](GroupChannelListResponse.md)

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

# **list_user_joined_group_channels**
> GroupChannelJoinedListResponse list_user_joined_group_channels(group_channel_joined_list_request)

Query user's groups

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.group_channel_joined_list_request import GroupChannelJoinedListRequest
from ncsdk.models.group_channel_joined_list_response import GroupChannelJoinedListResponse
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_joined_list_request = ncsdk.GroupChannelJoinedListRequest() # GroupChannelJoinedListRequest | 
    

    try:
        # Query user's groups
        api_response = api_instance.list_user_joined_group_channels(group_channel_joined_list_request)
        print("The response of GroupChannelManagementApi->list_user_joined_group_channels:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->list_user_joined_group_channels: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_joined_list_request** | [**GroupChannelJoinedListRequest**](GroupChannelJoinedListRequest.md)|  | 


### Return type

[**GroupChannelJoinedListResponse**](GroupChannelJoinedListResponse.md)

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

# **quit_group_channel**
> CodeOnlyResponse quit_group_channel(group_channel_quit_request)

Leave a group

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_quit_request import GroupChannelQuitRequest
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_quit_request = ncsdk.GroupChannelQuitRequest() # GroupChannelQuitRequest | 
    

    try:
        # Leave a group
        api_response = api_instance.quit_group_channel(group_channel_quit_request)
        print("The response of GroupChannelManagementApi->quit_group_channel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->quit_group_channel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_quit_request** | [**GroupChannelQuitRequest**](GroupChannelQuitRequest.md)|  | 


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

# **remove_group_channel_admins**
> CodeOnlyResponse remove_group_channel_admins(group_channel_admin_users_request)

Remove group admins

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_admin_users_request import GroupChannelAdminUsersRequest
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_admin_users_request = ncsdk.GroupChannelAdminUsersRequest() # GroupChannelAdminUsersRequest | 
    

    try:
        # Remove group admins
        api_response = api_instance.remove_group_channel_admins(group_channel_admin_users_request)
        print("The response of GroupChannelManagementApi->remove_group_channel_admins:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->remove_group_channel_admins: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_admin_users_request** | [**GroupChannelAdminUsersRequest**](GroupChannelAdminUsersRequest.md)|  | 


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

# **remove_group_channel_member_favorites**
> CodeOnlyResponse remove_group_channel_member_favorites(group_channel_member_favorites_update_request)

Remove favorite group members

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_member_favorites_update_request import GroupChannelMemberFavoritesUpdateRequest
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_member_favorites_update_request = ncsdk.GroupChannelMemberFavoritesUpdateRequest() # GroupChannelMemberFavoritesUpdateRequest | 
    

    try:
        # Remove favorite group members
        api_response = api_instance.remove_group_channel_member_favorites(group_channel_member_favorites_update_request)
        print("The response of GroupChannelManagementApi->remove_group_channel_member_favorites:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->remove_group_channel_member_favorites: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_member_favorites_update_request** | [**GroupChannelMemberFavoritesUpdateRequest**](GroupChannelMemberFavoritesUpdateRequest.md)|  | 


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

# **set_group_channel_alias**
> CodeOnlyResponse set_group_channel_alias(group_channel_alias_set_request)

Set group alias

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_alias_set_request import GroupChannelAliasSetRequest
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_alias_set_request = ncsdk.GroupChannelAliasSetRequest() # GroupChannelAliasSetRequest | 
    

    try:
        # Set group alias
        api_response = api_instance.set_group_channel_alias(group_channel_alias_set_request)
        print("The response of GroupChannelManagementApi->set_group_channel_alias:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->set_group_channel_alias: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_alias_set_request** | [**GroupChannelAliasSetRequest**](GroupChannelAliasSetRequest.md)|  | 


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

# **set_group_channel_member**
> CodeOnlyResponse set_group_channel_member(group_channel_member_set_request)

Set group member profile

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_member_set_request import GroupChannelMemberSetRequest
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_member_set_request = ncsdk.GroupChannelMemberSetRequest() # GroupChannelMemberSetRequest | 
    

    try:
        # Set group member profile
        api_response = api_instance.set_group_channel_member(group_channel_member_set_request)
        print("The response of GroupChannelManagementApi->set_group_channel_member:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->set_group_channel_member: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_member_set_request** | [**GroupChannelMemberSetRequest**](GroupChannelMemberSetRequest.md)|  | 


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

# **transfer_group_channel_owner**
> CodeOnlyResponse transfer_group_channel_owner(group_channel_transfer_owner_request)

Transfer group ownership

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_transfer_owner_request import GroupChannelTransferOwnerRequest
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_transfer_owner_request = ncsdk.GroupChannelTransferOwnerRequest() # GroupChannelTransferOwnerRequest | 
    

    try:
        # Transfer group ownership
        api_response = api_instance.transfer_group_channel_owner(group_channel_transfer_owner_request)
        print("The response of GroupChannelManagementApi->transfer_group_channel_owner:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->transfer_group_channel_owner: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_transfer_owner_request** | [**GroupChannelTransferOwnerRequest**](GroupChannelTransferOwnerRequest.md)|  | 


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

# **update_group_channel_profile**
> CodeOnlyResponse update_group_channel_profile(group_channel_profile_update_request)

Update group info

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.group_channel_profile_update_request import GroupChannelProfileUpdateRequest
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
    api_instance = ncsdk.GroupChannelManagementApi(api_client)
    
    group_channel_profile_update_request = ncsdk.GroupChannelProfileUpdateRequest() # GroupChannelProfileUpdateRequest | 
    

    try:
        # Update group info
        api_response = api_instance.update_group_channel_profile(group_channel_profile_update_request)
        print("The response of GroupChannelManagementApi->update_group_channel_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling GroupChannelManagementApi->update_group_channel_profile: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **group_channel_profile_update_request** | [**GroupChannelProfileUpdateRequest**](GroupChannelProfileUpdateRequest.md)|  | 


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

