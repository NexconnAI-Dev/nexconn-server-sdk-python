# ChannelTypeMessageMetadataListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | [**List[MessageMetadataListItem]**](MessageMetadataListItem.md) | Ordered list from &#x60;MessageMetadataResult&#x60; / &#x60;MetadataItem&#x60; (not a key-value object). | [optional] 

## Example

```python
from ncsdk.models.channel_type_message_metadata_list_response_result import ChannelTypeMessageMetadataListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelTypeMessageMetadataListResponseResult from a JSON string
channel_type_message_metadata_list_response_result_instance = ChannelTypeMessageMetadataListResponseResult.from_json(json)
# print the JSON string representation of the object
print(ChannelTypeMessageMetadataListResponseResult.to_json())

# convert the object into a dict
channel_type_message_metadata_list_response_result_dict = channel_type_message_metadata_list_response_result_instance.to_dict()
# create an instance of ChannelTypeMessageMetadataListResponseResult from a dict
channel_type_message_metadata_list_response_result_from_dict = ChannelTypeMessageMetadataListResponseResult.from_dict(channel_type_message_metadata_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


