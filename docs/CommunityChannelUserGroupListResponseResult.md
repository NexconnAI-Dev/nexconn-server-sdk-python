# CommunityChannelUserGroupListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_groups** | [**List[CommunityChannelUserGroupItem]**](CommunityChannelUserGroupItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.community_channel_user_group_list_response_result import CommunityChannelUserGroupListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelUserGroupListResponseResult from a JSON string
community_channel_user_group_list_response_result_instance = CommunityChannelUserGroupListResponseResult.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelUserGroupListResponseResult.to_json())

# convert the object into a dict
community_channel_user_group_list_response_result_dict = community_channel_user_group_list_response_result_instance.to_dict()
# create an instance of CommunityChannelUserGroupListResponseResult from a dict
community_channel_user_group_list_response_result_from_dict = CommunityChannelUserGroupListResponseResult.from_dict(community_channel_user_group_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


