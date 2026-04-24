# CommunityChannelMuteListAddRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**subchannel_id** | **str** |  | [optional] 
**user_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.community_channel_mute_list_add_request import CommunityChannelMuteListAddRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelMuteListAddRequest from a JSON string
community_channel_mute_list_add_request_instance = CommunityChannelMuteListAddRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelMuteListAddRequest.to_json())

# convert the object into a dict
community_channel_mute_list_add_request_dict = community_channel_mute_list_add_request_instance.to_dict()
# create an instance of CommunityChannelMuteListAddRequest from a dict
community_channel_mute_list_add_request_from_dict = CommunityChannelMuteListAddRequest.from_dict(community_channel_mute_list_add_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


