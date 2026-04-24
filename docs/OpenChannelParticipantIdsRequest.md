# OpenChannelParticipantIdsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**participant_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.open_channel_participant_ids_request import OpenChannelParticipantIdsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelParticipantIdsRequest from a JSON string
open_channel_participant_ids_request_instance = OpenChannelParticipantIdsRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelParticipantIdsRequest.to_json())

# convert the object into a dict
open_channel_participant_ids_request_dict = open_channel_participant_ids_request_instance.to_dict()
# create an instance of OpenChannelParticipantIdsRequest from a dict
open_channel_participant_ids_request_from_dict = OpenChannelParticipantIdsRequest.from_dict(open_channel_participant_ids_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


