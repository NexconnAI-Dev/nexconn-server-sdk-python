# ChannelTypeMessageMetadataListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_id** | **str** |  | 
**page** | **int** |  | [optional] 

## Example

```python
from ncsdk.models.channel_type_message_metadata_list_request import ChannelTypeMessageMetadataListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelTypeMessageMetadataListRequest from a JSON string
channel_type_message_metadata_list_request_instance = ChannelTypeMessageMetadataListRequest.from_json(json)
# print the JSON string representation of the object
print(ChannelTypeMessageMetadataListRequest.to_json())

# convert the object into a dict
channel_type_message_metadata_list_request_dict = channel_type_message_metadata_list_request_instance.to_dict()
# create an instance of ChannelTypeMessageMetadataListRequest from a dict
channel_type_message_metadata_list_request_from_dict = ChannelTypeMessageMetadataListRequest.from_dict(channel_type_message_metadata_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


