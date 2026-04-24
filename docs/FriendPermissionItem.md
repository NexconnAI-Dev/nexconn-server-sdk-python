# FriendPermissionItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**permission_type** | **int** |  | [optional] 

## Example

```python
from ncsdk.models.friend_permission_item import FriendPermissionItem

# TODO update the JSON string below
json = "{}"
# create an instance of FriendPermissionItem from a JSON string
friend_permission_item_instance = FriendPermissionItem.from_json(json)
# print the JSON string representation of the object
print(FriendPermissionItem.to_json())

# convert the object into a dict
friend_permission_item_dict = friend_permission_item_instance.to_dict()
# create an instance of FriendPermissionItem from a dict
friend_permission_item_from_dict = FriendPermissionItem.from_dict(friend_permission_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


