# CommunityChannelHistoryMessageListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**subchannel_id** | **str** |  | 
**start_at** | **int** |  | 
**end_at** | **int** |  | 
**from_user_id** | **str** |  | [optional] 
**page_size** | **int** |  | [optional] [default to 20]

## Example

```python
from ncsdk.models.community_channel_history_message_list_request import CommunityChannelHistoryMessageListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelHistoryMessageListRequest from a JSON string
community_channel_history_message_list_request_instance = CommunityChannelHistoryMessageListRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelHistoryMessageListRequest.to_json())

# convert the object into a dict
community_channel_history_message_list_request_dict = community_channel_history_message_list_request_instance.to_dict()
# create an instance of CommunityChannelHistoryMessageListRequest from a dict
community_channel_history_message_list_request_from_dict = CommunityChannelHistoryMessageListRequest.from_dict(community_channel_history_message_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


