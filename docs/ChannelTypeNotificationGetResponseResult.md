# ChannelTypeNotificationGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**no_disturb_level** | **int** | Effective notification level for the specified channel type. | [optional] 

## Example

```python
from ncsdk.models.channel_type_notification_get_response_result import ChannelTypeNotificationGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelTypeNotificationGetResponseResult from a JSON string
channel_type_notification_get_response_result_instance = ChannelTypeNotificationGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(ChannelTypeNotificationGetResponseResult.to_json())

# convert the object into a dict
channel_type_notification_get_response_result_dict = channel_type_notification_get_response_result_instance.to_dict()
# create an instance of ChannelTypeNotificationGetResponseResult from a dict
channel_type_notification_get_response_result_from_dict = ChannelTypeNotificationGetResponseResult.from_dict(channel_type_notification_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


