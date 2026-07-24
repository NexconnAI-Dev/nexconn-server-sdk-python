# DirectChannelStreamMessageSendRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from_user_id** | **str** | Sender user ID. The sender should have an access token so push notifications can display sender information correctly. | 
**to_user_id** | **str** | Recipient user ID. Only a single recipient is supported per stream message. | 
**message_type** | **str** | Message type. Fixed value &#x60;RC:StreamMsg&#x60; for stream messages. | 
**content** | [**StreamMessageContent**](StreamMessageContent.md) |  | 
**is_echo_to_sender** | **int** | Whether to sync the message to the sender&#39;s client while the sender is online. &#x60;1&#x60; enables sync and &#x60;0&#x60; disables it. | [optional] 
**should_persist** | **int** | Whether to store the message in recipient cloud history. &#x60;0&#x60; means do not store and &#x60;1&#x60; means store. | [optional] 
**metadata** | **Dict[str, str]** | Custom message metadata entries. Keys are limited to 32 characters and values to 4096 characters. Up to 100 key-value pairs. | [optional] 
**disable_update_last_msg** | **bool** | Whether to keep this message from updating the channel&#39;s last-message preview. | [optional] 

## Example

```python
from ncsdk.models.direct_channel_stream_message_send_request import DirectChannelStreamMessageSendRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DirectChannelStreamMessageSendRequest from a JSON string
direct_channel_stream_message_send_request_instance = DirectChannelStreamMessageSendRequest.from_json(json)
# print the JSON string representation of the object
print(DirectChannelStreamMessageSendRequest.to_json())

# convert the object into a dict
direct_channel_stream_message_send_request_dict = direct_channel_stream_message_send_request_instance.to_dict()
# create an instance of DirectChannelStreamMessageSendRequest from a dict
direct_channel_stream_message_send_request_from_dict = DirectChannelStreamMessageSendRequest.from_dict(direct_channel_stream_message_send_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


