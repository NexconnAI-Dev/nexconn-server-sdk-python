# ChannelTypeMessageMetadataListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**ChannelTypeMessageMetadataListResponseResult**](ChannelTypeMessageMetadataListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.channel_type_message_metadata_list_response import ChannelTypeMessageMetadataListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelTypeMessageMetadataListResponse from a JSON string
channel_type_message_metadata_list_response_instance = ChannelTypeMessageMetadataListResponse.from_json(json)
# print the JSON string representation of the object
print(ChannelTypeMessageMetadataListResponse.to_json())

# convert the object into a dict
channel_type_message_metadata_list_response_dict = channel_type_message_metadata_list_response_instance.to_dict()
# create an instance of ChannelTypeMessageMetadataListResponse from a dict
channel_type_message_metadata_list_response_from_dict = ChannelTypeMessageMetadataListResponse.from_dict(channel_type_message_metadata_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


