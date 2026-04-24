# GroupChannelUserMuteListGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**GroupChannelUserMuteListGetResponseResult**](GroupChannelUserMuteListGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_user_mute_list_get_response import GroupChannelUserMuteListGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelUserMuteListGetResponse from a JSON string
group_channel_user_mute_list_get_response_instance = GroupChannelUserMuteListGetResponse.from_json(json)
# print the JSON string representation of the object
print(GroupChannelUserMuteListGetResponse.to_json())

# convert the object into a dict
group_channel_user_mute_list_get_response_dict = group_channel_user_mute_list_get_response_instance.to_dict()
# create an instance of GroupChannelUserMuteListGetResponse from a dict
group_channel_user_mute_list_get_response_from_dict = GroupChannelUserMuteListGetResponse.from_dict(group_channel_user_mute_list_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


