# MessageUserDelivery


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**message_id** | **str** |  | [optional] 

## Example

```python
from ncsdk.models.message_user_delivery import MessageUserDelivery

# TODO update the JSON string below
json = "{}"
# create an instance of MessageUserDelivery from a JSON string
message_user_delivery_instance = MessageUserDelivery.from_json(json)
# print the JSON string representation of the object
print(MessageUserDelivery.to_json())

# convert the object into a dict
message_user_delivery_dict = message_user_delivery_instance.to_dict()
# create an instance of MessageUserDelivery from a dict
message_user_delivery_from_dict = MessageUserDelivery.from_dict(message_user_delivery_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


