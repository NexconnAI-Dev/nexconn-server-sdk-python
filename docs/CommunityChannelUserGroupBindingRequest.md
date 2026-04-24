# CommunityChannelUserGroupBindingRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**subchannel_id** | **str** |  | 
**user_group_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.community_channel_user_group_binding_request import CommunityChannelUserGroupBindingRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelUserGroupBindingRequest from a JSON string
community_channel_user_group_binding_request_instance = CommunityChannelUserGroupBindingRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelUserGroupBindingRequest.to_json())

# convert the object into a dict
community_channel_user_group_binding_request_dict = community_channel_user_group_binding_request_instance.to_dict()
# create an instance of CommunityChannelUserGroupBindingRequest from a dict
community_channel_user_group_binding_request_from_dict = CommunityChannelUserGroupBindingRequest.from_dict(community_channel_user_group_binding_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


