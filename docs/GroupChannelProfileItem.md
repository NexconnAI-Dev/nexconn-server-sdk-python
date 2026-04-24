# GroupChannelProfileItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** | Group channel ID. | [optional] 
**name** | **str** | Group name. | [optional] 
**group_profile** | **Dict[str, object]** | Group basic profile JSON object, such as introduction, announcement, and portrait URL. | [optional] 
**group_ext_profile** | **Dict[str, object]** | Extended group profile JSON object. Keys are typically custom fields prefixed with &#x60;ext_&#x60;. | [optional] 
**permissions** | **Dict[str, object]** | Group permission settings JSON object, including join, invite, and profile-management permissions. | [optional] 
**owner** | **str** | User ID of the current group owner. | [optional] 
**created_at** | **int** | Timestamp when the group was created. | [optional] 
**member_count** | **int** | Current number of group members. | [optional] 

## Example

```python
from ncsdk.models.group_channel_profile_item import GroupChannelProfileItem

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelProfileItem from a JSON string
group_channel_profile_item_instance = GroupChannelProfileItem.from_json(json)
# print the JSON string representation of the object
print(GroupChannelProfileItem.to_json())

# convert the object into a dict
group_channel_profile_item_dict = group_channel_profile_item_instance.to_dict()
# create an instance of GroupChannelProfileItem from a dict
group_channel_profile_item_from_dict = GroupChannelProfileItem.from_dict(group_channel_profile_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


