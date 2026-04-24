# SystemChannelBroadcastDeleteRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from_user_id** | **str** |  | 
**message_id** | **str** |  | 
**sent_at** | **int** |  | [optional] 
**is_admin** | **int** |  | [optional] 
**extra** | **str** |  | [optional] 
**disable_update_last_msg** | **bool** |  | [optional] 

## Example

```python
from ncsdk.models.system_channel_broadcast_delete_request import SystemChannelBroadcastDeleteRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SystemChannelBroadcastDeleteRequest from a JSON string
system_channel_broadcast_delete_request_instance = SystemChannelBroadcastDeleteRequest.from_json(json)
# print the JSON string representation of the object
print(SystemChannelBroadcastDeleteRequest.to_json())

# convert the object into a dict
system_channel_broadcast_delete_request_dict = system_channel_broadcast_delete_request_instance.to_dict()
# create an instance of SystemChannelBroadcastDeleteRequest from a dict
system_channel_broadcast_delete_request_from_dict = SystemChannelBroadcastDeleteRequest.from_dict(system_channel_broadcast_delete_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


