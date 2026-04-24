# SystemChannelPushResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**SystemChannelPushResponseResult**](SystemChannelPushResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.system_channel_push_response import SystemChannelPushResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SystemChannelPushResponse from a JSON string
system_channel_push_response_instance = SystemChannelPushResponse.from_json(json)
# print the JSON string representation of the object
print(SystemChannelPushResponse.to_json())

# convert the object into a dict
system_channel_push_response_dict = system_channel_push_response_instance.to_dict()
# create an instance of SystemChannelPushResponse from a dict
system_channel_push_response_from_dict = SystemChannelPushResponse.from_dict(system_channel_push_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


