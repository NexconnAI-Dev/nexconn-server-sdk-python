# SystemChannelBroadcastOnlineRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from_user_id** | **str** |  | 
**message_type** | **str** |  | 
**content** | **str** |  | 
**disable_update_last_msg** | **bool** |  | [optional] 

## Example

```python
from ncsdk.models.system_channel_broadcast_online_request import SystemChannelBroadcastOnlineRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SystemChannelBroadcastOnlineRequest from a JSON string
system_channel_broadcast_online_request_instance = SystemChannelBroadcastOnlineRequest.from_json(json)
# print the JSON string representation of the object
print(SystemChannelBroadcastOnlineRequest.to_json())

# convert the object into a dict
system_channel_broadcast_online_request_dict = system_channel_broadcast_online_request_instance.to_dict()
# create an instance of SystemChannelBroadcastOnlineRequest from a dict
system_channel_broadcast_online_request_from_dict = SystemChannelBroadcastOnlineRequest.from_dict(system_channel_broadcast_online_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


