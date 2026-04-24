# CommunityChannelUserGroupListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**page** | **int** |  | [optional] [default to 1]
**page_size** | **int** |  | [optional] [default to 10]
**order** | **int** | Sort order from &#x60;CommunityChannelPageInput&#x60;. | [optional] 

## Example

```python
from ncsdk.models.community_channel_user_group_list_request import CommunityChannelUserGroupListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelUserGroupListRequest from a JSON string
community_channel_user_group_list_request_instance = CommunityChannelUserGroupListRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelUserGroupListRequest.to_json())

# convert the object into a dict
community_channel_user_group_list_request_dict = community_channel_user_group_list_request_instance.to_dict()
# create an instance of CommunityChannelUserGroupListRequest from a dict
community_channel_user_group_list_request_from_dict = CommunityChannelUserGroupListRequest.from_dict(community_channel_user_group_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


