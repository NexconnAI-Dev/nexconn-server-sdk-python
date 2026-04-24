# OpenChannelParticipantExistResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**participants** | [**List[OpenChannelParticipantExistItem]**](OpenChannelParticipantExistItem.md) | Array of participant check results. | [optional] 

## Example

```python
from ncsdk.models.open_channel_participant_exist_response_result import OpenChannelParticipantExistResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelParticipantExistResponseResult from a JSON string
open_channel_participant_exist_response_result_instance = OpenChannelParticipantExistResponseResult.from_json(json)
# print the JSON string representation of the object
print(OpenChannelParticipantExistResponseResult.to_json())

# convert the object into a dict
open_channel_participant_exist_response_result_dict = open_channel_participant_exist_response_result_instance.to_dict()
# create an instance of OpenChannelParticipantExistResponseResult from a dict
open_channel_participant_exist_response_result_from_dict = OpenChannelParticipantExistResponseResult.from_dict(open_channel_participant_exist_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


