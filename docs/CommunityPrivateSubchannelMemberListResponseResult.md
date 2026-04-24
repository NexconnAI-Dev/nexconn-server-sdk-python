# CommunityPrivateSubchannelMemberListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**members** | **List[str]** |  | [optional] 

## Example

```python
from ncsdk.models.community_private_subchannel_member_list_response_result import CommunityPrivateSubchannelMemberListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityPrivateSubchannelMemberListResponseResult from a JSON string
community_private_subchannel_member_list_response_result_instance = CommunityPrivateSubchannelMemberListResponseResult.from_json(json)
# print the JSON string representation of the object
print(CommunityPrivateSubchannelMemberListResponseResult.to_json())

# convert the object into a dict
community_private_subchannel_member_list_response_result_dict = community_private_subchannel_member_list_response_result_instance.to_dict()
# create an instance of CommunityPrivateSubchannelMemberListResponseResult from a dict
community_private_subchannel_member_list_response_result_from_dict = CommunityPrivateSubchannelMemberListResponseResult.from_dict(community_private_subchannel_member_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


