# CommunityChannelMessageUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**subchannel_id** | **str** |  | [optional] 
**from_user_id** | **str** |  | 
**message_id** | **str** |  | 
**content** | **str** |  | 

## Example

```python
from ncsdk.models.community_channel_message_update_request import CommunityChannelMessageUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelMessageUpdateRequest from a JSON string
community_channel_message_update_request_instance = CommunityChannelMessageUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelMessageUpdateRequest.to_json())

# convert the object into a dict
community_channel_message_update_request_dict = community_channel_message_update_request_instance.to_dict()
# create an instance of CommunityChannelMessageUpdateRequest from a dict
community_channel_message_update_request_from_dict = CommunityChannelMessageUpdateRequest.from_dict(community_channel_message_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


