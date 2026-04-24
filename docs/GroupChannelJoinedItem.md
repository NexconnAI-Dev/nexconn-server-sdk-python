# GroupChannelJoinedItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** | Group channel ID. | [optional] 
**name** | **str** | Group name. | [optional] 
**group_profile** | **Dict[str, object]** | Group basic profile JSON object. | [optional] 
**group_ext_profile** | **Dict[str, object]** | Group extended profile JSON object. | [optional] 
**permissions** | **Dict[str, object]** | Group permission settings JSON object. | [optional] 
**alias** | **str** | Group alias or remark name set by the querying user. | [optional] 
**owner** | **str** | User ID of the current group owner. | [optional] 
**member_count** | **int** | Number of members in the group. | [optional] 
**joined_at** | **int** | Timestamp when the querying user joined the group. | [optional] 
**role** | **int** | The querying user&#39;s role in the group. &#x60;1&#x60; regular member, &#x60;2&#x60; admin, &#x60;3&#x60; owner. | [optional] 
**created_at** | **int** | Timestamp when the group was created. | [optional] 

## Example

```python
from ncsdk.models.group_channel_joined_item import GroupChannelJoinedItem

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelJoinedItem from a JSON string
group_channel_joined_item_instance = GroupChannelJoinedItem.from_json(json)
# print the JSON string representation of the object
print(GroupChannelJoinedItem.to_json())

# convert the object into a dict
group_channel_joined_item_dict = group_channel_joined_item_instance.to_dict()
# create an instance of GroupChannelJoinedItem from a dict
group_channel_joined_item_from_dict = GroupChannelJoinedItem.from_dict(group_channel_joined_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


