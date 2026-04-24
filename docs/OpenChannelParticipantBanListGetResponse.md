# OpenChannelParticipantBanListGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**OpenChannelParticipantBanListGetResponseResult**](OpenChannelParticipantBanListGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_participant_ban_list_get_response import OpenChannelParticipantBanListGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelParticipantBanListGetResponse from a JSON string
open_channel_participant_ban_list_get_response_instance = OpenChannelParticipantBanListGetResponse.from_json(json)
# print the JSON string representation of the object
print(OpenChannelParticipantBanListGetResponse.to_json())

# convert the object into a dict
open_channel_participant_ban_list_get_response_dict = open_channel_participant_ban_list_get_response_instance.to_dict()
# create an instance of OpenChannelParticipantBanListGetResponse from a dict
open_channel_participant_ban_list_get_response_from_dict = OpenChannelParticipantBanListGetResponse.from_dict(open_channel_participant_ban_list_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


