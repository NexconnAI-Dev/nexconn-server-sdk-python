# CommunityChannelUserGroupSubchannelListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**CommunityChannelUserGroupSubchannelListResponseResult**](CommunityChannelUserGroupSubchannelListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.community_channel_user_group_subchannel_list_response import CommunityChannelUserGroupSubchannelListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelUserGroupSubchannelListResponse from a JSON string
community_channel_user_group_subchannel_list_response_instance = CommunityChannelUserGroupSubchannelListResponse.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelUserGroupSubchannelListResponse.to_json())

# convert the object into a dict
community_channel_user_group_subchannel_list_response_dict = community_channel_user_group_subchannel_list_response_instance.to_dict()
# create an instance of CommunityChannelUserGroupSubchannelListResponse from a dict
community_channel_user_group_subchannel_list_response_from_dict = CommunityChannelUserGroupSubchannelListResponse.from_dict(community_channel_user_group_subchannel_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


