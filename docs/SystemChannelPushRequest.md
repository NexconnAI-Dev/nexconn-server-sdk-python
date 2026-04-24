# SystemChannelPushRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**platform** | **List[str]** |  | 
**from_user_id** | **str** |  | 
**audience** | [**SystemChannelPushAudience**](SystemChannelPushAudience.md) |  | 
**message** | [**SystemChannelPushMessage**](SystemChannelPushMessage.md) |  | 
**notification** | [**SystemChannelPushNotification**](SystemChannelPushNotification.md) |  | 

## Example

```python
from ncsdk.models.system_channel_push_request import SystemChannelPushRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SystemChannelPushRequest from a JSON string
system_channel_push_request_instance = SystemChannelPushRequest.from_json(json)
# print the JSON string representation of the object
print(SystemChannelPushRequest.to_json())

# convert the object into a dict
system_channel_push_request_dict = system_channel_push_request_instance.to_dict()
# create an instance of SystemChannelPushRequest from a dict
system_channel_push_request_from_dict = SystemChannelPushRequest.from_dict(system_channel_push_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


