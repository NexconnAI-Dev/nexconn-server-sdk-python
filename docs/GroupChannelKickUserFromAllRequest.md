# GroupChannelKickUserFromAllRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 

## Example

```python
from ncsdk.models.group_channel_kick_user_from_all_request import GroupChannelKickUserFromAllRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelKickUserFromAllRequest from a JSON string
group_channel_kick_user_from_all_request_instance = GroupChannelKickUserFromAllRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelKickUserFromAllRequest.to_json())

# convert the object into a dict
group_channel_kick_user_from_all_request_dict = group_channel_kick_user_from_all_request_instance.to_dict()
# create an instance of GroupChannelKickUserFromAllRequest from a dict
group_channel_kick_user_from_all_request_from_dict = GroupChannelKickUserFromAllRequest.from_dict(group_channel_kick_user_from_all_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


