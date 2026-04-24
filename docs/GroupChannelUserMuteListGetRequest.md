# GroupChannelUserMuteListGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** | Optional group channel ID filter. | [optional] 

## Example

```python
from ncsdk.models.group_channel_user_mute_list_get_request import GroupChannelUserMuteListGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelUserMuteListGetRequest from a JSON string
group_channel_user_mute_list_get_request_instance = GroupChannelUserMuteListGetRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelUserMuteListGetRequest.to_json())

# convert the object into a dict
group_channel_user_mute_list_get_request_dict = group_channel_user_mute_list_get_request_instance.to_dict()
# create an instance of GroupChannelUserMuteListGetRequest from a dict
group_channel_user_mute_list_get_request_from_dict = GroupChannelUserMuteListGetRequest.from_dict(group_channel_user_mute_list_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


