# ChannelPushGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**ChannelPushGetResponseResult**](ChannelPushGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.channel_push_get_response import ChannelPushGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelPushGetResponse from a JSON string
channel_push_get_response_instance = ChannelPushGetResponse.from_json(json)
# print the JSON string representation of the object
print(ChannelPushGetResponse.to_json())

# convert the object into a dict
channel_push_get_response_dict = channel_push_get_response_instance.to_dict()
# create an instance of ChannelPushGetResponse from a dict
channel_push_get_response_from_dict = ChannelPushGetResponse.from_dict(channel_push_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


