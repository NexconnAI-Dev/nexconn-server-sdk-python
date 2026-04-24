# SystemChannelPushResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**message_id** | **str** |  | [optional] 

## Example

```python
from ncsdk.models.system_channel_push_response_result import SystemChannelPushResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of SystemChannelPushResponseResult from a JSON string
system_channel_push_response_result_instance = SystemChannelPushResponseResult.from_json(json)
# print the JSON string representation of the object
print(SystemChannelPushResponseResult.to_json())

# convert the object into a dict
system_channel_push_response_result_dict = system_channel_push_response_result_instance.to_dict()
# create an instance of SystemChannelPushResponseResult from a dict
system_channel_push_response_result_from_dict = SystemChannelPushResponseResult.from_dict(system_channel_push_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


