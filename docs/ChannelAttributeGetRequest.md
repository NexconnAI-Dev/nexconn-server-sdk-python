# ChannelAttributeGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**channel_id** | **str** |  | 
**channel_type** | **int** |  | 

## Example

```python
from ncsdk.models.channel_attribute_get_request import ChannelAttributeGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelAttributeGetRequest from a JSON string
channel_attribute_get_request_instance = ChannelAttributeGetRequest.from_json(json)
# print the JSON string representation of the object
print(ChannelAttributeGetRequest.to_json())

# convert the object into a dict
channel_attribute_get_request_dict = channel_attribute_get_request_instance.to_dict()
# create an instance of ChannelAttributeGetRequest from a dict
channel_attribute_get_request_from_dict = ChannelAttributeGetRequest.from_dict(channel_attribute_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


