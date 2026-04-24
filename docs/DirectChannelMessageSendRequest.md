# DirectChannelMessageSendRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from_user_id** | **str** | Sender user ID. The sender should have an access token so push notifications can display sender information correctly. | 
**to_user_ids** | **List[str]** | Recipient user IDs. Up to 1000 users are supported in a single request. | 
**message_type** | **str** | Message type. Supports built-in types and custom types registered in the client SDK. Custom types must not start with &#x60;RC:&#x60; and must not exceed 32 characters. | 
**content** | **str** | Message content payload. Built-in message types should pass a JSON object serialized as a string. Maximum size is 128 KB. | 
**push_content** | **str** | Push notification text shown to offline recipients. Required for custom message types or notification/signal messages that need push delivery. | [optional] 
**push_data** | **str** | Custom payload included in the push notification. Exposed as &#x60;appData&#x60; on iOS and Android. | [optional] 
**is_echo_to_sender** | **int** | Whether to sync the message to the sender&#39;s client while the sender is online. &#x60;1&#x60; enables sync and &#x60;0&#x60; disables it. | [optional] 
**count** | **int** | Aligns with Java &#x60;DirectChannelMsgSendInput.count&#x60; (push/badge-related counter field name in server model). | [optional] 
**verify_blocklist** | **int** | Whether to filter recipients against the sender&#39;s blocklist. &#x60;0&#x60; means no filtering and &#x60;1&#x60; means filter blocked users out. | [optional] 
**should_persist** | **int** | Whether to store the message in recipient cloud history. &#x60;0&#x60; means do not store and &#x60;1&#x60; means store. | [optional] 
**content_available** | **int** | iOS silent-push flag. &#x60;1&#x60; enables background delivery and &#x60;0&#x60; disables it. | [optional] 
**has_metadata** | **bool** | Whether to enable message metadata (message expansion) for this message. | [optional] 
**metadata** | **Dict[str, object]** | Custom message metadata entries. Keys are limited to 32 characters and values to 4096 characters. | [optional] 
**disable_push** | **bool** | Whether to suppress push notifications for offline recipients. | [optional] 
**push_ext** | **str** | Extended push configuration (JSON string as accepted by &#x60;DirectChannelMsgSendInput&#x60;). | [optional] 
**disable_update_last_msg** | **bool** | Whether to keep this message from updating the channel&#39;s last-message preview. | [optional] 
**need_read_receipt** | **int** | Whether to request read receipts for this persisted message. &#x60;1&#x60; requests read receipts and &#x60;0&#x60; disables them. | [optional] 

## Example

```python
from ncsdk.models.direct_channel_message_send_request import DirectChannelMessageSendRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DirectChannelMessageSendRequest from a JSON string
direct_channel_message_send_request_instance = DirectChannelMessageSendRequest.from_json(json)
# print the JSON string representation of the object
print(DirectChannelMessageSendRequest.to_json())

# convert the object into a dict
direct_channel_message_send_request_dict = direct_channel_message_send_request_instance.to_dict()
# create an instance of DirectChannelMessageSendRequest from a dict
direct_channel_message_send_request_from_dict = DirectChannelMessageSendRequest.from_dict(direct_channel_message_send_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


