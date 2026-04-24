# ChannelPinState


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_pinned** | **bool** |  | [optional] 
**pinned_at** | **int** |  | [optional] 

## Example

```python
from ncsdk.models.channel_pin_state import ChannelPinState

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelPinState from a JSON string
channel_pin_state_instance = ChannelPinState.from_json(json)
# print the JSON string representation of the object
print(ChannelPinState.to_json())

# convert the object into a dict
channel_pin_state_dict = channel_pin_state_instance.to_dict()
# create an instance of ChannelPinState from a dict
channel_pin_state_from_dict = ChannelPinState.from_dict(channel_pin_state_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


