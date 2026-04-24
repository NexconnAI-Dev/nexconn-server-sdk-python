# OpenChannelParticipantListByChannelRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 

## Example

```python
from ncsdk.models.open_channel_participant_list_by_channel_request import OpenChannelParticipantListByChannelRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelParticipantListByChannelRequest from a JSON string
open_channel_participant_list_by_channel_request_instance = OpenChannelParticipantListByChannelRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelParticipantListByChannelRequest.to_json())

# convert the object into a dict
open_channel_participant_list_by_channel_request_dict = open_channel_participant_list_by_channel_request_instance.to_dict()
# create an instance of OpenChannelParticipantListByChannelRequest from a dict
open_channel_participant_list_by_channel_request_from_dict = OpenChannelParticipantListByChannelRequest.from_dict(open_channel_participant_list_by_channel_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


