# CommunityChannelMessageMetadataDeleteRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_id** | **str** |  | 
**user_id** | **str** |  | 
**channel_id** | **str** |  | 
**subchannel_id** | **str** | Should match the subchannel used when the message was sent. | [optional] 
**keys** | **List[str]** |  | 

## Example

```python
from ncsdk.models.community_channel_message_metadata_delete_request import CommunityChannelMessageMetadataDeleteRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelMessageMetadataDeleteRequest from a JSON string
community_channel_message_metadata_delete_request_instance = CommunityChannelMessageMetadataDeleteRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelMessageMetadataDeleteRequest.to_json())

# convert the object into a dict
community_channel_message_metadata_delete_request_dict = community_channel_message_metadata_delete_request_instance.to_dict()
# create an instance of CommunityChannelMessageMetadataDeleteRequest from a dict
community_channel_message_metadata_delete_request_from_dict = CommunityChannelMessageMetadataDeleteRequest.from_dict(community_channel_message_metadata_delete_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


