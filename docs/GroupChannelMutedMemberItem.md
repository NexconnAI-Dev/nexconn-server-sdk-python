# GroupChannelMutedMemberItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**muted_at** | **str** | Mute start time in &#x60;YYYY-MM-DD HH:MM:SS&#x60; format. | [optional] 
**mute_expires_at** | **str** | Mute expiry time in &#x60;YYYY-MM-DD HH:MM:SS&#x60; format. | [optional] 

## Example

```python
from ncsdk.models.group_channel_muted_member_item import GroupChannelMutedMemberItem

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelMutedMemberItem from a JSON string
group_channel_muted_member_item_instance = GroupChannelMutedMemberItem.from_json(json)
# print the JSON string representation of the object
print(GroupChannelMutedMemberItem.to_json())

# convert the object into a dict
group_channel_muted_member_item_dict = group_channel_muted_member_item_instance.to_dict()
# create an instance of GroupChannelMutedMemberItem from a dict
group_channel_muted_member_item_from_dict = GroupChannelMutedMemberItem.from_dict(group_channel_muted_member_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


