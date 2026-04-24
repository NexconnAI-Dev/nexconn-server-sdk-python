# SystemChannelMessageSendRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from_user_id** | **str** | Sender user ID. The sender should have an access token. | 
**to_user_ids** | **List[str]** | Recipient user IDs. Up to 100 users are supported in a single request. | 
**message_type** | **str** | Message type. Supports built-in types and custom types. Custom types must not start with &#x60;RC:&#x60; and must not exceed 32 characters. | 
**content** | **str** | Message content payload serialized as a string. Built-in message types should use a JSON object string. Maximum size is 128 KB. | 
**push_content** | **str** | Push notification text for offline recipients. Required for custom or notification messages that need push delivery. | [optional] 
**push_data** | **str** | Custom push payload data. Exposed as &#x60;appData&#x60; on iOS and Android. | [optional] 
**should_persist** | **int** | Whether to store the message in cloud message history. &#x60;0&#x60; means do not store and &#x60;1&#x60; means store. | [optional] 
**content_available** | **int** | iOS silent-push flag. &#x60;1&#x60; enables background delivery and &#x60;0&#x60; disables it. | [optional] 
**disable_push** | **bool** | Whether to suppress push notifications for offline recipients. | [optional] 
**push_ext** | **str** | Extended push configuration (JSON string as accepted by &#x60;SystemChannelMsgSendInput&#x60;). | [optional] 
**disable_update_last_msg** | **bool** | Whether to keep this message from updating the system channel&#39;s last-message preview. | [optional] 

## Example

```python
from ncsdk.models.system_channel_message_send_request import SystemChannelMessageSendRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SystemChannelMessageSendRequest from a JSON string
system_channel_message_send_request_instance = SystemChannelMessageSendRequest.from_json(json)
# print the JSON string representation of the object
print(SystemChannelMessageSendRequest.to_json())

# convert the object into a dict
system_channel_message_send_request_dict = system_channel_message_send_request_instance.to_dict()
# create an instance of SystemChannelMessageSendRequest from a dict
system_channel_message_send_request_from_dict = SystemChannelMessageSendRequest.from_dict(system_channel_message_send_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


