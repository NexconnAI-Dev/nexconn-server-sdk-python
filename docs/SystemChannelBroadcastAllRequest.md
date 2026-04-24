# SystemChannelBroadcastAllRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from_user_id** | **str** |  | 
**message_type** | **str** |  | 
**content** | **str** |  | 
**push_content** | **str** |  | [optional] 
**push_data** | **str** |  | [optional] 
**content_available** | **int** |  | [optional] 
**push_ext** | **str** | Extended push configuration (JSON string as accepted by &#x60;MessageBroadcastInput&#x60;). | [optional] 
**disable_update_last_msg** | **bool** |  | [optional] 

## Example

```python
from ncsdk.models.system_channel_broadcast_all_request import SystemChannelBroadcastAllRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SystemChannelBroadcastAllRequest from a JSON string
system_channel_broadcast_all_request_instance = SystemChannelBroadcastAllRequest.from_json(json)
# print the JSON string representation of the object
print(SystemChannelBroadcastAllRequest.to_json())

# convert the object into a dict
system_channel_broadcast_all_request_dict = system_channel_broadcast_all_request_instance.to_dict()
# create an instance of SystemChannelBroadcastAllRequest from a dict
system_channel_broadcast_all_request_from_dict = SystemChannelBroadcastAllRequest.from_dict(system_channel_broadcast_all_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


