# OpenChannelGlobalMuteListAddRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**participant_ids** | **List[str]** |  | 
**duration_minutes** | **int** |  | 
**extra** | **str** | Notification extra payload in JSON string format. | [optional] 
**need_notify** | **bool** |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_global_mute_list_add_request import OpenChannelGlobalMuteListAddRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelGlobalMuteListAddRequest from a JSON string
open_channel_global_mute_list_add_request_instance = OpenChannelGlobalMuteListAddRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelGlobalMuteListAddRequest.to_json())

# convert the object into a dict
open_channel_global_mute_list_add_request_dict = open_channel_global_mute_list_add_request_instance.to_dict()
# create an instance of OpenChannelGlobalMuteListAddRequest from a dict
open_channel_global_mute_list_add_request_from_dict = OpenChannelGlobalMuteListAddRequest.from_dict(open_channel_global_mute_list_add_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


