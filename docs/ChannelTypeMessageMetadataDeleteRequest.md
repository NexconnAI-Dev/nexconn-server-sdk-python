# ChannelTypeMessageMetadataDeleteRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_id** | **str** |  | 
**user_id** | **str** |  | 
**channel_type** | **int** | Supports direct and group channels. Legacy field name is &#x60;conversationType&#x60;. | 
**channel_id** | **str** | Legacy &#x60;targetId&#x60;. | 
**keys** | **List[str]** |  | 
**sync_to_sender** | **int** | Legacy &#x60;syncToSender&#x60;. &#x60;0&#x60; by default. | [optional] 

## Example

```python
from ncsdk.models.channel_type_message_metadata_delete_request import ChannelTypeMessageMetadataDeleteRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelTypeMessageMetadataDeleteRequest from a JSON string
channel_type_message_metadata_delete_request_instance = ChannelTypeMessageMetadataDeleteRequest.from_json(json)
# print the JSON string representation of the object
print(ChannelTypeMessageMetadataDeleteRequest.to_json())

# convert the object into a dict
channel_type_message_metadata_delete_request_dict = channel_type_message_metadata_delete_request_instance.to_dict()
# create an instance of ChannelTypeMessageMetadataDeleteRequest from a dict
channel_type_message_metadata_delete_request_from_dict = ChannelTypeMessageMetadataDeleteRequest.from_dict(channel_type_message_metadata_delete_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


