# GroupChannelMemberFavoritesListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**channel_id** | **str** |  | [optional] 
**favorites** | [**List[GroupChannelFavoriteItem]**](GroupChannelFavoriteItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_member_favorites_list_response_result import GroupChannelMemberFavoritesListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelMemberFavoritesListResponseResult from a JSON string
group_channel_member_favorites_list_response_result_instance = GroupChannelMemberFavoritesListResponseResult.from_json(json)
# print the JSON string representation of the object
print(GroupChannelMemberFavoritesListResponseResult.to_json())

# convert the object into a dict
group_channel_member_favorites_list_response_result_dict = group_channel_member_favorites_list_response_result_instance.to_dict()
# create an instance of GroupChannelMemberFavoritesListResponseResult from a dict
group_channel_member_favorites_list_response_result_from_dict = GroupChannelMemberFavoritesListResponseResult.from_dict(group_channel_member_favorites_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


