# MessageDeleteRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from_user_id** | **str** | Sender user ID of the original message that is being deleted. | 
**channel_type** | **int** | Channel type of the original message. Supports &#x60;1&#x60; direct, &#x60;3&#x60; group, &#x60;4&#x60; open channel, &#x60;6&#x60; system, and &#x60;10&#x60; community. | 
**channel_id** | **str** | Target identifier of the original message. Depending on &#x60;channelType&#x60;, this can be a user ID, group ID, open channel ID, community channel ID, or system target ID. | 
**subchannel_id** | **str** | Community subchannel ID. Required only when deleting a community-channel message that was sent to a specific subchannel. | [optional] 
**message_id** | **str** | Unique message ID to delete. This corresponds to the message UID returned by send or routing services. | 
**sent_at** | **int** | Send timestamp of the original message in milliseconds. Providing it helps the service locate the original message precisely. | [optional] 
**is_admin** | **int** | Whether the deletion is performed as an admin operation. &#x60;1&#x60; shows an admin recall indicator and &#x60;0&#x60; performs a normal sender recall. | [optional] 
**disable_push** | **bool** | Whether to suppress push notifications for the recall event. Not supported for open channels or community channels. | [optional] 
**extra** | **str** | Custom extension data carried with the recall operation. Not supported for community channels. | [optional] 
**disable_update_last_msg** | **bool** | Whether to keep the recall operation from updating the channel&#39;s last-message preview. | [optional] 

## Example

```python
from ncsdk.models.message_delete_request import MessageDeleteRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MessageDeleteRequest from a JSON string
message_delete_request_instance = MessageDeleteRequest.from_json(json)
# print the JSON string representation of the object
print(MessageDeleteRequest.to_json())

# convert the object into a dict
message_delete_request_dict = message_delete_request_instance.to_dict()
# create an instance of MessageDeleteRequest from a dict
message_delete_request_from_dict = MessageDeleteRequest.from_dict(message_delete_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


