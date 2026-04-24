# GroupChannelFavoriteItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**favorited_at** | **int** |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_favorite_item import GroupChannelFavoriteItem

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelFavoriteItem from a JSON string
group_channel_favorite_item_instance = GroupChannelFavoriteItem.from_json(json)
# print the JSON string representation of the object
print(GroupChannelFavoriteItem.to_json())

# convert the object into a dict
group_channel_favorite_item_dict = group_channel_favorite_item_instance.to_dict()
# create an instance of GroupChannelFavoriteItem from a dict
group_channel_favorite_item_from_dict = GroupChannelFavoriteItem.from_dict(group_channel_favorite_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


