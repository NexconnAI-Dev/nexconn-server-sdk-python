# GroupChannelFreezeListUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.group_channel_freeze_list_update_request import GroupChannelFreezeListUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelFreezeListUpdateRequest from a JSON string
group_channel_freeze_list_update_request_instance = GroupChannelFreezeListUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelFreezeListUpdateRequest.to_json())

# convert the object into a dict
group_channel_freeze_list_update_request_dict = group_channel_freeze_list_update_request_instance.to_dict()
# create an instance of GroupChannelFreezeListUpdateRequest from a dict
group_channel_freeze_list_update_request_from_dict = GroupChannelFreezeListUpdateRequest.from_dict(group_channel_freeze_list_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


