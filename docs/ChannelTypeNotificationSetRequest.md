# ChannelTypeNotificationSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_type** | **str** | Session / channel type as a string (&#x60;1&#x60; to &#x60;10&#x60; as accepted by the server). | 
**request_id** | **str** | User ID whose channel-type notification setting is updated. | 
**no_disturb_level** | **int** | Do-not-disturb level for the specified channel type. | 

## Example

```python
from ncsdk.models.channel_type_notification_set_request import ChannelTypeNotificationSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelTypeNotificationSetRequest from a JSON string
channel_type_notification_set_request_instance = ChannelTypeNotificationSetRequest.from_json(json)
# print the JSON string representation of the object
print(ChannelTypeNotificationSetRequest.to_json())

# convert the object into a dict
channel_type_notification_set_request_dict = channel_type_notification_set_request_instance.to_dict()
# create an instance of ChannelTypeNotificationSetRequest from a dict
channel_type_notification_set_request_from_dict = ChannelTypeNotificationSetRequest.from_dict(channel_type_notification_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


