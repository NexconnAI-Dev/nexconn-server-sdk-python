# GroupChannelMemberFavoritesUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**user_id** | **str** |  | 
**favorite_ids** | **List[str]** | Followed member user IDs. | 

## Example

```python
from ncsdk.models.group_channel_member_favorites_update_request import GroupChannelMemberFavoritesUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelMemberFavoritesUpdateRequest from a JSON string
group_channel_member_favorites_update_request_instance = GroupChannelMemberFavoritesUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelMemberFavoritesUpdateRequest.to_json())

# convert the object into a dict
group_channel_member_favorites_update_request_dict = group_channel_member_favorites_update_request_instance.to_dict()
# create an instance of GroupChannelMemberFavoritesUpdateRequest from a dict
group_channel_member_favorites_update_request_from_dict = GroupChannelMemberFavoritesUpdateRequest.from_dict(group_channel_member_favorites_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


