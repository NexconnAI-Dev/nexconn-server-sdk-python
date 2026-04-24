# OpenChannelParticipantExistRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** | The open channel ID. | 
**participant_ids** | **List[str]** | User IDs to check. Up to 1,000 users per request. Pass a single-element array to check one user. | 

## Example

```python
from ncsdk.models.open_channel_participant_exist_request import OpenChannelParticipantExistRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelParticipantExistRequest from a JSON string
open_channel_participant_exist_request_instance = OpenChannelParticipantExistRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelParticipantExistRequest.to_json())

# convert the object into a dict
open_channel_participant_exist_request_dict = open_channel_participant_exist_request_instance.to_dict()
# create an instance of OpenChannelParticipantExistRequest from a dict
open_channel_participant_exist_request_from_dict = OpenChannelParticipantExistRequest.from_dict(open_channel_participant_exist_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


