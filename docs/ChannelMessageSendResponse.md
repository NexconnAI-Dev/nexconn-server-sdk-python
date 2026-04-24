# ChannelMessageSendResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**ChannelMessageSendResponseResult**](ChannelMessageSendResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.channel_message_send_response import ChannelMessageSendResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelMessageSendResponse from a JSON string
channel_message_send_response_instance = ChannelMessageSendResponse.from_json(json)
# print the JSON string representation of the object
print(ChannelMessageSendResponse.to_json())

# convert the object into a dict
channel_message_send_response_dict = channel_message_send_response_instance.to_dict()
# create an instance of ChannelMessageSendResponse from a dict
channel_message_send_response_from_dict = ChannelMessageSendResponse.from_dict(channel_message_send_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


