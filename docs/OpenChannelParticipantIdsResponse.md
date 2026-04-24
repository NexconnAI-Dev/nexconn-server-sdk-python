# OpenChannelParticipantIdsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**OpenChannelParticipantIdsResponseResult**](OpenChannelParticipantIdsResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_participant_ids_response import OpenChannelParticipantIdsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelParticipantIdsResponse from a JSON string
open_channel_participant_ids_response_instance = OpenChannelParticipantIdsResponse.from_json(json)
# print the JSON string representation of the object
print(OpenChannelParticipantIdsResponse.to_json())

# convert the object into a dict
open_channel_participant_ids_response_dict = open_channel_participant_ids_response_instance.to_dict()
# create an instance of OpenChannelParticipantIdsResponse from a dict
open_channel_participant_ids_response_from_dict = OpenChannelParticipantIdsResponse.from_dict(open_channel_participant_ids_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


