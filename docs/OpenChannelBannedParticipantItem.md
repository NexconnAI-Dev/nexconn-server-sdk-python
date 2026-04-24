# OpenChannelBannedParticipantItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**participant_id** | **str** |  | [optional] 
**ban_expires_at** | **str** | Ban expiration time in &#x60;YYYY-MM-DD HH:MM:SS&#x60; format. | [optional] 

## Example

```python
from ncsdk.models.open_channel_banned_participant_item import OpenChannelBannedParticipantItem

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelBannedParticipantItem from a JSON string
open_channel_banned_participant_item_instance = OpenChannelBannedParticipantItem.from_json(json)
# print the JSON string representation of the object
print(OpenChannelBannedParticipantItem.to_json())

# convert the object into a dict
open_channel_banned_participant_item_dict = open_channel_banned_participant_item_instance.to_dict()
# create an instance of OpenChannelBannedParticipantItem from a dict
open_channel_banned_participant_item_from_dict = OpenChannelBannedParticipantItem.from_dict(open_channel_banned_participant_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


