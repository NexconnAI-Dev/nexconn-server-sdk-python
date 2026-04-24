# GroupChannelUserMuteListAddRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** | Optional. When omitted, the operation applies to all group channels according to the PDF. | [optional] 
**user_ids** | **List[str]** |  | 
**duration_minutes** | **int** |  | 

## Example

```python
from ncsdk.models.group_channel_user_mute_list_add_request import GroupChannelUserMuteListAddRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelUserMuteListAddRequest from a JSON string
group_channel_user_mute_list_add_request_instance = GroupChannelUserMuteListAddRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelUserMuteListAddRequest.to_json())

# convert the object into a dict
group_channel_user_mute_list_add_request_dict = group_channel_user_mute_list_add_request_instance.to_dict()
# create an instance of GroupChannelUserMuteListAddRequest from a dict
group_channel_user_mute_list_add_request_from_dict = GroupChannelUserMuteListAddRequest.from_dict(group_channel_user_mute_list_add_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


