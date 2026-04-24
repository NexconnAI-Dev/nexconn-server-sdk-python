# CommunityChannelMuteListGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**subchannel_id** | **str** |  | [optional] 
**page** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] [default to 50]

## Example

```python
from ncsdk.models.community_channel_mute_list_get_request import CommunityChannelMuteListGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelMuteListGetRequest from a JSON string
community_channel_mute_list_get_request_instance = CommunityChannelMuteListGetRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelMuteListGetRequest.to_json())

# convert the object into a dict
community_channel_mute_list_get_request_dict = community_channel_mute_list_get_request_instance.to_dict()
# create an instance of CommunityChannelMuteListGetRequest from a dict
community_channel_mute_list_get_request_from_dict = CommunityChannelMuteListGetRequest.from_dict(community_channel_mute_list_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


