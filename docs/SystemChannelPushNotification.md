# SystemChannelPushNotification


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** |  | [optional] 
**force_show_push_content** | **int** |  | [optional] 
**alert** | **str** |  | [optional] 
**ios** | **Dict[str, object]** |  | [optional] 
**android** | **Dict[str, object]** |  | [optional] 
**harmony_os** | **Dict[str, object]** |  | [optional] 

## Example

```python
from ncsdk.models.system_channel_push_notification import SystemChannelPushNotification

# TODO update the JSON string below
json = "{}"
# create an instance of SystemChannelPushNotification from a JSON string
system_channel_push_notification_instance = SystemChannelPushNotification.from_json(json)
# print the JSON string representation of the object
print(SystemChannelPushNotification.to_json())

# convert the object into a dict
system_channel_push_notification_dict = system_channel_push_notification_instance.to_dict()
# create an instance of SystemChannelPushNotification from a dict
system_channel_push_notification_from_dict = SystemChannelPushNotification.from_dict(system_channel_push_notification_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


