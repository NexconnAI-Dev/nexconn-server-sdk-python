# OpenChannelHistoryMessageResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**OpenChannelHistoryMessageResult**](OpenChannelHistoryMessageResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_history_message_response import OpenChannelHistoryMessageResponse

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelHistoryMessageResponse from a JSON string
open_channel_history_message_response_instance = OpenChannelHistoryMessageResponse.from_json(json)
# print the JSON string representation of the object
print(OpenChannelHistoryMessageResponse.to_json())

# convert the object into a dict
open_channel_history_message_response_dict = open_channel_history_message_response_instance.to_dict()
# create an instance of OpenChannelHistoryMessageResponse from a dict
open_channel_history_message_response_from_dict = OpenChannelHistoryMessageResponse.from_dict(open_channel_history_message_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


