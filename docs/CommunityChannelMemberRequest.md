# CommunityChannelMemberRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**channel_id** | **str** |  | 

## Example

```python
from ncsdk.models.community_channel_member_request import CommunityChannelMemberRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelMemberRequest from a JSON string
community_channel_member_request_instance = CommunityChannelMemberRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelMemberRequest.to_json())

# convert the object into a dict
community_channel_member_request_dict = community_channel_member_request_instance.to_dict()
# create an instance of CommunityChannelMemberRequest from a dict
community_channel_member_request_from_dict = CommunityChannelMemberRequest.from_dict(community_channel_member_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


