# CommunityChannelUserGroupUsersRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**user_group_id** | **str** |  | 
**user_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.community_channel_user_group_users_request import CommunityChannelUserGroupUsersRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelUserGroupUsersRequest from a JSON string
community_channel_user_group_users_request_instance = CommunityChannelUserGroupUsersRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelUserGroupUsersRequest.to_json())

# convert the object into a dict
community_channel_user_group_users_request_dict = community_channel_user_group_users_request_instance.to_dict()
# create an instance of CommunityChannelUserGroupUsersRequest from a dict
community_channel_user_group_users_request_from_dict = CommunityChannelUserGroupUsersRequest.from_dict(community_channel_user_group_users_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


