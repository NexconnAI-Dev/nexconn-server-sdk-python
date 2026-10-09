# DirectGroupHistoryMessageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**DirectGroupHistoryMessageResult**](DirectGroupHistoryMessageResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.direct_group_history_message_response import DirectGroupHistoryMessageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of DirectGroupHistoryMessageResponse from a JSON string
direct_group_history_message_response_instance = DirectGroupHistoryMessageResponse.from_json(json)
# print the JSON string representation of the object
print(DirectGroupHistoryMessageResponse.to_json())

# convert the object into a dict
direct_group_history_message_response_dict = direct_group_history_message_response_instance.to_dict()
# create an instance of DirectGroupHistoryMessageResponse from a dict
direct_group_history_message_response_from_dict = DirectGroupHistoryMessageResponse.from_dict(direct_group_history_message_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


