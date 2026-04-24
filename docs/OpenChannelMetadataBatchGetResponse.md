# OpenChannelMetadataBatchGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**OpenChannelMetadataBatchGetResponseResult**](OpenChannelMetadataBatchGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_metadata_batch_get_response import OpenChannelMetadataBatchGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelMetadataBatchGetResponse from a JSON string
open_channel_metadata_batch_get_response_instance = OpenChannelMetadataBatchGetResponse.from_json(json)
# print the JSON string representation of the object
print(OpenChannelMetadataBatchGetResponse.to_json())

# convert the object into a dict
open_channel_metadata_batch_get_response_dict = open_channel_metadata_batch_get_response_instance.to_dict()
# create an instance of OpenChannelMetadataBatchGetResponse from a dict
open_channel_metadata_batch_get_response_from_dict = OpenChannelMetadataBatchGetResponse.from_dict(open_channel_metadata_batch_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


