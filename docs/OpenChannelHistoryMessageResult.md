# OpenChannelHistoryMessageResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**messages** | [**List[OpenChannelHistoryMessageRecord]**](OpenChannelHistoryMessageRecord.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_history_message_result import OpenChannelHistoryMessageResult

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelHistoryMessageResult from a JSON string
open_channel_history_message_result_instance = OpenChannelHistoryMessageResult.from_json(json)
# print the JSON string representation of the object
print(OpenChannelHistoryMessageResult.to_json())

# convert the object into a dict
open_channel_history_message_result_dict = open_channel_history_message_result_instance.to_dict()
# create an instance of OpenChannelHistoryMessageResult from a dict
open_channel_history_message_result_from_dict = OpenChannelHistoryMessageResult.from_dict(open_channel_history_message_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


