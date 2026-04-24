# CommunityChannelMessageMetadataListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | [**List[MessageMetadataListItem]**](MessageMetadataListItem.md) | Same shape as channel-type list; array of &#x60;MetadataItem&#x60;. | [optional] 

## Example

```python
from ncsdk.models.community_channel_message_metadata_list_response_result import CommunityChannelMessageMetadataListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelMessageMetadataListResponseResult from a JSON string
community_channel_message_metadata_list_response_result_instance = CommunityChannelMessageMetadataListResponseResult.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelMessageMetadataListResponseResult.to_json())

# convert the object into a dict
community_channel_message_metadata_list_response_result_dict = community_channel_message_metadata_list_response_result_instance.to_dict()
# create an instance of CommunityChannelMessageMetadataListResponseResult from a dict
community_channel_message_metadata_list_response_result_from_dict = CommunityChannelMessageMetadataListResponseResult.from_dict(community_channel_message_metadata_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


