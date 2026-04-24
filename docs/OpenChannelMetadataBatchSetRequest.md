# OpenChannelMetadataBatchSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**metadata_owner_id** | **str** | Legacy &#x60;entryOwnerId&#x60;. | 
**metadata** | **Dict[str, str]** | Legacy &#x60;entryInfo&#x60;. Up to 20 metadata entries per request. | 
**should_auto_delete** | **int** | &#x60;0&#x60; keeps metadata after the owner leaves and &#x60;1&#x60; removes it automatically. | [optional] 

## Example

```python
from ncsdk.models.open_channel_metadata_batch_set_request import OpenChannelMetadataBatchSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelMetadataBatchSetRequest from a JSON string
open_channel_metadata_batch_set_request_instance = OpenChannelMetadataBatchSetRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelMetadataBatchSetRequest.to_json())

# convert the object into a dict
open_channel_metadata_batch_set_request_dict = open_channel_metadata_batch_set_request_instance.to_dict()
# create an instance of OpenChannelMetadataBatchSetRequest from a dict
open_channel_metadata_batch_set_request_from_dict = OpenChannelMetadataBatchSetRequest.from_dict(open_channel_metadata_batch_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


