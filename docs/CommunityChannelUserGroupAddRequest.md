# CommunityChannelUserGroupAddRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**user_groups** | [**List[CommunityChannelUserGroupItem]**](CommunityChannelUserGroupItem.md) |  | 

## Example

```python
from ncsdk.models.community_channel_user_group_add_request import CommunityChannelUserGroupAddRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelUserGroupAddRequest from a JSON string
community_channel_user_group_add_request_instance = CommunityChannelUserGroupAddRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelUserGroupAddRequest.to_json())

# convert the object into a dict
community_channel_user_group_add_request_dict = community_channel_user_group_add_request_instance.to_dict()
# create an instance of CommunityChannelUserGroupAddRequest from a dict
community_channel_user_group_add_request_from_dict = CommunityChannelUserGroupAddRequest.from_dict(community_channel_user_group_add_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


