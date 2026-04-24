# GroupChannelFreezeStatusItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | [optional] 
**status** | **int** | Freeze status defined by the source API. | [optional] 

## Example

```python
from ncsdk.models.group_channel_freeze_status_item import GroupChannelFreezeStatusItem

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelFreezeStatusItem from a JSON string
group_channel_freeze_status_item_instance = GroupChannelFreezeStatusItem.from_json(json)
# print the JSON string representation of the object
print(GroupChannelFreezeStatusItem.to_json())

# convert the object into a dict
group_channel_freeze_status_item_dict = group_channel_freeze_status_item_instance.to_dict()
# create an instance of GroupChannelFreezeStatusItem from a dict
group_channel_freeze_status_item_from_dict = GroupChannelFreezeStatusItem.from_dict(group_channel_freeze_status_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


