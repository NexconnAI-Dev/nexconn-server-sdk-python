# ncsdk.OpenChannelMetadataApi

All requests use the primary/backup domains configured by the caller.

Method | HTTP request | Description
------------- | ------------- | -------------
[**batch_get_open_channel_metadata**](OpenChannelMetadataApi.md#batch_get_open_channel_metadata) | **POST** /v4/open-channel/metadata/batch/get | Query metadata
[**batch_remove_open_channel_metadata**](OpenChannelMetadataApi.md#batch_remove_open_channel_metadata) | **POST** /v4/open-channel/metadata/batch/remove | Batch delete metadata
[**batch_set_open_channel_metadata**](OpenChannelMetadataApi.md#batch_set_open_channel_metadata) | **POST** /v4/open-channel/metadata/batch/set | Batch set metadata


# **batch_get_open_channel_metadata**
> OpenChannelMetadataBatchGetResponse batch_get_open_channel_metadata(open_channel_metadata_batch_get_request)

Query metadata

Rate limit: 100/sec.

### Example

* Api Key Authentication (NexconnSignature):

```python
import os
import ncsdk
from ncsdk.models.open_channel_metadata_batch_get_request import OpenChannelMetadataBatchGetRequest
from ncsdk.models.open_channel_metadata_batch_get_response import OpenChannelMetadataBatchGetResponse
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
    api_instance = ncsdk.OpenChannelMetadataApi(api_client)
    
    open_channel_metadata_batch_get_request = ncsdk.OpenChannelMetadataBatchGetRequest() # OpenChannelMetadataBatchGetRequest | 
    

    try:
        # Query metadata
        api_response = api_instance.batch_get_open_channel_metadata(open_channel_metadata_batch_get_request)
        print("The response of OpenChannelMetadataApi->batch_get_open_channel_metadata:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelMetadataApi->batch_get_open_channel_metadata: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_metadata_batch_get_request** | [**OpenChannelMetadataBatchGetRequest**](OpenChannelMetadataBatchGetRequest.md)|  | 


### Return type

[**OpenChannelMetadataBatchGetResponse**](OpenChannelMetadataBatchGetResponse.md)

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

# **batch_remove_open_channel_metadata**
> CodeOnlyResponse batch_remove_open_channel_metadata(open_channel_metadata_batch_remove_request)

Batch delete metadata

Rate limit: 100 attrs/sec (shared).

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_metadata_batch_remove_request import OpenChannelMetadataBatchRemoveRequest
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
    api_instance = ncsdk.OpenChannelMetadataApi(api_client)
    
    open_channel_metadata_batch_remove_request = ncsdk.OpenChannelMetadataBatchRemoveRequest() # OpenChannelMetadataBatchRemoveRequest | 
    

    try:
        # Batch delete metadata
        api_response = api_instance.batch_remove_open_channel_metadata(open_channel_metadata_batch_remove_request)
        print("The response of OpenChannelMetadataApi->batch_remove_open_channel_metadata:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelMetadataApi->batch_remove_open_channel_metadata: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_metadata_batch_remove_request** | [**OpenChannelMetadataBatchRemoveRequest**](OpenChannelMetadataBatchRemoveRequest.md)|  | 


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

# **batch_set_open_channel_metadata**
> CodeOnlyResponse batch_set_open_channel_metadata(open_channel_metadata_batch_set_request)

Batch set metadata

Rate limit: 100 attrs/sec (shared).

### Example

* Api Key Authentication (NexconnSignature):

```python
import ncsdk
from ncsdk.models.code_only_response import CodeOnlyResponse
from ncsdk.models.open_channel_metadata_batch_set_request import OpenChannelMetadataBatchSetRequest
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
    api_instance = ncsdk.OpenChannelMetadataApi(api_client)
    
    open_channel_metadata_batch_set_request = ncsdk.OpenChannelMetadataBatchSetRequest() # OpenChannelMetadataBatchSetRequest | 
    

    try:
        # Batch set metadata
        api_response = api_instance.batch_set_open_channel_metadata(open_channel_metadata_batch_set_request)
        print("The response of OpenChannelMetadataApi->batch_set_open_channel_metadata:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OpenChannelMetadataApi->batch_set_open_channel_metadata: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **open_channel_metadata_batch_set_request** | [**OpenChannelMetadataBatchSetRequest**](OpenChannelMetadataBatchSetRequest.md)|  | 


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

