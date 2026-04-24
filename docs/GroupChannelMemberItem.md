# GroupChannelMemberItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** | Member user ID. | [optional] 
**role** | **int** | Member role. &#x60;1&#x60; regular member, &#x60;2&#x60; admin, &#x60;3&#x60; owner. | [optional] 
**nickname** | **str** | Member nickname in the group. | [optional] 
**extra** | **str** | Additional member profile information. | [optional] 
**joined_at** | **int** | Timestamp when the member joined the group. | [optional] 

## Example

```python
from ncsdk.models.group_channel_member_item import GroupChannelMemberItem

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelMemberItem from a JSON string
group_channel_member_item_instance = GroupChannelMemberItem.from_json(json)
# print the JSON string representation of the object
print(GroupChannelMemberItem.to_json())

# convert the object into a dict
group_channel_member_item_dict = group_channel_member_item_instance.to_dict()
# create an instance of GroupChannelMemberItem from a dict
group_channel_member_item_from_dict = GroupChannelMemberItem.from_dict(group_channel_member_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


