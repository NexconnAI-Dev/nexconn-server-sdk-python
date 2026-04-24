# OpenChannelParticipantExistItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**participant_id** | **str** | User ID. | [optional] 
**is_in_open_channel** | **int** | Whether the user is in the open channel. &#x60;1&#x60; &#x3D; yes, &#x60;0&#x60; &#x3D; no. | [optional] 

## Example

```python
from ncsdk.models.open_channel_participant_exist_item import OpenChannelParticipantExistItem

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelParticipantExistItem from a JSON string
open_channel_participant_exist_item_instance = OpenChannelParticipantExistItem.from_json(json)
# print the JSON string representation of the object
print(OpenChannelParticipantExistItem.to_json())

# convert the object into a dict
open_channel_participant_exist_item_dict = open_channel_participant_exist_item_instance.to_dict()
# create an instance of OpenChannelParticipantExistItem from a dict
open_channel_participant_exist_item_from_dict = OpenChannelParticipantExistItem.from_dict(open_channel_participant_exist_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


