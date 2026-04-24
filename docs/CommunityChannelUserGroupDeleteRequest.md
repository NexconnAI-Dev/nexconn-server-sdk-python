# CommunityChannelUserGroupDeleteRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**user_group_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.community_channel_user_group_delete_request import CommunityChannelUserGroupDeleteRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelUserGroupDeleteRequest from a JSON string
community_channel_user_group_delete_request_instance = CommunityChannelUserGroupDeleteRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelUserGroupDeleteRequest.to_json())

# convert the object into a dict
community_channel_user_group_delete_request_dict = community_channel_user_group_delete_request_instance.to_dict()
# create an instance of CommunityChannelUserGroupDeleteRequest from a dict
community_channel_user_group_delete_request_from_dict = CommunityChannelUserGroupDeleteRequest.from_dict(community_channel_user_group_delete_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


