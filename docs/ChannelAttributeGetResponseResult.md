# ChannelAttributeGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | [optional] 
**channel_type** | **int** |  | [optional] 
**pin** | [**ChannelPinState**](ChannelPinState.md) |  | [optional] 
**notification** | [**ChannelNotificationState**](ChannelNotificationState.md) |  | [optional] 
**tags** | [**List[ChannelAttributeTagItem]**](ChannelAttributeTagItem.md) | Same shape as &#x60;ChannelAttributeResult.TagInfo&#x60; (no &#x60;createdAt&#x60;; distinct from user tag list items). | [optional] 

## Example

```python
from ncsdk.models.channel_attribute_get_response_result import ChannelAttributeGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelAttributeGetResponseResult from a JSON string
channel_attribute_get_response_result_instance = ChannelAttributeGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(ChannelAttributeGetResponseResult.to_json())

# convert the object into a dict
channel_attribute_get_response_result_dict = channel_attribute_get_response_result_instance.to_dict()
# create an instance of ChannelAttributeGetResponseResult from a dict
channel_attribute_get_response_result_from_dict = ChannelAttributeGetResponseResult.from_dict(channel_attribute_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


