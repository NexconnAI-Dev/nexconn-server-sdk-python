# CommunityChannelAllowedSenderListGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**members** | [**List[CommunityChannelAllowedSenderItem]**](CommunityChannelAllowedSenderItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.community_channel_allowed_sender_list_get_response_result import CommunityChannelAllowedSenderListGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelAllowedSenderListGetResponseResult from a JSON string
community_channel_allowed_sender_list_get_response_result_instance = CommunityChannelAllowedSenderListGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelAllowedSenderListGetResponseResult.to_json())

# convert the object into a dict
community_channel_allowed_sender_list_get_response_result_dict = community_channel_allowed_sender_list_get_response_result_instance.to_dict()
# create an instance of CommunityChannelAllowedSenderListGetResponseResult from a dict
community_channel_allowed_sender_list_get_response_result_from_dict = CommunityChannelAllowedSenderListGetResponseResult.from_dict(community_channel_allowed_sender_list_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


