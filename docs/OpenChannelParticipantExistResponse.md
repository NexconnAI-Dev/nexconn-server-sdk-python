# OpenChannelParticipantExistResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** | Return code. &#x60;0&#x60; indicates success. | 
**result** | [**OpenChannelParticipantExistResponseResult**](OpenChannelParticipantExistResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_participant_exist_response import OpenChannelParticipantExistResponse

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelParticipantExistResponse from a JSON string
open_channel_participant_exist_response_instance = OpenChannelParticipantExistResponse.from_json(json)
# print the JSON string representation of the object
print(OpenChannelParticipantExistResponse.to_json())

# convert the object into a dict
open_channel_participant_exist_response_dict = open_channel_participant_exist_response_instance.to_dict()
# create an instance of OpenChannelParticipantExistResponse from a dict
open_channel_participant_exist_response_from_dict = OpenChannelParticipantExistResponse.from_dict(open_channel_participant_exist_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


