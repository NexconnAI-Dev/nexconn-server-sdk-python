# OpenChannelFreezeListUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**extra** | **str** | Notification extra payload in JSON string format. | [optional] 
**need_notify** | **bool** |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_freeze_list_update_request import OpenChannelFreezeListUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelFreezeListUpdateRequest from a JSON string
open_channel_freeze_list_update_request_instance = OpenChannelFreezeListUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelFreezeListUpdateRequest.to_json())

# convert the object into a dict
open_channel_freeze_list_update_request_dict = open_channel_freeze_list_update_request_instance.to_dict()
# create an instance of OpenChannelFreezeListUpdateRequest from a dict
open_channel_freeze_list_update_request_from_dict = OpenChannelFreezeListUpdateRequest.from_dict(open_channel_freeze_list_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


