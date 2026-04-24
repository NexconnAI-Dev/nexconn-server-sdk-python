# GroupChannelJoinRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**user_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.group_channel_join_request import GroupChannelJoinRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelJoinRequest from a JSON string
group_channel_join_request_instance = GroupChannelJoinRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelJoinRequest.to_json())

# convert the object into a dict
group_channel_join_request_dict = group_channel_join_request_instance.to_dict()
# create an instance of GroupChannelJoinRequest from a dict
group_channel_join_request_from_dict = GroupChannelJoinRequest.from_dict(group_channel_join_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


