# CommunityChannelFreezeListGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**CommunityChannelFreezeListGetResponseResult**](CommunityChannelFreezeListGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.community_channel_freeze_list_get_response import CommunityChannelFreezeListGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelFreezeListGetResponse from a JSON string
community_channel_freeze_list_get_response_instance = CommunityChannelFreezeListGetResponse.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelFreezeListGetResponse.to_json())

# convert the object into a dict
community_channel_freeze_list_get_response_dict = community_channel_freeze_list_get_response_instance.to_dict()
# create an instance of CommunityChannelFreezeListGetResponse from a dict
community_channel_freeze_list_get_response_from_dict = CommunityChannelFreezeListGetResponse.from_dict(community_channel_freeze_list_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


