# CommunityPrivateSubchannelMemberListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**CommunityPrivateSubchannelMemberListResponseResult**](CommunityPrivateSubchannelMemberListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.community_private_subchannel_member_list_response import CommunityPrivateSubchannelMemberListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityPrivateSubchannelMemberListResponse from a JSON string
community_private_subchannel_member_list_response_instance = CommunityPrivateSubchannelMemberListResponse.from_json(json)
# print the JSON string representation of the object
print(CommunityPrivateSubchannelMemberListResponse.to_json())

# convert the object into a dict
community_private_subchannel_member_list_response_dict = community_private_subchannel_member_list_response_instance.to_dict()
# create an instance of CommunityPrivateSubchannelMemberListResponse from a dict
community_private_subchannel_member_list_response_from_dict = CommunityPrivateSubchannelMemberListResponse.from_dict(community_private_subchannel_member_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


