# ChannelMessageSendResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_ids** | [**List[MessageChannelDelivery]**](MessageChannelDelivery.md) |  | [optional] 

## Example

```python
from ncsdk.models.channel_message_send_response_result import ChannelMessageSendResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelMessageSendResponseResult from a JSON string
channel_message_send_response_result_instance = ChannelMessageSendResponseResult.from_json(json)
# print the JSON string representation of the object
print(ChannelMessageSendResponseResult.to_json())

# convert the object into a dict
channel_message_send_response_result_dict = channel_message_send_response_result_instance.to_dict()
# create an instance of ChannelMessageSendResponseResult from a dict
channel_message_send_response_result_from_dict = ChannelMessageSendResponseResult.from_dict(channel_message_send_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


