# CommunityChannelMessageMetadataSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_id** | **str** |  | 
**user_id** | **str** |  | 
**channel_id** | **str** |  | 
**subchannel_id** | **str** |  | [optional] 
**metadata** | **Dict[str, str]** | Community-channel message metadata to set. Keys support letters, digits, and &#x60;+ &#x3D; - _&#x60;, with a maximum key length of 32 characters. Each request can set up to 20 entries.  | 

## Example

```python
from ncsdk.models.community_channel_message_metadata_set_request import CommunityChannelMessageMetadataSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelMessageMetadataSetRequest from a JSON string
community_channel_message_metadata_set_request_instance = CommunityChannelMessageMetadataSetRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelMessageMetadataSetRequest.to_json())

# convert the object into a dict
community_channel_message_metadata_set_request_dict = community_channel_message_metadata_set_request_instance.to_dict()
# create an instance of CommunityChannelMessageMetadataSetRequest from a dict
community_channel_message_metadata_set_request_from_dict = CommunityChannelMessageMetadataSetRequest.from_dict(community_channel_message_metadata_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


