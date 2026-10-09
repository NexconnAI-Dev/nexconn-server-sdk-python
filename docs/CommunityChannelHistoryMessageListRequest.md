# CommunityChannelHistoryMessageListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** | Community channel ID. | 
**subchannel_id** | **str** | Optional community subchannel ID. When omitted, messages from the whole community channel are queried. | [optional] 
**user_id** | **str** | User ID of the community-channel participant. | 
**start_at** | **int** | Query start timestamp in Unix milliseconds. Must be greater than or equal to &#x60;endAt&#x60;; the range cannot exceed 14 days. | 
**end_at** | **int** | Query end timestamp in Unix milliseconds. Messages are returned in descending timestamp order. | 
**page_size** | **int** | Number of messages to return. Must be between 1 and 100. | [optional] [default to 10]
**include_start** | **bool** | Whether to include the message at &#x60;startAt&#x60; when it matches the query boundary. | 

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


