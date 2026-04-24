# CommunityPrivateSubchannelMemberListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**subchannel_id** | **str** |  | 
**page** | **int** |  | [optional] [default to 1]
**page_size** | **int** |  | [optional] [default to 50]

## Example

```python
from ncsdk.models.community_private_subchannel_member_list_request import CommunityPrivateSubchannelMemberListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityPrivateSubchannelMemberListRequest from a JSON string
community_private_subchannel_member_list_request_instance = CommunityPrivateSubchannelMemberListRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityPrivateSubchannelMemberListRequest.to_json())

# convert the object into a dict
community_private_subchannel_member_list_request_dict = community_private_subchannel_member_list_request_instance.to_dict()
# create an instance of CommunityPrivateSubchannelMemberListRequest from a dict
community_private_subchannel_member_list_request_from_dict = CommunityPrivateSubchannelMemberListRequest.from_dict(community_private_subchannel_member_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


