# DirectGroupHistoryMessageRecord


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** | Channel identifier of the stored message. | [optional] 
**from_user_id** | **str** | Sender user ID of the stored message. | [optional] 
**message_id** | **str** | Unique message ID. | [optional] 
**sent_at** | **int** | Message send timestamp in milliseconds. | [optional] 
**message_type** | **str** | Message type of the stored message. | [optional] 
**content** | **str** | Raw message content payload as stored by the service. | [optional] 
**has_metadata** | **bool** | Whether the message has metadata entries attached. | [optional] 
**metadata** | [**List[MessageMetadataListItem]**](MessageMetadataListItem.md) | Structured message metadata entries. Omitted when the original metadata is empty or cannot be parsed. | [optional] 
**ai_generated** | **bool** | Whether the message was AI-generated. Returned only for direct and group channels when the application has enabled this capability. | [optional] 
**quote** | **str** | Quoted message details as a JSON string containing msgUID, objectName and fromUserId. Omitted for messages without a quote. | [optional] 

## Example

```python
from ncsdk.models.direct_group_history_message_record import DirectGroupHistoryMessageRecord

# TODO update the JSON string below
json = "{}"
# create an instance of DirectGroupHistoryMessageRecord from a JSON string
direct_group_history_message_record_instance = DirectGroupHistoryMessageRecord.from_json(json)
# print the JSON string representation of the object
print(DirectGroupHistoryMessageRecord.to_json())

# convert the object into a dict
direct_group_history_message_record_dict = direct_group_history_message_record_instance.to_dict()
# create an instance of DirectGroupHistoryMessageRecord from a dict
direct_group_history_message_record_from_dict = DirectGroupHistoryMessageRecord.from_dict(direct_group_history_message_record_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


