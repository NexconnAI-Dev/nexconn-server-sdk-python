# ChannelMessageHistoryDeleteRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_type** | **int** | Channel type. Supports &#x60;1&#x60; direct, &#x60;3&#x60; group, &#x60;4&#x60; open channel, and &#x60;6&#x60; system (&#x60;HistoryCleanInput&#x60;). | 
**from_user_id** | **str** | User whose server-side history is operated on. For open channels, this is the operator ID. | 
**channel_id** | **str** | Target channel ID (&#x60;targetId&#x60; / conversation target). | 
**sent_at** | **str** | Optional cutoff (&#x60;msgTimestamp&#x60;). Serialized as string in &#x60;HistoryCleanInput&#x60;. | [optional] 

## Example

```python
from ncsdk.models.channel_message_history_delete_request import ChannelMessageHistoryDeleteRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelMessageHistoryDeleteRequest from a JSON string
channel_message_history_delete_request_instance = ChannelMessageHistoryDeleteRequest.from_json(json)
# print the JSON string representation of the object
print(ChannelMessageHistoryDeleteRequest.to_json())

# convert the object into a dict
channel_message_history_delete_request_dict = channel_message_history_delete_request_instance.to_dict()
# create an instance of ChannelMessageHistoryDeleteRequest from a dict
channel_message_history_delete_request_from_dict = ChannelMessageHistoryDeleteRequest.from_dict(channel_message_history_delete_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


