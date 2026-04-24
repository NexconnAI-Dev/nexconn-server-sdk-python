# OpenChannelParticipantListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | **int** |  | [optional] 
**participants** | [**List[OpenChannelParticipantItem]**](OpenChannelParticipantItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_participant_list_response_result import OpenChannelParticipantListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelParticipantListResponseResult from a JSON string
open_channel_participant_list_response_result_instance = OpenChannelParticipantListResponseResult.from_json(json)
# print the JSON string representation of the object
print(OpenChannelParticipantListResponseResult.to_json())

# convert the object into a dict
open_channel_participant_list_response_result_dict = open_channel_participant_list_response_result_instance.to_dict()
# create an instance of OpenChannelParticipantListResponseResult from a dict
open_channel_participant_list_response_result_from_dict = OpenChannelParticipantListResponseResult.from_dict(open_channel_participant_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


