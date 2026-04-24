# MessageHistoryResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**messages** | [**List[MessageRecord]**](MessageRecord.md) |  | [optional] 

## Example

```python
from ncsdk.models.message_history_response_result import MessageHistoryResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of MessageHistoryResponseResult from a JSON string
message_history_response_result_instance = MessageHistoryResponseResult.from_json(json)
# print the JSON string representation of the object
print(MessageHistoryResponseResult.to_json())

# convert the object into a dict
message_history_response_result_dict = message_history_response_result_instance.to_dict()
# create an instance of MessageHistoryResponseResult from a dict
message_history_response_result_from_dict = MessageHistoryResponseResult.from_dict(message_history_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


