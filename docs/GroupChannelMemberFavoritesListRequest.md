# GroupChannelMemberFavoritesListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**user_id** | **str** |  | 

## Example

```python
from ncsdk.models.group_channel_member_favorites_list_request import GroupChannelMemberFavoritesListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelMemberFavoritesListRequest from a JSON string
group_channel_member_favorites_list_request_instance = GroupChannelMemberFavoritesListRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelMemberFavoritesListRequest.to_json())

# convert the object into a dict
group_channel_member_favorites_list_request_dict = group_channel_member_favorites_list_request_instance.to_dict()
# create an instance of GroupChannelMemberFavoritesListRequest from a dict
group_channel_member_favorites_list_request_from_dict = GroupChannelMemberFavoritesListRequest.from_dict(group_channel_member_favorites_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


