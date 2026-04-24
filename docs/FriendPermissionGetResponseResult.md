# FriendPermissionGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**permissions** | [**List[FriendPermissionItem]**](FriendPermissionItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.friend_permission_get_response_result import FriendPermissionGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of FriendPermissionGetResponseResult from a JSON string
friend_permission_get_response_result_instance = FriendPermissionGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(FriendPermissionGetResponseResult.to_json())

# convert the object into a dict
friend_permission_get_response_result_dict = friend_permission_get_response_result_instance.to_dict()
# create an instance of FriendPermissionGetResponseResult from a dict
friend_permission_get_response_result_from_dict = FriendPermissionGetResponseResult.from_dict(friend_permission_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


