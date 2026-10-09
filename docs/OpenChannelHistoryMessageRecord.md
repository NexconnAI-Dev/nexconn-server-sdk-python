# OpenChannelHistoryMessageRecord


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** | Channel identifier of the stored message. | [optional] 
**from_user_id** | **str** | Sender user ID of the stored message. | [optional] 
**message_id** | **str** | Unique message ID. | [optional] 
**sent_at** | **int** | Message send timestamp in milliseconds. | [optional] 
**message_type** | **str** | Message type of the stored message. | [optional] 
**content** | **str** | Raw message content payload as stored by the service. | [optional] 
**quote** | **str** | Quoted message details as a JSON string containing msgUID, objectName and fromUserId. Omitted for messages without a quote. | [optional] 

## Example

```python
from ncsdk.models.open_channel_history_message_record import OpenChannelHistoryMessageRecord

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelHistoryMessageRecord from a JSON string
open_channel_history_message_record_instance = OpenChannelHistoryMessageRecord.from_json(json)
# print the JSON string representation of the object
print(OpenChannelHistoryMessageRecord.to_json())

# convert the object into a dict
open_channel_history_message_record_dict = open_channel_history_message_record_instance.to_dict()
# create an instance of OpenChannelHistoryMessageRecord from a dict
open_channel_history_message_record_from_dict = OpenChannelHistoryMessageRecord.from_dict(open_channel_history_message_record_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


