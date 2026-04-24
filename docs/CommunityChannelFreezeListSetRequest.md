# CommunityChannelFreezeListSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**subchannel_id** | **str** |  | [optional] 
**status** | **bool** | Freeze status for the community channel or subchannel. | 

## Example

```python
from ncsdk.models.community_channel_freeze_list_set_request import CommunityChannelFreezeListSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelFreezeListSetRequest from a JSON string
community_channel_freeze_list_set_request_instance = CommunityChannelFreezeListSetRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelFreezeListSetRequest.to_json())

# convert the object into a dict
community_channel_freeze_list_set_request_dict = community_channel_freeze_list_set_request_instance.to_dict()
# create an instance of CommunityChannelFreezeListSetRequest from a dict
community_channel_freeze_list_set_request_from_dict = CommunityChannelFreezeListSetRequest.from_dict(community_channel_freeze_list_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


