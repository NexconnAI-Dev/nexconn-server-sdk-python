# OpenChannelParticipantIdsResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**participant_ids** | **List[str]** |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_participant_ids_response_result import OpenChannelParticipantIdsResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelParticipantIdsResponseResult from a JSON string
open_channel_participant_ids_response_result_instance = OpenChannelParticipantIdsResponseResult.from_json(json)
# print the JSON string representation of the object
print(OpenChannelParticipantIdsResponseResult.to_json())

# convert the object into a dict
open_channel_participant_ids_response_result_dict = open_channel_participant_ids_response_result_instance.to_dict()
# create an instance of OpenChannelParticipantIdsResponseResult from a dict
open_channel_participant_ids_response_result_from_dict = OpenChannelParticipantIdsResponseResult.from_dict(open_channel_participant_ids_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


