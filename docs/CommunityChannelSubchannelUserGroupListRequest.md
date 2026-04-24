# CommunityChannelSubchannelUserGroupListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**subchannel_id** | **str** |  | 
**page** | **int** |  | [optional] [default to 1]
**page_size** | **int** |  | [optional] [default to 10]

## Example

```python
from ncsdk.models.community_channel_subchannel_user_group_list_request import CommunityChannelSubchannelUserGroupListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelSubchannelUserGroupListRequest from a JSON string
community_channel_subchannel_user_group_list_request_instance = CommunityChannelSubchannelUserGroupListRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelSubchannelUserGroupListRequest.to_json())

# convert the object into a dict
community_channel_subchannel_user_group_list_request_dict = community_channel_subchannel_user_group_list_request_instance.to_dict()
# create an instance of CommunityChannelSubchannelUserGroupListRequest from a dict
community_channel_subchannel_user_group_list_request_from_dict = CommunityChannelSubchannelUserGroupListRequest.from_dict(community_channel_subchannel_user_group_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


