# CommunityChannelMessageMetadataListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_id** | **str** |  | 
**channel_id** | **str** |  | 
**subchannel_id** | **str** | Should match the subchannel used when the message was sent. | [optional] 
**page** | **int** |  | [optional] 

## Example

```python
from ncsdk.models.community_channel_message_metadata_list_request import CommunityChannelMessageMetadataListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelMessageMetadataListRequest from a JSON string
community_channel_message_metadata_list_request_instance = CommunityChannelMessageMetadataListRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelMessageMetadataListRequest.to_json())

# convert the object into a dict
community_channel_message_metadata_list_request_dict = community_channel_message_metadata_list_request_instance.to_dict()
# create an instance of CommunityChannelMessageMetadataListRequest from a dict
community_channel_message_metadata_list_request_from_dict = CommunityChannelMessageMetadataListRequest.from_dict(community_channel_message_metadata_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


