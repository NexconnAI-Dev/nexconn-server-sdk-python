# ncsdk.FriendshipApi

All requests use the primary/backup domains configured by the caller.

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_friend**](FriendshipApi.md#add_friend) | **POST** /v4/friend/add | Add friend
[**get_friend_permission**](FriendshipApi.md#get_friend_permission) | **POST** /v4/friend/permission/get | Get friend permission
[**get_friend_relationships**](FriendshipApi.md#get_friend_relationships) | **POST** /v4/friend/relationship/get | Get friend relationships
[**list_friends**](FriendshipApi.md#list_friends) | **POST** /v4/friend/list | List friends
[**remove_all_friends**](FriendshipApi.md#remove_all_friends) | **POST** /v4/friend/remove-all | Clean all friends
[**remove_friends**](FriendshipApi.md#remove_friends) | **POST** /v4/friend/remove | Delete friends
[**set_friend_permission**](FriendshipApi.md#set_friend_permission) | **POST** /v4/friend/permission/set | Set friend permission
[**set_friend_profile**](FriendshipApi.md#set_friend_profile) | **POST** /v4/friend/profile/set | Set friend profile


# **add_friend**
> CodeOnlyResponse add_friend(friend_add_request)

Add friend

### Example

* Api Key Authentication (NexconnSignature):

```python
import os
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.friend_add_request import FriendAddRequest
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
    api_instance = ncsdk.FriendshipApi(api_client)
    
    friend_add_request = ncsdk.FriendAddRequest() # FriendAddRequest | 
    

    try:
        # Add friend
        api_response = api_instance.add_friend(friend_add_request)
        print("The response of FriendshipApi->add_friend:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FriendshipApi->add_friend: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **friend_add_request** | [**FriendAddRequest**](FriendAddRequest.md)|  | 


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

# **get_friend_permission**
> FriendPermissionGetResponse get_friend_permission(friend_permission_get_request)

Get friend permission

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.friend_permission_get_request import FriendPermissionGetRequest
from ncsdk.models.friend_permission_get_response import FriendPermissionGetResponse
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
    api_instance = ncsdk.FriendshipApi(api_client)
    
    friend_permission_get_request = ncsdk.FriendPermissionGetRequest() # FriendPermissionGetRequest | 
    

    try:
        # Get friend permission
        api_response = api_instance.get_friend_permission(friend_permission_get_request)
        print("The response of FriendshipApi->get_friend_permission:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FriendshipApi->get_friend_permission: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **friend_permission_get_request** | [**FriendPermissionGetRequest**](FriendPermissionGetRequest.md)|  | 


### Return type

[**FriendPermissionGetResponse**](FriendPermissionGetResponse.md)

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

# **get_friend_relationships**
> FriendRelationshipGetResponse get_friend_relationships(friend_relationship_get_request)

Get friend relationships

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.friend_relationship_get_request import FriendRelationshipGetRequest
from ncsdk.models.friend_relationship_get_response import FriendRelationshipGetResponse
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
    api_instance = ncsdk.FriendshipApi(api_client)
    
    friend_relationship_get_request = ncsdk.FriendRelationshipGetRequest() # FriendRelationshipGetRequest | 
    

    try:
        # Get friend relationships
        api_response = api_instance.get_friend_relationships(friend_relationship_get_request)
        print("The response of FriendshipApi->get_friend_relationships:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FriendshipApi->get_friend_relationships: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **friend_relationship_get_request** | [**FriendRelationshipGetRequest**](FriendRelationshipGetRequest.md)|  | 


### Return type

[**FriendRelationshipGetResponse**](FriendRelationshipGetResponse.md)

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

# **list_friends**
> FriendListResponse list_friends(friend_list_request)

List friends

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.friend_list_request import FriendListRequest
from ncsdk.models.friend_list_response import FriendListResponse
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
    api_instance = ncsdk.FriendshipApi(api_client)
    
    friend_list_request = ncsdk.FriendListRequest() # FriendListRequest | 
    

    try:
        # List friends
        api_response = api_instance.list_friends(friend_list_request)
        print("The response of FriendshipApi->list_friends:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FriendshipApi->list_friends: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **friend_list_request** | [**FriendListRequest**](FriendListRequest.md)|  | 


### Return type

[**FriendListResponse**](FriendListResponse.md)

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

# **remove_all_friends**
> CodeOnlyResponse remove_all_friends(friend_clean_request)

Clean all friends

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.friend_clean_request import FriendCleanRequest
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
    api_instance = ncsdk.FriendshipApi(api_client)
    
    friend_clean_request = ncsdk.FriendCleanRequest() # FriendCleanRequest | 
    

    try:
        # Clean all friends
        api_response = api_instance.remove_all_friends(friend_clean_request)
        print("The response of FriendshipApi->remove_all_friends:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FriendshipApi->remove_all_friends: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **friend_clean_request** | [**FriendCleanRequest**](FriendCleanRequest.md)|  | 


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

# **remove_friends**
> CodeOnlyResponse remove_friends(friend_delete_request)

Delete friends

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.friend_delete_request import FriendDeleteRequest
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
    api_instance = ncsdk.FriendshipApi(api_client)
    
    friend_delete_request = ncsdk.FriendDeleteRequest() # FriendDeleteRequest | 
    

    try:
        # Delete friends
        api_response = api_instance.remove_friends(friend_delete_request)
        print("The response of FriendshipApi->remove_friends:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FriendshipApi->remove_friends: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **friend_delete_request** | [**FriendDeleteRequest**](FriendDeleteRequest.md)|  | 


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

# **set_friend_permission**
> CodeOnlyResponse set_friend_permission(friend_permission_set_request)

Set friend permission

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.friend_permission_set_request import FriendPermissionSetRequest
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
    api_instance = ncsdk.FriendshipApi(api_client)
    
    friend_permission_set_request = ncsdk.FriendPermissionSetRequest() # FriendPermissionSetRequest | 
    

    try:
        # Set friend permission
        api_response = api_instance.set_friend_permission(friend_permission_set_request)
        print("The response of FriendshipApi->set_friend_permission:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FriendshipApi->set_friend_permission: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **friend_permission_set_request** | [**FriendPermissionSetRequest**](FriendPermissionSetRequest.md)|  | 


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

# **set_friend_profile**
> CodeOnlyResponse set_friend_profile(friend_profile_set_request)

Set friend profile

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.friend_profile_set_request import FriendProfileSetRequest
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
    api_instance = ncsdk.FriendshipApi(api_client)
    
    friend_profile_set_request = ncsdk.FriendProfileSetRequest() # FriendProfileSetRequest | 
    

    try:
        # Set friend profile
        api_response = api_instance.set_friend_profile(friend_profile_set_request)
        print("The response of FriendshipApi->set_friend_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FriendshipApi->set_friend_profile: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **friend_profile_set_request** | [**FriendProfileSetRequest**](FriendProfileSetRequest.md)|  | 


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

