# OpenChannelMetadataBatchGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**metadata_keys** | **List[str]** | Metadata keys to fetch. When omitted, the service returns metadata according to its default rule. | [optional] 

## Example

```python
from ncsdk.models.open_channel_metadata_batch_get_request import OpenChannelMetadataBatchGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelMetadataBatchGetRequest from a JSON string
open_channel_metadata_batch_get_request_instance = OpenChannelMetadataBatchGetRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelMetadataBatchGetRequest.to_json())

# convert the object into a dict
open_channel_metadata_batch_get_request_dict = open_channel_metadata_batch_get_request_instance.to_dict()
# create an instance of OpenChannelMetadataBatchGetRequest from a dict
open_channel_metadata_batch_get_request_from_dict = OpenChannelMetadataBatchGetRequest.from_dict(open_channel_metadata_batch_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


