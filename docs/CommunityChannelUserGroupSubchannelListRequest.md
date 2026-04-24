# CommunityChannelUserGroupSubchannelListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**user_group_id** | **str** |  | 
**page** | **int** |  | [optional] [default to 1]
**page_size** | **int** |  | [optional] [default to 10]

## Example

```python
from ncsdk.models.community_channel_user_group_subchannel_list_request import CommunityChannelUserGroupSubchannelListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelUserGroupSubchannelListRequest from a JSON string
community_channel_user_group_subchannel_list_request_instance = CommunityChannelUserGroupSubchannelListRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelUserGroupSubchannelListRequest.to_json())

# convert the object into a dict
community_channel_user_group_subchannel_list_request_dict = community_channel_user_group_subchannel_list_request_instance.to_dict()
# create an instance of CommunityChannelUserGroupSubchannelListRequest from a dict
community_channel_user_group_subchannel_list_request_from_dict = CommunityChannelUserGroupSubchannelListRequest.from_dict(community_channel_user_group_subchannel_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


