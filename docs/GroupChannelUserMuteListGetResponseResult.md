# GroupChannelUserMuteListGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**muted_members** | [**List[GroupChannelMutedMemberItem]**](GroupChannelMutedMemberItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_user_mute_list_get_response_result import GroupChannelUserMuteListGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelUserMuteListGetResponseResult from a JSON string
group_channel_user_mute_list_get_response_result_instance = GroupChannelUserMuteListGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(GroupChannelUserMuteListGetResponseResult.to_json())

# convert the object into a dict
group_channel_user_mute_list_get_response_result_dict = group_channel_user_mute_list_get_response_result_instance.to_dict()
# create an instance of GroupChannelUserMuteListGetResponseResult from a dict
group_channel_user_mute_list_get_response_result_from_dict = GroupChannelUserMuteListGetResponseResult.from_dict(group_channel_user_mute_list_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


