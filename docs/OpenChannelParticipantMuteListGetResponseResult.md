# OpenChannelParticipantMuteListGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**muted_participants** | [**List[OpenChannelMutedParticipantItem]**](OpenChannelMutedParticipantItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_participant_mute_list_get_response_result import OpenChannelParticipantMuteListGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelParticipantMuteListGetResponseResult from a JSON string
open_channel_participant_mute_list_get_response_result_instance = OpenChannelParticipantMuteListGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(OpenChannelParticipantMuteListGetResponseResult.to_json())

# convert the object into a dict
open_channel_participant_mute_list_get_response_result_dict = open_channel_participant_mute_list_get_response_result_instance.to_dict()
# create an instance of OpenChannelParticipantMuteListGetResponseResult from a dict
open_channel_participant_mute_list_get_response_result_from_dict = OpenChannelParticipantMuteListGetResponseResult.from_dict(open_channel_participant_mute_list_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


