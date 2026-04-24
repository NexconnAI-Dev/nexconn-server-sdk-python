# ChannelTypeNotificationGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**ChannelTypeNotificationGetResponseResult**](ChannelTypeNotificationGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.channel_type_notification_get_response import ChannelTypeNotificationGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelTypeNotificationGetResponse from a JSON string
channel_type_notification_get_response_instance = ChannelTypeNotificationGetResponse.from_json(json)
# print the JSON string representation of the object
print(ChannelTypeNotificationGetResponse.to_json())

# convert the object into a dict
channel_type_notification_get_response_dict = channel_type_notification_get_response_instance.to_dict()
# create an instance of ChannelTypeNotificationGetResponse from a dict
channel_type_notification_get_response_from_dict = ChannelTypeNotificationGetResponse.from_dict(channel_type_notification_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


