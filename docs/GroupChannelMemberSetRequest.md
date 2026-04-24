# GroupChannelMemberSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**user_id** | **str** |  | 
**nickname** | **str** |  | [optional] 
**extra** | **str** | Member extra profile string defined by the source API. | [optional] 

## Example

```python
from ncsdk.models.group_channel_member_set_request import GroupChannelMemberSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelMemberSetRequest from a JSON string
group_channel_member_set_request_instance = GroupChannelMemberSetRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelMemberSetRequest.to_json())

# convert the object into a dict
group_channel_member_set_request_dict = group_channel_member_set_request_instance.to_dict()
# create an instance of GroupChannelMemberSetRequest from a dict
group_channel_member_set_request_from_dict = GroupChannelMemberSetRequest.from_dict(group_channel_member_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


