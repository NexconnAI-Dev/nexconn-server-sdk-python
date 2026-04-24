# ncsdk.ModerationApi

All requests use the primary/backup domains configured by the caller.

Method | HTTP request | Description
------------- | ------------- | -------------
[**batch_add_profanity_words**](ModerationApi.md#batch_add_profanity_words) | **POST** /v4/profanity-word/batch/add | Batch add profanity words
[**batch_remove_profanity_words**](ModerationApi.md#batch_remove_profanity_words) | **POST** /v4/profanity-word/batch/remove | Batch delete profanity words
[**list_profanity_words**](ModerationApi.md#list_profanity_words) | **POST** /v4/profanity-word/list | List profanity words
[**remove_profanity_word**](ModerationApi.md#remove_profanity_word) | **POST** /v4/profanity-word/remove | Delete profanity word


# **batch_add_profanity_words**
> ProfanityWordBatchAddResponse batch_add_profanity_words(profanity_word_batch_add_request)

Batch add profanity words

### Example

* Api Key Authentication (NexconnSignature):

```python
import os
import ncsdk
from ncsdk.models.profanity_word_batch_add_request import ProfanityWordBatchAddRequest
from ncsdk.models.profanity_word_batch_add_response import ProfanityWordBatchAddResponse
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
    api_instance = ncsdk.ModerationApi(api_client)
    
    profanity_word_batch_add_request = ncsdk.ProfanityWordBatchAddRequest() # ProfanityWordBatchAddRequest | 
    

    try:
        # Batch add profanity words
        api_response = api_instance.batch_add_profanity_words(profanity_word_batch_add_request)
        print("The response of ModerationApi->batch_add_profanity_words:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ModerationApi->batch_add_profanity_words: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profanity_word_batch_add_request** | [**ProfanityWordBatchAddRequest**](ProfanityWordBatchAddRequest.md)|  | 


### Return type

[**ProfanityWordBatchAddResponse**](ProfanityWordBatchAddResponse.md)

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

# **batch_remove_profanity_words**
> CodeOnlyResponse batch_remove_profanity_words(profanity_word_batch_delete_request)

Batch delete profanity words

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.profanity_word_batch_delete_request import ProfanityWordBatchDeleteRequest
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
    api_instance = ncsdk.ModerationApi(api_client)
    
    profanity_word_batch_delete_request = ncsdk.ProfanityWordBatchDeleteRequest() # ProfanityWordBatchDeleteRequest | 
    

    try:
        # Batch delete profanity words
        api_response = api_instance.batch_remove_profanity_words(profanity_word_batch_delete_request)
        print("The response of ModerationApi->batch_remove_profanity_words:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ModerationApi->batch_remove_profanity_words: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profanity_word_batch_delete_request** | [**ProfanityWordBatchDeleteRequest**](ProfanityWordBatchDeleteRequest.md)|  | 


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

# **list_profanity_words**
> ProfanityWordListResponse list_profanity_words(profanity_word_list_request)

List profanity words

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.profanity_word_list_request import ProfanityWordListRequest
from ncsdk.models.profanity_word_list_response import ProfanityWordListResponse
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
    api_instance = ncsdk.ModerationApi(api_client)
    
    profanity_word_list_request = ncsdk.ProfanityWordListRequest() # ProfanityWordListRequest | 
    

    try:
        # List profanity words
        api_response = api_instance.list_profanity_words(profanity_word_list_request)
        print("The response of ModerationApi->list_profanity_words:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ModerationApi->list_profanity_words: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profanity_word_list_request** | [**ProfanityWordListRequest**](ProfanityWordListRequest.md)|  | 


### Return type

[**ProfanityWordListResponse**](ProfanityWordListResponse.md)

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

# **remove_profanity_word**
> CodeOnlyResponse remove_profanity_word(profanity_word_delete_request)

Delete profanity word

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.profanity_word_delete_request import ProfanityWordDeleteRequest
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
    api_instance = ncsdk.ModerationApi(api_client)
    
    profanity_word_delete_request = ncsdk.ProfanityWordDeleteRequest() # ProfanityWordDeleteRequest | 
    

    try:
        # Delete profanity word
        api_response = api_instance.remove_profanity_word(profanity_word_delete_request)
        print("The response of ModerationApi->remove_profanity_word:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ModerationApi->remove_profanity_word: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profanity_word_delete_request** | [**ProfanityWordDeleteRequest**](ProfanityWordDeleteRequest.md)|  | 


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

