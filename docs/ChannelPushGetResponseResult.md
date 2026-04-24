# ChannelPushGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**no_disturb_level** | **int** | Effective notification level for the specified channel. | [optional] 

## Example

```python
from ncsdk.models.channel_push_get_response_result import ChannelPushGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelPushGetResponseResult from a JSON string
channel_push_get_response_result_instance = ChannelPushGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(ChannelPushGetResponseResult.to_json())

# convert the object into a dict
channel_push_get_response_result_dict = channel_push_get_response_result_instance.to_dict()
# create an instance of ChannelPushGetResponseResult from a dict
channel_push_get_response_result_from_dict = ChannelPushGetResponseResult.from_dict(channel_push_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


