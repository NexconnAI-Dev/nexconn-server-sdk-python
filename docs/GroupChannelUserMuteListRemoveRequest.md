# GroupChannelUserMuteListRemoveRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** | Optional. When omitted, the operation applies to all group channels according to the PDF. | [optional] 
**user_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.group_channel_user_mute_list_remove_request import GroupChannelUserMuteListRemoveRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelUserMuteListRemoveRequest from a JSON string
group_channel_user_mute_list_remove_request_instance = GroupChannelUserMuteListRemoveRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelUserMuteListRemoveRequest.to_json())

# convert the object into a dict
group_channel_user_mute_list_remove_request_dict = group_channel_user_mute_list_remove_request_instance.to_dict()
# create an instance of GroupChannelUserMuteListRemoveRequest from a dict
group_channel_user_mute_list_remove_request_from_dict = GroupChannelUserMuteListRemoveRequest.from_dict(group_channel_user_mute_list_remove_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


