# OpenChannelBroadcastRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from_user_id** | **str** | Sender user ID. | 
**message_type** | **str** | Message type. Supports built-in types and custom types registered in the client SDK. Custom types must not start with &#x60;RC:&#x60; and must not exceed 32 characters. | 
**content** | **str** | Broadcast message payload serialized as a string. Maximum size is 128 KB. | 
**is_echo_to_sender** | **int** | Whether to sync the broadcast message to the sender&#39;s client while the sender is online. | [optional] 

## Example

```python
from ncsdk.models.open_channel_broadcast_request import OpenChannelBroadcastRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelBroadcastRequest from a JSON string
open_channel_broadcast_request_instance = OpenChannelBroadcastRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelBroadcastRequest.to_json())

# convert the object into a dict
open_channel_broadcast_request_dict = open_channel_broadcast_request_instance.to_dict()
# create an instance of OpenChannelBroadcastRequest from a dict
open_channel_broadcast_request_from_dict = OpenChannelBroadcastRequest.from_dict(open_channel_broadcast_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


