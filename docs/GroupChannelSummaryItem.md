# GroupChannelSummaryItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**group_profile** | **Dict[str, object]** | Group basic profile object as in &#x60;EGGroupListResult.GroupItem.groupProfile&#x60;. | [optional] 
**creator** | **str** | Group creator user ID. | [optional] 
**owner** | **str** |  | [optional] 
**created_at** | **int** |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_summary_item import GroupChannelSummaryItem

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelSummaryItem from a JSON string
group_channel_summary_item_instance = GroupChannelSummaryItem.from_json(json)
# print the JSON string representation of the object
print(GroupChannelSummaryItem.to_json())

# convert the object into a dict
group_channel_summary_item_dict = group_channel_summary_item_instance.to_dict()
# create an instance of GroupChannelSummaryItem from a dict
group_channel_summary_item_from_dict = GroupChannelSummaryItem.from_dict(group_channel_summary_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


