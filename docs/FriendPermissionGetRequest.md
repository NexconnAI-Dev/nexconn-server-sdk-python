# FriendPermissionGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.friend_permission_get_request import FriendPermissionGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FriendPermissionGetRequest from a JSON string
friend_permission_get_request_instance = FriendPermissionGetRequest.from_json(json)
# print the JSON string representation of the object
print(FriendPermissionGetRequest.to_json())

# convert the object into a dict
friend_permission_get_request_dict = friend_permission_get_request_instance.to_dict()
# create an instance of FriendPermissionGetRequest from a dict
friend_permission_get_request_from_dict = FriendPermissionGetRequest.from_dict(friend_permission_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


