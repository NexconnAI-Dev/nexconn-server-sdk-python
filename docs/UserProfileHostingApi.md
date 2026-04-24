# ncsdk.UserProfileHostingApi

All requests use the primary/backup domains configured by the caller.

Method | HTTP request | Description
------------- | ------------- | -------------
[**batch_get_user_profiles**](UserProfileHostingApi.md#batch_get_user_profiles) | **POST** /v4/user/profile/batch/get | Batch get user profiles
[**delete_user_profiles**](UserProfileHostingApi.md#delete_user_profiles) | **POST** /v4/user/profile/delete | Clear user profiles
[**list_user_profiles**](UserProfileHostingApi.md#list_user_profiles) | **POST** /v4/user/profile/list | List user profiles
[**set_user_profile**](UserProfileHostingApi.md#set_user_profile) | **POST** /v4/user/profile/set | Set user profile


# **batch_get_user_profiles**
> UserProfileBatchGetResponse batch_get_user_profiles(user_ids_max20_request)

Batch get user profiles

### Example

* Api Key Authentication (NexconnSignature):

```python
import os
import ncsdk
from ncsdk.models.user_ids_max20_request import UserIdsMax20Request
from ncsdk.models.user_profile_batch_get_response import UserProfileBatchGetResponse
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
    api_instance = ncsdk.UserProfileHostingApi(api_client)
    
    user_ids_max20_request = ncsdk.UserIdsMax20Request() # UserIdsMax20Request | 
    

    try:
        # Batch get user profiles
        api_response = api_instance.batch_get_user_profiles(user_ids_max20_request)
        print("The response of UserProfileHostingApi->batch_get_user_profiles:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserProfileHostingApi->batch_get_user_profiles: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_ids_max20_request** | [**UserIdsMax20Request**](UserIdsMax20Request.md)|  | 


### Return type

[**UserProfileBatchGetResponse**](UserProfileBatchGetResponse.md)

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

# **delete_user_profiles**
> CodeOnlyResponse delete_user_profiles(user_ids_max20_request)

Clear user profiles

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
    api_instance = ncsdk.UserProfileHostingApi(api_client)
    
    user_ids_max20_request = ncsdk.UserIdsMax20Request() # UserIdsMax20Request | 
    

    try:
        # Clear user profiles
        api_response = api_instance.delete_user_profiles(user_ids_max20_request)
        print("The response of UserProfileHostingApi->delete_user_profiles:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserProfileHostingApi->delete_user_profiles: %s\n" % e)
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

# **list_user_profiles**
> UserProfileListResponse list_user_profiles(user_profile_list_request)

List user profiles

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.user_profile_list_request import UserProfileListRequest
from ncsdk.models.user_profile_list_response import UserProfileListResponse
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
    api_instance = ncsdk.UserProfileHostingApi(api_client)
    
    user_profile_list_request = ncsdk.UserProfileListRequest() # UserProfileListRequest | 
    

    try:
        # List user profiles
        api_response = api_instance.list_user_profiles(user_profile_list_request)
        print("The response of UserProfileHostingApi->list_user_profiles:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserProfileHostingApi->list_user_profiles: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_profile_list_request** | [**UserProfileListRequest**](UserProfileListRequest.md)|  | 


### Return type

[**UserProfileListResponse**](UserProfileListResponse.md)

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

# **set_user_profile**
> UserProfileSetResponse set_user_profile(user_profile_set_request)

Set user profile

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.user_profile_set_request import UserProfileSetRequest
from ncsdk.models.user_profile_set_response import UserProfileSetResponse
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
    api_instance = ncsdk.UserProfileHostingApi(api_client)
    
    user_profile_set_request = ncsdk.UserProfileSetRequest() # UserProfileSetRequest | 
    

    try:
        # Set user profile
        api_response = api_instance.set_user_profile(user_profile_set_request)
        print("The response of UserProfileHostingApi->set_user_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserProfileHostingApi->set_user_profile: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_profile_set_request** | [**UserProfileSetRequest**](UserProfileSetRequest.md)|  | 


### Return type

[**UserProfileSetResponse**](UserProfileSetResponse.md)

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

