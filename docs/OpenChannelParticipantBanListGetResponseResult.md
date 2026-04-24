# OpenChannelParticipantBanListGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**banned_participants** | [**List[OpenChannelBannedParticipantItem]**](OpenChannelBannedParticipantItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_participant_ban_list_get_response_result import OpenChannelParticipantBanListGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelParticipantBanListGetResponseResult from a JSON string
open_channel_participant_ban_list_get_response_result_instance = OpenChannelParticipantBanListGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(OpenChannelParticipantBanListGetResponseResult.to_json())

# convert the object into a dict
open_channel_participant_ban_list_get_response_result_dict = open_channel_participant_ban_list_get_response_result_instance.to_dict()
# create an instance of OpenChannelParticipantBanListGetResponseResult from a dict
open_channel_participant_ban_list_get_response_result_from_dict = OpenChannelParticipantBanListGetResponseResult.from_dict(open_channel_participant_ban_list_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


