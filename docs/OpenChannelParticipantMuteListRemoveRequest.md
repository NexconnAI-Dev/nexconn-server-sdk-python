# OpenChannelParticipantMuteListRemoveRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**participant_ids** | **List[str]** |  | 
**extra** | **str** | Notification extra payload in JSON string format. | [optional] 
**need_notify** | **bool** |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_participant_mute_list_remove_request import OpenChannelParticipantMuteListRemoveRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelParticipantMuteListRemoveRequest from a JSON string
open_channel_participant_mute_list_remove_request_instance = OpenChannelParticipantMuteListRemoveRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelParticipantMuteListRemoveRequest.to_json())

# convert the object into a dict
open_channel_participant_mute_list_remove_request_dict = open_channel_participant_mute_list_remove_request_instance.to_dict()
# create an instance of OpenChannelParticipantMuteListRemoveRequest from a dict
open_channel_participant_mute_list_remove_request_from_dict = OpenChannelParticipantMuteListRemoveRequest.from_dict(open_channel_participant_mute_list_remove_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


