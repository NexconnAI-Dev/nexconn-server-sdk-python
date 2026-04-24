# GroupChannelMessageUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from_user_id** | **str** |  | 
**channel_id** | **str** |  | 
**message_id** | **str** |  | 
**content** | **str** |  | 

## Example

```python
from ncsdk.models.group_channel_message_update_request import GroupChannelMessageUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelMessageUpdateRequest from a JSON string
group_channel_message_update_request_instance = GroupChannelMessageUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelMessageUpdateRequest.to_json())

# convert the object into a dict
group_channel_message_update_request_dict = group_channel_message_update_request_instance.to_dict()
# create an instance of GroupChannelMessageUpdateRequest from a dict
group_channel_message_update_request_from_dict = GroupChannelMessageUpdateRequest.from_dict(group_channel_message_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


