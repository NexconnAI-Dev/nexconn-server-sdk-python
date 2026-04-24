# CommunityChannelMuteListRemoveRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**subchannel_id** | **str** |  | [optional] 
**user_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.community_channel_mute_list_remove_request import CommunityChannelMuteListRemoveRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelMuteListRemoveRequest from a JSON string
community_channel_mute_list_remove_request_instance = CommunityChannelMuteListRemoveRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelMuteListRemoveRequest.to_json())

# convert the object into a dict
community_channel_mute_list_remove_request_dict = community_channel_mute_list_remove_request_instance.to_dict()
# create an instance of CommunityChannelMuteListRemoveRequest from a dict
community_channel_mute_list_remove_request_from_dict = CommunityChannelMuteListRemoveRequest.from_dict(community_channel_mute_list_remove_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


