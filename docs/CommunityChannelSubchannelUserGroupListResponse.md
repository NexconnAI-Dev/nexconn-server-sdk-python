# CommunityChannelSubchannelUserGroupListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**CommunityChannelSubchannelUserGroupListResponseResult**](CommunityChannelSubchannelUserGroupListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.community_channel_subchannel_user_group_list_response import CommunityChannelSubchannelUserGroupListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelSubchannelUserGroupListResponse from a JSON string
community_channel_subchannel_user_group_list_response_instance = CommunityChannelSubchannelUserGroupListResponse.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelSubchannelUserGroupListResponse.to_json())

# convert the object into a dict
community_channel_subchannel_user_group_list_response_dict = community_channel_subchannel_user_group_list_response_instance.to_dict()
# create an instance of CommunityChannelSubchannelUserGroupListResponse from a dict
community_channel_subchannel_user_group_list_response_from_dict = CommunityChannelSubchannelUserGroupListResponse.from_dict(community_channel_subchannel_user_group_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


