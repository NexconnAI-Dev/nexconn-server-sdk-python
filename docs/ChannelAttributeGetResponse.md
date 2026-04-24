# ChannelAttributeGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**ChannelAttributeGetResponseResult**](ChannelAttributeGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.channel_attribute_get_response import ChannelAttributeGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelAttributeGetResponse from a JSON string
channel_attribute_get_response_instance = ChannelAttributeGetResponse.from_json(json)
# print the JSON string representation of the object
print(ChannelAttributeGetResponse.to_json())

# convert the object into a dict
channel_attribute_get_response_dict = channel_attribute_get_response_instance.to_dict()
# create an instance of ChannelAttributeGetResponse from a dict
channel_attribute_get_response_from_dict = ChannelAttributeGetResponse.from_dict(channel_attribute_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


