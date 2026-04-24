# OpenChannelParticipantListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**page_size** | **int** |  | [optional] 
**order** | **int** | &#x60;1&#x60; for ascending join time and &#x60;2&#x60; for descending join time. | [optional] 

## Example

```python
from ncsdk.models.open_channel_participant_list_request import OpenChannelParticipantListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelParticipantListRequest from a JSON string
open_channel_participant_list_request_instance = OpenChannelParticipantListRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelParticipantListRequest.to_json())

# convert the object into a dict
open_channel_participant_list_request_dict = open_channel_participant_list_request_instance.to_dict()
# create an instance of OpenChannelParticipantListRequest from a dict
open_channel_participant_list_request_from_dict = OpenChannelParticipantListRequest.from_dict(open_channel_participant_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


