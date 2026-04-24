# GroupChannelAdminUsersRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**user_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.group_channel_admin_users_request import GroupChannelAdminUsersRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelAdminUsersRequest from a JSON string
group_channel_admin_users_request_instance = GroupChannelAdminUsersRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelAdminUsersRequest.to_json())

# convert the object into a dict
group_channel_admin_users_request_dict = group_channel_admin_users_request_instance.to_dict()
# create an instance of GroupChannelAdminUsersRequest from a dict
group_channel_admin_users_request_from_dict = GroupChannelAdminUsersRequest.from_dict(group_channel_admin_users_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


