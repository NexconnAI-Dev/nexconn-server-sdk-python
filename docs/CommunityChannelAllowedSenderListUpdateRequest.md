# CommunityChannelAllowedSenderListUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**subchannel_id** | **str** |  | [optional] 
**user_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.community_channel_allowed_sender_list_update_request import CommunityChannelAllowedSenderListUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelAllowedSenderListUpdateRequest from a JSON string
community_channel_allowed_sender_list_update_request_instance = CommunityChannelAllowedSenderListUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelAllowedSenderListUpdateRequest.to_json())

# convert the object into a dict
community_channel_allowed_sender_list_update_request_dict = community_channel_allowed_sender_list_update_request_instance.to_dict()
# create an instance of CommunityChannelAllowedSenderListUpdateRequest from a dict
community_channel_allowed_sender_list_update_request_from_dict = CommunityChannelAllowedSenderListUpdateRequest.from_dict(community_channel_allowed_sender_list_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


