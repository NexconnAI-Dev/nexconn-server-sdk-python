# GroupChannelMemberFavoritesListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**GroupChannelMemberFavoritesListResponseResult**](GroupChannelMemberFavoritesListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_member_favorites_list_response import GroupChannelMemberFavoritesListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelMemberFavoritesListResponse from a JSON string
group_channel_member_favorites_list_response_instance = GroupChannelMemberFavoritesListResponse.from_json(json)
# print the JSON string representation of the object
print(GroupChannelMemberFavoritesListResponse.to_json())

# convert the object into a dict
group_channel_member_favorites_list_response_dict = group_channel_member_favorites_list_response_instance.to_dict()
# create an instance of GroupChannelMemberFavoritesListResponse from a dict
group_channel_member_favorites_list_response_from_dict = GroupChannelMemberFavoritesListResponse.from_dict(group_channel_member_favorites_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


