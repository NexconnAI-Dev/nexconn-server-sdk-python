# OpenChannelMetadataBatchRemoveRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**metadata_owner_id** | **str** | Legacy &#x60;entryOwnerId&#x60;. | 
**metadata_keys** | **List[str]** |  | 

## Example

```python
from ncsdk.models.open_channel_metadata_batch_remove_request import OpenChannelMetadataBatchRemoveRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelMetadataBatchRemoveRequest from a JSON string
open_channel_metadata_batch_remove_request_instance = OpenChannelMetadataBatchRemoveRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelMetadataBatchRemoveRequest.to_json())

# convert the object into a dict
open_channel_metadata_batch_remove_request_dict = open_channel_metadata_batch_remove_request_instance.to_dict()
# create an instance of OpenChannelMetadataBatchRemoveRequest from a dict
open_channel_metadata_batch_remove_request_from_dict = OpenChannelMetadataBatchRemoveRequest.from_dict(open_channel_metadata_batch_remove_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


