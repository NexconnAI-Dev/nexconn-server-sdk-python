# ChannelTagTargetItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**channel_type** | **int** |  | 

## Example

```python
from ncsdk.models.channel_tag_target_item import ChannelTagTargetItem

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelTagTargetItem from a JSON string
channel_tag_target_item_instance = ChannelTagTargetItem.from_json(json)
# print the JSON string representation of the object
print(ChannelTagTargetItem.to_json())

# convert the object into a dict
channel_tag_target_item_dict = channel_tag_target_item_instance.to_dict()
# create an instance of ChannelTagTargetItem from a dict
channel_tag_target_item_from_dict = ChannelTagTargetItem.from_dict(channel_tag_target_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


