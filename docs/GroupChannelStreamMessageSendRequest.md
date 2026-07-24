# GroupChannelStreamMessageSendRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from_user_id** | **str** | Sender user ID. | 
**to_channel_id** | **str** | Target group channel ID. | 
**message_type** | **str** | Message type. Fixed value &#x60;RC:StreamMsg&#x60; for stream messages. | 
**content** | [**StreamMessageContent**](StreamMessageContent.md) |  | 
**to_user_ids** | **List[str]** | Recipient member user IDs for a targeted group message. Up to 10 users. | [optional] 
**is_echo_to_sender** | **int** | Whether to sync the message to the sender&#39;s client while the sender is online. &#x60;1&#x60; enables sync and &#x60;0&#x60; disables it. | [optional] 
**should_persist** | **int** | Whether to store the message in cloud message history. &#x60;0&#x60; means do not store and &#x60;1&#x60; means store. | [optional] 
**has_mention** | **int** | Whether this is an @mention message. Set to &#x60;1&#x60; when &#x60;content&#x60; contains &#x60;mentionedInfo&#x60;. | [optional] 
**metadata** | **Dict[str, str]** | Custom message metadata entries. Keys are limited to 32 characters and values to 4096 characters. Up to 100 key-value pairs. | [optional] 
**disable_update_last_msg** | **bool** | Whether to keep this message from updating the channel&#39;s last-message preview. | [optional] 

## Example

```python
from ncsdk.models.group_channel_stream_message_send_request import GroupChannelStreamMessageSendRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelStreamMessageSendRequest from a JSON string
group_channel_stream_message_send_request_instance = GroupChannelStreamMessageSendRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelStreamMessageSendRequest.to_json())

# convert the object into a dict
group_channel_stream_message_send_request_dict = group_channel_stream_message_send_request_instance.to_dict()
# create an instance of GroupChannelStreamMessageSendRequest from a dict
group_channel_stream_message_send_request_from_dict = GroupChannelStreamMessageSendRequest.from_dict(group_channel_stream_message_send_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


