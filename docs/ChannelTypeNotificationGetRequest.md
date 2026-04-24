# ChannelTypeNotificationGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_type** | **str** | Session / channel type as a string (&#x60;1&#x60; to &#x60;10&#x60; as accepted by the server). | 
**request_id** | **str** | User ID whose channel-type notification setting is queried. | 

## Example

```python
from ncsdk.models.channel_type_notification_get_request import ChannelTypeNotificationGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelTypeNotificationGetRequest from a JSON string
channel_type_notification_get_request_instance = ChannelTypeNotificationGetRequest.from_json(json)
# print the JSON string representation of the object
print(ChannelTypeNotificationGetRequest.to_json())

# convert the object into a dict
channel_type_notification_get_request_dict = channel_type_notification_get_request_instance.to_dict()
# create an instance of ChannelTypeNotificationGetRequest from a dict
channel_type_notification_get_request_from_dict = ChannelTypeNotificationGetRequest.from_dict(channel_type_notification_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


