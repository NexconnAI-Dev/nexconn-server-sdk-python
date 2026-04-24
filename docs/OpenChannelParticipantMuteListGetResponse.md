# OpenChannelParticipantMuteListGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**OpenChannelParticipantMuteListGetResponseResult**](OpenChannelParticipantMuteListGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_participant_mute_list_get_response import OpenChannelParticipantMuteListGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelParticipantMuteListGetResponse from a JSON string
open_channel_participant_mute_list_get_response_instance = OpenChannelParticipantMuteListGetResponse.from_json(json)
# print the JSON string representation of the object
print(OpenChannelParticipantMuteListGetResponse.to_json())

# convert the object into a dict
open_channel_participant_mute_list_get_response_dict = open_channel_participant_mute_list_get_response_instance.to_dict()
# create an instance of OpenChannelParticipantMuteListGetResponse from a dict
open_channel_participant_mute_list_get_response_from_dict = OpenChannelParticipantMuteListGetResponse.from_dict(open_channel_participant_mute_list_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


