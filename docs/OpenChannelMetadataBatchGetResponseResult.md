# OpenChannelMetadataBatchGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | [**List[OpenChannelMetadataEntry]**](OpenChannelMetadataEntry.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_metadata_batch_get_response_result import OpenChannelMetadataBatchGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelMetadataBatchGetResponseResult from a JSON string
open_channel_metadata_batch_get_response_result_instance = OpenChannelMetadataBatchGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(OpenChannelMetadataBatchGetResponseResult.to_json())

# convert the object into a dict
open_channel_metadata_batch_get_response_result_dict = open_channel_metadata_batch_get_response_result_instance.to_dict()
# create an instance of OpenChannelMetadataBatchGetResponseResult from a dict
open_channel_metadata_batch_get_response_result_from_dict = OpenChannelMetadataBatchGetResponseResult.from_dict(open_channel_metadata_batch_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


