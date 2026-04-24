# ChannelPinSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**channel_type** | **int** | Legacy &#x60;conversationType&#x60;. Current docs use numeric channel types such as &#x60;1&#x60;, &#x60;3&#x60;, and &#x60;6&#x60;. | 
**channel_id** | **str** | Legacy &#x60;targetId&#x60;. | 
**is_pin** | **bool** | JSON field name used by the server. &#x60;true&#x60; pins the conversation and &#x60;false&#x60; cancels the pin. | 

## Example

```python
from ncsdk.models.channel_pin_set_request import ChannelPinSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelPinSetRequest from a JSON string
channel_pin_set_request_instance = ChannelPinSetRequest.from_json(json)
# print the JSON string representation of the object
print(ChannelPinSetRequest.to_json())

# convert the object into a dict
channel_pin_set_request_dict = channel_pin_set_request_instance.to_dict()
# create an instance of ChannelPinSetRequest from a dict
channel_pin_set_request_from_dict = ChannelPinSetRequest.from_dict(channel_pin_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


