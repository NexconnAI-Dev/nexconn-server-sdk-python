# CommunityPrivateSubchannelMembersRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**subchannel_id** | **str** |  | 
**user_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.community_private_subchannel_members_request import CommunityPrivateSubchannelMembersRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityPrivateSubchannelMembersRequest from a JSON string
community_private_subchannel_members_request_instance = CommunityPrivateSubchannelMembersRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityPrivateSubchannelMembersRequest.to_json())

# convert the object into a dict
community_private_subchannel_members_request_dict = community_private_subchannel_members_request_instance.to_dict()
# create an instance of CommunityPrivateSubchannelMembersRequest from a dict
community_private_subchannel_members_request_from_dict = CommunityPrivateSubchannelMembersRequest.from_dict(community_private_subchannel_members_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


