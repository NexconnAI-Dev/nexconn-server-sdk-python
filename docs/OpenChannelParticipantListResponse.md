# OpenChannelParticipantListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**OpenChannelParticipantListResponseResult**](OpenChannelParticipantListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_participant_list_response import OpenChannelParticipantListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelParticipantListResponse from a JSON string
open_channel_participant_list_response_instance = OpenChannelParticipantListResponse.from_json(json)
# print the JSON string representation of the object
print(OpenChannelParticipantListResponse.to_json())

# convert the object into a dict
open_channel_participant_list_response_dict = open_channel_participant_list_response_instance.to_dict()
# create an instance of OpenChannelParticipantListResponse from a dict
open_channel_participant_list_response_from_dict = OpenChannelParticipantListResponse.from_dict(open_channel_participant_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


