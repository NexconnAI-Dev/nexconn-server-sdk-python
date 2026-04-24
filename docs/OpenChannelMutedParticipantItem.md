# OpenChannelMutedParticipantItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**participant_id** | **str** |  | [optional] 
**mute_expires_at** | **str** | Mute expiration time in &#x60;YYYY-MM-DD HH:MM:SS&#x60; format. | [optional] 

## Example

```python
from ncsdk.models.open_channel_muted_participant_item import OpenChannelMutedParticipantItem

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelMutedParticipantItem from a JSON string
open_channel_muted_participant_item_instance = OpenChannelMutedParticipantItem.from_json(json)
# print the JSON string representation of the object
print(OpenChannelMutedParticipantItem.to_json())

# convert the object into a dict
open_channel_muted_participant_item_dict = open_channel_muted_participant_item_instance.to_dict()
# create an instance of OpenChannelMutedParticipantItem from a dict
open_channel_muted_participant_item_from_dict = OpenChannelMutedParticipantItem.from_dict(open_channel_muted_participant_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


