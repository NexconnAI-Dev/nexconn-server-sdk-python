# CommunityChannelMuteListGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**muted_members** | [**List[CommunityChannelMutedMemberItem]**](CommunityChannelMutedMemberItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.community_channel_mute_list_get_response_result import CommunityChannelMuteListGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelMuteListGetResponseResult from a JSON string
community_channel_mute_list_get_response_result_instance = CommunityChannelMuteListGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelMuteListGetResponseResult.to_json())

# convert the object into a dict
community_channel_mute_list_get_response_result_dict = community_channel_mute_list_get_response_result_instance.to_dict()
# create an instance of CommunityChannelMuteListGetResponseResult from a dict
community_channel_mute_list_get_response_result_from_dict = CommunityChannelMuteListGetResponseResult.from_dict(community_channel_mute_list_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


