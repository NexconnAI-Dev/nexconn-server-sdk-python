# OpenChannelMessageTypeListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_types** | **List[str]** |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_message_type_list_response_result import OpenChannelMessageTypeListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelMessageTypeListResponseResult from a JSON string
open_channel_message_type_list_response_result_instance = OpenChannelMessageTypeListResponseResult.from_json(json)
# print the JSON string representation of the object
print(OpenChannelMessageTypeListResponseResult.to_json())

# convert the object into a dict
open_channel_message_type_list_response_result_dict = open_channel_message_type_list_response_result_instance.to_dict()
# create an instance of OpenChannelMessageTypeListResponseResult from a dict
open_channel_message_type_list_response_result_from_dict = OpenChannelMessageTypeListResponseResult.from_dict(open_channel_message_type_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


