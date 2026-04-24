# ncsdk.CommunityChannelManagementApi

All requests use the primary/backup domains configured by the caller.

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_community_channel_user_group_users**](CommunityChannelManagementApi.md#add_community_channel_user_group_users) | **POST** /v4/community-channel/user-group/user/add | Add community channel user group users
[**add_community_channel_user_groups**](CommunityChannelManagementApi.md#add_community_channel_user_groups) | **POST** /v4/community-channel/user-group/add | Add community channel user groups
[**add_private_subchannel_members**](CommunityChannelManagementApi.md#add_private_subchannel_members) | **POST** /v4/community-channel/private-subchannel/member/add | Add private subchannel members
[**bind_community_channel_user_group**](CommunityChannelManagementApi.md#bind_community_channel_user_group) | **POST** /v4/community-channel/channel/user-group/bind | Bind community channel user group
[**check_community_channel_member_exist**](CommunityChannelManagementApi.md#check_community_channel_member_exist) | **POST** /v4/community-channel/member/exist | Check community channel member exist
[**create_community_channel**](CommunityChannelManagementApi.md#create_community_channel) | **POST** /v4/community-channel/create | Create community channel
[**create_community_subchannel**](CommunityChannelManagementApi.md#create_community_subchannel) | **POST** /v4/community-channel/subchannel/create | Create community subchannel
[**delete_community_subchannel**](CommunityChannelManagementApi.md#delete_community_subchannel) | **POST** /v4/community-channel/subchannel/delete | Delete community subchannel
[**dismiss_community_channel**](CommunityChannelManagementApi.md#dismiss_community_channel) | **POST** /v4/community-channel/dismiss | Dismiss community channel
[**join_community_channel**](CommunityChannelManagementApi.md#join_community_channel) | **POST** /v4/community-channel/join | Join community channel
[**list_community_channel_history_messages**](CommunityChannelManagementApi.md#list_community_channel_history_messages) | **POST** /v4/community-channel/history-message/list | List community-channel history messages
[**list_community_channel_subchannel_user_groups**](CommunityChannelManagementApi.md#list_community_channel_subchannel_user_groups) | **POST** /v4/community-channel/channel/user-group/list | List community channel subchannel user groups
[**list_community_channel_user_group_subchannels**](CommunityChannelManagementApi.md#list_community_channel_user_group_subchannels) | **POST** /v4/community-channel/user-group/subchannel/list | List community channel user group subchannels
[**list_community_channel_user_groups**](CommunityChannelManagementApi.md#list_community_channel_user_groups) | **POST** /v4/community-channel/user-group/list | List community channel user groups
[**list_community_channel_user_user_groups**](CommunityChannelManagementApi.md#list_community_channel_user_user_groups) | **POST** /v4/community-channel/user/user-group/list | List community channel user user groups
[**list_community_subchannels**](CommunityChannelManagementApi.md#list_community_subchannels) | **POST** /v4/community-channel/subchannel/list | List community subchannels
[**list_community_user_subchannels**](CommunityChannelManagementApi.md#list_community_user_subchannels) | **POST** /v4/community-channel/user/subchannel/list | List community user subchannels
[**list_private_subchannel_members**](CommunityChannelManagementApi.md#list_private_subchannel_members) | **POST** /v4/community-channel/private-subchannel/member/list | List private subchannel members
[**quit_community_channel**](CommunityChannelManagementApi.md#quit_community_channel) | **POST** /v4/community-channel/leave | Leave community channel
[**remove_community_channel_user_group_users**](CommunityChannelManagementApi.md#remove_community_channel_user_group_users) | **POST** /v4/community-channel/user-group/user/remove | Remove community channel user group users
[**remove_community_channel_user_groups**](CommunityChannelManagementApi.md#remove_community_channel_user_groups) | **POST** /v4/community-channel/user-group/remove | Delete community channel user groups
[**remove_private_subchannel_members**](CommunityChannelManagementApi.md#remove_private_subchannel_members) | **POST** /v4/community-channel/private-subchannel/member/remove | Remove private subchannel members
[**unbind_community_channel_user_group**](CommunityChannelManagementApi.md#unbind_community_channel_user_group) | **POST** /v4/community-channel/channel/user-group/unbind | Unbind community channel user group
[**update_community_channel_info**](CommunityChannelManagementApi.md#update_community_channel_info) | **POST** /v4/community-channel/update | Update community channel info
[**update_community_subchannel_type**](CommunityChannelManagementApi.md#update_community_subchannel_type) | **POST** /v4/community-channel/subchannel-type/update | Update community subchannel type


# **add_community_channel_user_group_users**
> CodeOnlyResponse add_community_channel_user_group_users(community_channel_user_group_users_request)

Add community channel user group users

### Example

* Api Key Authentication (NexconnSignature):

```python
import os
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_user_group_users_request import CommunityChannelUserGroupUsersRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_user_group_users_request = ncsdk.CommunityChannelUserGroupUsersRequest() # CommunityChannelUserGroupUsersRequest | 
    

    try:
        # Add community channel user group users
        api_response = api_instance.add_community_channel_user_group_users(community_channel_user_group_users_request)
        print("The response of CommunityChannelManagementApi->add_community_channel_user_group_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->add_community_channel_user_group_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_user_group_users_request** | [**CommunityChannelUserGroupUsersRequest**](CommunityChannelUserGroupUsersRequest.md)|  | 


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

# **add_community_channel_user_groups**
> CodeOnlyResponse add_community_channel_user_groups(community_channel_user_group_add_request)

Add community channel user groups

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_user_group_add_request import CommunityChannelUserGroupAddRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_user_group_add_request = ncsdk.CommunityChannelUserGroupAddRequest() # CommunityChannelUserGroupAddRequest | 
    

    try:
        # Add community channel user groups
        api_response = api_instance.add_community_channel_user_groups(community_channel_user_group_add_request)
        print("The response of CommunityChannelManagementApi->add_community_channel_user_groups:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->add_community_channel_user_groups: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_user_group_add_request** | [**CommunityChannelUserGroupAddRequest**](CommunityChannelUserGroupAddRequest.md)|  | 


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

# **add_private_subchannel_members**
> CodeOnlyResponse add_private_subchannel_members(community_private_subchannel_members_request)

Add private subchannel members

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_private_subchannel_members_request import CommunityPrivateSubchannelMembersRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_private_subchannel_members_request = ncsdk.CommunityPrivateSubchannelMembersRequest() # CommunityPrivateSubchannelMembersRequest | 
    

    try:
        # Add private subchannel members
        api_response = api_instance.add_private_subchannel_members(community_private_subchannel_members_request)
        print("The response of CommunityChannelManagementApi->add_private_subchannel_members:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->add_private_subchannel_members: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_private_subchannel_members_request** | [**CommunityPrivateSubchannelMembersRequest**](CommunityPrivateSubchannelMembersRequest.md)|  | 


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

# **bind_community_channel_user_group**
> CodeOnlyResponse bind_community_channel_user_group(community_channel_user_group_binding_request)

Bind community channel user group

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_user_group_binding_request import CommunityChannelUserGroupBindingRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_user_group_binding_request = ncsdk.CommunityChannelUserGroupBindingRequest() # CommunityChannelUserGroupBindingRequest | 
    

    try:
        # Bind community channel user group
        api_response = api_instance.bind_community_channel_user_group(community_channel_user_group_binding_request)
        print("The response of CommunityChannelManagementApi->bind_community_channel_user_group:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->bind_community_channel_user_group: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_user_group_binding_request** | [**CommunityChannelUserGroupBindingRequest**](CommunityChannelUserGroupBindingRequest.md)|  | 


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

# **check_community_channel_member_exist**
> CommunityChannelMemberExistResponse check_community_channel_member_exist(community_channel_member_request)

Check community channel member exist

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.community_channel_member_exist_response import CommunityChannelMemberExistResponse
from ncsdk.models.community_channel_member_request import CommunityChannelMemberRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_member_request = ncsdk.CommunityChannelMemberRequest() # CommunityChannelMemberRequest | 
    

    try:
        # Check community channel member exist
        api_response = api_instance.check_community_channel_member_exist(community_channel_member_request)
        print("The response of CommunityChannelManagementApi->check_community_channel_member_exist:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->check_community_channel_member_exist: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_member_request** | [**CommunityChannelMemberRequest**](CommunityChannelMemberRequest.md)|  | 


### Return type

[**CommunityChannelMemberExistResponse**](CommunityChannelMemberExistResponse.md)

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

# **create_community_channel**
> CodeOnlyResponse create_community_channel(community_channel_create_request)

Create community channel

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_create_request import CommunityChannelCreateRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_create_request = ncsdk.CommunityChannelCreateRequest() # CommunityChannelCreateRequest | 
    

    try:
        # Create community channel
        api_response = api_instance.create_community_channel(community_channel_create_request)
        print("The response of CommunityChannelManagementApi->create_community_channel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->create_community_channel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_create_request** | [**CommunityChannelCreateRequest**](CommunityChannelCreateRequest.md)|  | 


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

# **create_community_subchannel**
> CodeOnlyResponse create_community_subchannel(community_subchannel_create_request)

Create community subchannel

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_subchannel_create_request import CommunitySubchannelCreateRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_subchannel_create_request = ncsdk.CommunitySubchannelCreateRequest() # CommunitySubchannelCreateRequest | 
    

    try:
        # Create community subchannel
        api_response = api_instance.create_community_subchannel(community_subchannel_create_request)
        print("The response of CommunityChannelManagementApi->create_community_subchannel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->create_community_subchannel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_subchannel_create_request** | [**CommunitySubchannelCreateRequest**](CommunitySubchannelCreateRequest.md)|  | 


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

# **delete_community_subchannel**
> CodeOnlyResponse delete_community_subchannel(community_subchannel_key_request)

Delete community subchannel

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_subchannel_key_request import CommunitySubchannelKeyRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_subchannel_key_request = ncsdk.CommunitySubchannelKeyRequest() # CommunitySubchannelKeyRequest | 
    

    try:
        # Delete community subchannel
        api_response = api_instance.delete_community_subchannel(community_subchannel_key_request)
        print("The response of CommunityChannelManagementApi->delete_community_subchannel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->delete_community_subchannel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_subchannel_key_request** | [**CommunitySubchannelKeyRequest**](CommunitySubchannelKeyRequest.md)|  | 


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

# **dismiss_community_channel**
> CodeOnlyResponse dismiss_community_channel(community_channel_dismiss_request)

Dismiss community channel

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_dismiss_request import CommunityChannelDismissRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_dismiss_request = ncsdk.CommunityChannelDismissRequest() # CommunityChannelDismissRequest | 
    

    try:
        # Dismiss community channel
        api_response = api_instance.dismiss_community_channel(community_channel_dismiss_request)
        print("The response of CommunityChannelManagementApi->dismiss_community_channel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->dismiss_community_channel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_dismiss_request** | [**CommunityChannelDismissRequest**](CommunityChannelDismissRequest.md)|  | 


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

# **join_community_channel**
> CodeOnlyResponse join_community_channel(community_channel_member_request)

Join community channel

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_member_request import CommunityChannelMemberRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_member_request = ncsdk.CommunityChannelMemberRequest() # CommunityChannelMemberRequest | 
    

    try:
        # Join community channel
        api_response = api_instance.join_community_channel(community_channel_member_request)
        print("The response of CommunityChannelManagementApi->join_community_channel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->join_community_channel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_member_request** | [**CommunityChannelMemberRequest**](CommunityChannelMemberRequest.md)|  | 


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

# **list_community_channel_history_messages**
> MessageHistoryResponse list_community_channel_history_messages(community_channel_history_message_list_request)

List community-channel history messages

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.community_channel_history_message_list_request import CommunityChannelHistoryMessageListRequest
from ncsdk.models.message_history_response import MessageHistoryResponse
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_history_message_list_request = ncsdk.CommunityChannelHistoryMessageListRequest() # CommunityChannelHistoryMessageListRequest | 
    

    try:
        # List community-channel history messages
        api_response = api_instance.list_community_channel_history_messages(community_channel_history_message_list_request)
        print("The response of CommunityChannelManagementApi->list_community_channel_history_messages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->list_community_channel_history_messages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_history_message_list_request** | [**CommunityChannelHistoryMessageListRequest**](CommunityChannelHistoryMessageListRequest.md)|  | 


### Return type

[**MessageHistoryResponse**](MessageHistoryResponse.md)

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

# **list_community_channel_subchannel_user_groups**
> CommunityChannelSubchannelUserGroupListResponse list_community_channel_subchannel_user_groups(community_channel_subchannel_user_group_list_request)

List community channel subchannel user groups

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.community_channel_subchannel_user_group_list_request import CommunityChannelSubchannelUserGroupListRequest
from ncsdk.models.community_channel_subchannel_user_group_list_response import CommunityChannelSubchannelUserGroupListResponse
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_subchannel_user_group_list_request = ncsdk.CommunityChannelSubchannelUserGroupListRequest() # CommunityChannelSubchannelUserGroupListRequest | 
    

    try:
        # List community channel subchannel user groups
        api_response = api_instance.list_community_channel_subchannel_user_groups(community_channel_subchannel_user_group_list_request)
        print("The response of CommunityChannelManagementApi->list_community_channel_subchannel_user_groups:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->list_community_channel_subchannel_user_groups: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_subchannel_user_group_list_request** | [**CommunityChannelSubchannelUserGroupListRequest**](CommunityChannelSubchannelUserGroupListRequest.md)|  | 


### Return type

[**CommunityChannelSubchannelUserGroupListResponse**](CommunityChannelSubchannelUserGroupListResponse.md)

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

# **list_community_channel_user_group_subchannels**
> CommunityChannelUserGroupSubchannelListResponse list_community_channel_user_group_subchannels(community_channel_user_group_subchannel_list_request)

List community channel user group subchannels

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.community_channel_user_group_subchannel_list_request import CommunityChannelUserGroupSubchannelListRequest
from ncsdk.models.community_channel_user_group_subchannel_list_response import CommunityChannelUserGroupSubchannelListResponse
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_user_group_subchannel_list_request = ncsdk.CommunityChannelUserGroupSubchannelListRequest() # CommunityChannelUserGroupSubchannelListRequest | 
    

    try:
        # List community channel user group subchannels
        api_response = api_instance.list_community_channel_user_group_subchannels(community_channel_user_group_subchannel_list_request)
        print("The response of CommunityChannelManagementApi->list_community_channel_user_group_subchannels:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->list_community_channel_user_group_subchannels: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_user_group_subchannel_list_request** | [**CommunityChannelUserGroupSubchannelListRequest**](CommunityChannelUserGroupSubchannelListRequest.md)|  | 


### Return type

[**CommunityChannelUserGroupSubchannelListResponse**](CommunityChannelUserGroupSubchannelListResponse.md)

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

# **list_community_channel_user_groups**
> CommunityChannelUserGroupListResponse list_community_channel_user_groups(community_channel_user_group_list_request)

List community channel user groups

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.community_channel_user_group_list_request import CommunityChannelUserGroupListRequest
from ncsdk.models.community_channel_user_group_list_response import CommunityChannelUserGroupListResponse
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_user_group_list_request = ncsdk.CommunityChannelUserGroupListRequest() # CommunityChannelUserGroupListRequest | 
    

    try:
        # List community channel user groups
        api_response = api_instance.list_community_channel_user_groups(community_channel_user_group_list_request)
        print("The response of CommunityChannelManagementApi->list_community_channel_user_groups:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->list_community_channel_user_groups: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_user_group_list_request** | [**CommunityChannelUserGroupListRequest**](CommunityChannelUserGroupListRequest.md)|  | 


### Return type

[**CommunityChannelUserGroupListResponse**](CommunityChannelUserGroupListResponse.md)

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

# **list_community_channel_user_user_groups**
> CommunityChannelUserUserGroupListResponse list_community_channel_user_user_groups(community_channel_user_user_group_list_request)

List community channel user user groups

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.community_channel_user_user_group_list_request import CommunityChannelUserUserGroupListRequest
from ncsdk.models.community_channel_user_user_group_list_response import CommunityChannelUserUserGroupListResponse
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_user_user_group_list_request = ncsdk.CommunityChannelUserUserGroupListRequest() # CommunityChannelUserUserGroupListRequest | 
    

    try:
        # List community channel user user groups
        api_response = api_instance.list_community_channel_user_user_groups(community_channel_user_user_group_list_request)
        print("The response of CommunityChannelManagementApi->list_community_channel_user_user_groups:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->list_community_channel_user_user_groups: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_user_user_group_list_request** | [**CommunityChannelUserUserGroupListRequest**](CommunityChannelUserUserGroupListRequest.md)|  | 


### Return type

[**CommunityChannelUserUserGroupListResponse**](CommunityChannelUserUserGroupListResponse.md)

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

# **list_community_subchannels**
> CommunitySubchannelListResponse list_community_subchannels(community_subchannel_list_request)

List community subchannels

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.community_subchannel_list_request import CommunitySubchannelListRequest
from ncsdk.models.community_subchannel_list_response import CommunitySubchannelListResponse
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_subchannel_list_request = ncsdk.CommunitySubchannelListRequest() # CommunitySubchannelListRequest | 
    

    try:
        # List community subchannels
        api_response = api_instance.list_community_subchannels(community_subchannel_list_request)
        print("The response of CommunityChannelManagementApi->list_community_subchannels:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->list_community_subchannels: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_subchannel_list_request** | [**CommunitySubchannelListRequest**](CommunitySubchannelListRequest.md)|  | 


### Return type

[**CommunitySubchannelListResponse**](CommunitySubchannelListResponse.md)

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

# **list_community_user_subchannels**
> CommunityUserSubchannelListResponse list_community_user_subchannels(community_user_subchannel_list_request)

List community user subchannels

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.community_user_subchannel_list_request import CommunityUserSubchannelListRequest
from ncsdk.models.community_user_subchannel_list_response import CommunityUserSubchannelListResponse
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_user_subchannel_list_request = ncsdk.CommunityUserSubchannelListRequest() # CommunityUserSubchannelListRequest | 
    

    try:
        # List community user subchannels
        api_response = api_instance.list_community_user_subchannels(community_user_subchannel_list_request)
        print("The response of CommunityChannelManagementApi->list_community_user_subchannels:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->list_community_user_subchannels: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_user_subchannel_list_request** | [**CommunityUserSubchannelListRequest**](CommunityUserSubchannelListRequest.md)|  | 


### Return type

[**CommunityUserSubchannelListResponse**](CommunityUserSubchannelListResponse.md)

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

# **list_private_subchannel_members**
> CommunityPrivateSubchannelMemberListResponse list_private_subchannel_members(community_private_subchannel_member_list_request)

List private subchannel members

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.community_private_subchannel_member_list_request import CommunityPrivateSubchannelMemberListRequest
from ncsdk.models.community_private_subchannel_member_list_response import CommunityPrivateSubchannelMemberListResponse
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_private_subchannel_member_list_request = ncsdk.CommunityPrivateSubchannelMemberListRequest() # CommunityPrivateSubchannelMemberListRequest | 
    

    try:
        # List private subchannel members
        api_response = api_instance.list_private_subchannel_members(community_private_subchannel_member_list_request)
        print("The response of CommunityChannelManagementApi->list_private_subchannel_members:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->list_private_subchannel_members: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_private_subchannel_member_list_request** | [**CommunityPrivateSubchannelMemberListRequest**](CommunityPrivateSubchannelMemberListRequest.md)|  | 


### Return type

[**CommunityPrivateSubchannelMemberListResponse**](CommunityPrivateSubchannelMemberListResponse.md)

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

# **quit_community_channel**
> CodeOnlyResponse quit_community_channel(community_channel_member_request)

Leave community channel

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_member_request import CommunityChannelMemberRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_member_request = ncsdk.CommunityChannelMemberRequest() # CommunityChannelMemberRequest | 
    

    try:
        # Leave community channel
        api_response = api_instance.quit_community_channel(community_channel_member_request)
        print("The response of CommunityChannelManagementApi->quit_community_channel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->quit_community_channel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_member_request** | [**CommunityChannelMemberRequest**](CommunityChannelMemberRequest.md)|  | 


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

# **remove_community_channel_user_group_users**
> CodeOnlyResponse remove_community_channel_user_group_users(community_channel_user_group_users_request)

Remove community channel user group users

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_user_group_users_request import CommunityChannelUserGroupUsersRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_user_group_users_request = ncsdk.CommunityChannelUserGroupUsersRequest() # CommunityChannelUserGroupUsersRequest | 
    

    try:
        # Remove community channel user group users
        api_response = api_instance.remove_community_channel_user_group_users(community_channel_user_group_users_request)
        print("The response of CommunityChannelManagementApi->remove_community_channel_user_group_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->remove_community_channel_user_group_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_user_group_users_request** | [**CommunityChannelUserGroupUsersRequest**](CommunityChannelUserGroupUsersRequest.md)|  | 


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

# **remove_community_channel_user_groups**
> CodeOnlyResponse remove_community_channel_user_groups(community_channel_user_group_delete_request)

Delete community channel user groups

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_user_group_delete_request import CommunityChannelUserGroupDeleteRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_user_group_delete_request = ncsdk.CommunityChannelUserGroupDeleteRequest() # CommunityChannelUserGroupDeleteRequest | 
    

    try:
        # Delete community channel user groups
        api_response = api_instance.remove_community_channel_user_groups(community_channel_user_group_delete_request)
        print("The response of CommunityChannelManagementApi->remove_community_channel_user_groups:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->remove_community_channel_user_groups: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_user_group_delete_request** | [**CommunityChannelUserGroupDeleteRequest**](CommunityChannelUserGroupDeleteRequest.md)|  | 


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

# **remove_private_subchannel_members**
> CodeOnlyResponse remove_private_subchannel_members(community_private_subchannel_members_request)

Remove private subchannel members

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_private_subchannel_members_request import CommunityPrivateSubchannelMembersRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_private_subchannel_members_request = ncsdk.CommunityPrivateSubchannelMembersRequest() # CommunityPrivateSubchannelMembersRequest | 
    

    try:
        # Remove private subchannel members
        api_response = api_instance.remove_private_subchannel_members(community_private_subchannel_members_request)
        print("The response of CommunityChannelManagementApi->remove_private_subchannel_members:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->remove_private_subchannel_members: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_private_subchannel_members_request** | [**CommunityPrivateSubchannelMembersRequest**](CommunityPrivateSubchannelMembersRequest.md)|  | 


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

# **unbind_community_channel_user_group**
> CodeOnlyResponse unbind_community_channel_user_group(community_channel_user_group_binding_request)

Unbind community channel user group

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_user_group_binding_request import CommunityChannelUserGroupBindingRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_user_group_binding_request = ncsdk.CommunityChannelUserGroupBindingRequest() # CommunityChannelUserGroupBindingRequest | 
    

    try:
        # Unbind community channel user group
        api_response = api_instance.unbind_community_channel_user_group(community_channel_user_group_binding_request)
        print("The response of CommunityChannelManagementApi->unbind_community_channel_user_group:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->unbind_community_channel_user_group: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_user_group_binding_request** | [**CommunityChannelUserGroupBindingRequest**](CommunityChannelUserGroupBindingRequest.md)|  | 


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

# **update_community_channel_info**
> CodeOnlyResponse update_community_channel_info(community_channel_update_request)

Update community channel info

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_channel_update_request import CommunityChannelUpdateRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_channel_update_request = ncsdk.CommunityChannelUpdateRequest() # CommunityChannelUpdateRequest | 
    

    try:
        # Update community channel info
        api_response = api_instance.update_community_channel_info(community_channel_update_request)
        print("The response of CommunityChannelManagementApi->update_community_channel_info:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->update_community_channel_info: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_channel_update_request** | [**CommunityChannelUpdateRequest**](CommunityChannelUpdateRequest.md)|  | 


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

# **update_community_subchannel_type**
> CodeOnlyResponse update_community_subchannel_type(community_subchannel_type_update_request)

Update community subchannel type

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.community_subchannel_type_update_request import CommunitySubchannelTypeUpdateRequest
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
    api_instance = ncsdk.CommunityChannelManagementApi(api_client)
    
    community_subchannel_type_update_request = ncsdk.CommunitySubchannelTypeUpdateRequest() # CommunitySubchannelTypeUpdateRequest | 
    

    try:
        # Update community subchannel type
        api_response = api_instance.update_community_subchannel_type(community_subchannel_type_update_request)
        print("The response of CommunityChannelManagementApi->update_community_subchannel_type:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CommunityChannelManagementApi->update_community_subchannel_type: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **community_subchannel_type_update_request** | [**CommunitySubchannelTypeUpdateRequest**](CommunitySubchannelTypeUpdateRequest.md)|  | 


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

