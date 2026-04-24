# MessageChannelDelivery


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | [optional] 
**message_id** | **str** |  | [optional] 

## Example

```python
from ncsdk.models.message_channel_delivery import MessageChannelDelivery

# TODO update the JSON string below
json = "{}"
# create an instance of MessageChannelDelivery from a JSON string
message_channel_delivery_instance = MessageChannelDelivery.from_json(json)
# print the JSON string representation of the object
print(MessageChannelDelivery.to_json())

# convert the object into a dict
message_channel_delivery_dict = message_channel_delivery_instance.to_dict()
# create an instance of MessageChannelDelivery from a dict
message_channel_delivery_from_dict = MessageChannelDelivery.from_dict(message_channel_delivery_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


