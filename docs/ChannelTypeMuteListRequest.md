# ChannelTypeMuteListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_size** | **int** |  | [optional] [default to 100]
**offset** | **int** |  | [optional] [default to 0]
**channel_type** | **str** |  | 

## Example

```python
from ncsdk.models.channel_type_mute_list_request import ChannelTypeMuteListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelTypeMuteListRequest from a JSON string
channel_type_mute_list_request_instance = ChannelTypeMuteListRequest.from_json(json)
# print the JSON string representation of the object
print(ChannelTypeMuteListRequest.to_json())

# convert the object into a dict
channel_type_mute_list_request_dict = channel_type_mute_list_request_instance.to_dict()
# create an instance of ChannelTypeMuteListRequest from a dict
channel_type_mute_list_request_from_dict = ChannelTypeMuteListRequest.from_dict(channel_type_mute_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


