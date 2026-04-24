# MessageRecord


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** | Channel identifier of the stored message. | [optional] 
**subchannel_id** | **str** | Community subchannel ID associated with the stored message, when applicable. | [optional] 
**from_user_id** | **str** | Sender user ID of the stored message. | [optional] 
**message_id** | **str** | Unique message ID. | [optional] 
**sent_at** | **int** | Message send timestamp in milliseconds. | [optional] 
**message_type** | **str** | Message type of the stored message. | [optional] 
**channel_type** | **int** | Channel type of the stored message. | [optional] 
**content** | **str** | Raw message content payload as stored by the service. | [optional] 
**has_metadata** | **bool** | Whether the message has metadata entries attached. | [optional] 
**metadata** | [**List[MessageMetadataListItem]**](MessageMetadataListItem.md) | List of metadata entries (&#x60;CommunityHistoryMessage&#x60; uses &#x60;List&lt;MetadataItem&gt;&#x60;, not a map). | [optional] 

## Example

```python
from ncsdk.models.message_record import MessageRecord

# TODO update the JSON string below
json = "{}"
# create an instance of MessageRecord from a JSON string
message_record_instance = MessageRecord.from_json(json)
# print the JSON string representation of the object
print(MessageRecord.to_json())

# convert the object into a dict
message_record_dict = message_record_instance.to_dict()
# create an instance of MessageRecord from a dict
message_record_from_dict = MessageRecord.from_dict(message_record_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


