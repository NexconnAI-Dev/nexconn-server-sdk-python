# OpenChannelMessageSendRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from_user_id** | **str** | Sender user ID. | 
**to_channel_ids** | **List[str]** | Target open channel IDs. Multiple channels are allowed; the official documentation recommends up to 10 IDs per request. | 
**message_type** | **str** | Message type. Supports built-in types and custom types registered in the client SDK. Custom types must not start with &#x60;RC:&#x60; and must not exceed 32 characters. | 
**content** | **str** | Message content payload serialized as a string. Built-in message types should use a JSON object string. Maximum size is 128 KB. | 
**should_persist** | **int** | Whether to store the message in open channel cloud history. &#x60;0&#x60; means do not store and &#x60;1&#x60; means store. | [optional] 
**is_echo_to_sender** | **int** | Whether to sync the sent message to the sender&#39;s client while online. &#x60;1&#x60; enables sync and &#x60;0&#x60; disables it. | [optional] 
**priority** | **int** | Message priority. &#x60;0&#x60; standard, &#x60;1&#x60; allowlisted, &#x60;2&#x60; high priority, &#x60;3&#x60; low priority. | [optional] 

## Example

```python
from ncsdk.models.open_channel_message_send_request import OpenChannelMessageSendRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelMessageSendRequest from a JSON string
open_channel_message_send_request_instance = OpenChannelMessageSendRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelMessageSendRequest.to_json())

# convert the object into a dict
open_channel_message_send_request_dict = open_channel_message_send_request_instance.to_dict()
# create an instance of OpenChannelMessageSendRequest from a dict
open_channel_message_send_request_from_dict = OpenChannelMessageSendRequest.from_dict(open_channel_message_send_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


