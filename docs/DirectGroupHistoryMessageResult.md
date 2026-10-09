# DirectGroupHistoryMessageResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**messages** | [**List[DirectGroupHistoryMessageRecord]**](DirectGroupHistoryMessageRecord.md) |  | [optional] 

## Example

```python
from ncsdk.models.direct_group_history_message_result import DirectGroupHistoryMessageResult

# TODO update the JSON string below
json = "{}"
# create an instance of DirectGroupHistoryMessageResult from a JSON string
direct_group_history_message_result_instance = DirectGroupHistoryMessageResult.from_json(json)
# print the JSON string representation of the object
print(DirectGroupHistoryMessageResult.to_json())

# convert the object into a dict
direct_group_history_message_result_dict = direct_group_history_message_result_instance.to_dict()
# create an instance of DirectGroupHistoryMessageResult from a dict
direct_group_history_message_result_from_dict = DirectGroupHistoryMessageResult.from_dict(direct_group_history_message_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


