# CommunityChannelMuteListGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**CommunityChannelMuteListGetResponseResult**](CommunityChannelMuteListGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.community_channel_mute_list_get_response import CommunityChannelMuteListGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelMuteListGetResponse from a JSON string
community_channel_mute_list_get_response_instance = CommunityChannelMuteListGetResponse.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelMuteListGetResponse.to_json())

# convert the object into a dict
community_channel_mute_list_get_response_dict = community_channel_mute_list_get_response_instance.to_dict()
# create an instance of CommunityChannelMuteListGetResponse from a dict
community_channel_mute_list_get_response_from_dict = CommunityChannelMuteListGetResponse.from_dict(community_channel_mute_list_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


