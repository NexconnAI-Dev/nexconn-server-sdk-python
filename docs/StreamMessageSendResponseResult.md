# StreamMessageSendResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_id** | **str** | Stream message unique ID. Only present in the response to the first chunk. | [optional] 

## Example

```python
from ncsdk.models.stream_message_send_response_result import StreamMessageSendResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of StreamMessageSendResponseResult from a JSON string
stream_message_send_response_result_instance = StreamMessageSendResponseResult.from_json(json)
# print the JSON string representation of the object
print(StreamMessageSendResponseResult.to_json())

# convert the object into a dict
stream_message_send_response_result_dict = stream_message_send_response_result_instance.to_dict()
# create an instance of StreamMessageSendResponseResult from a dict
stream_message_send_response_result_from_dict = StreamMessageSendResponseResult.from_dict(stream_message_send_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


