# ChannelTypeMuteSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_ids** | **List[str]** |  | 
**mute_state** | **int** | &#x60;0&#x60; removes mute and &#x60;1&#x60; enables mute. | 
**channel_types** | **List[str]** | Channel types to apply (e.g. &#x60;PERSON&#x60;, &#x60;GROUP&#x60;, &#x60;CHATROOM&#x60;). Server validates against supported enums. | 

## Example

```python
from ncsdk.models.channel_type_mute_set_request import ChannelTypeMuteSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelTypeMuteSetRequest from a JSON string
channel_type_mute_set_request_instance = ChannelTypeMuteSetRequest.from_json(json)
# print the JSON string representation of the object
print(ChannelTypeMuteSetRequest.to_json())

# convert the object into a dict
channel_type_mute_set_request_dict = channel_type_mute_set_request_instance.to_dict()
# create an instance of ChannelTypeMuteSetRequest from a dict
channel_type_mute_set_request_from_dict = ChannelTypeMuteSetRequest.from_dict(channel_type_mute_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


