# StreamMessageSendResponse

Response for stream message send. The `result` field is only present in the response to the first chunk.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**StreamMessageSendResponseResult**](StreamMessageSendResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.stream_message_send_response import StreamMessageSendResponse

# TODO update the JSON string below
json = "{}"
# create an instance of StreamMessageSendResponse from a JSON string
stream_message_send_response_instance = StreamMessageSendResponse.from_json(json)
# print the JSON string representation of the object
print(StreamMessageSendResponse.to_json())

# convert the object into a dict
stream_message_send_response_dict = stream_message_send_response_instance.to_dict()
# create an instance of StreamMessageSendResponse from a dict
stream_message_send_response_from_dict = StreamMessageSendResponse.from_dict(stream_message_send_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


