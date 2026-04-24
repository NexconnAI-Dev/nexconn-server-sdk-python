# FriendPermissionGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**FriendPermissionGetResponseResult**](FriendPermissionGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.friend_permission_get_response import FriendPermissionGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FriendPermissionGetResponse from a JSON string
friend_permission_get_response_instance = FriendPermissionGetResponse.from_json(json)
# print the JSON string representation of the object
print(FriendPermissionGetResponse.to_json())

# convert the object into a dict
friend_permission_get_response_dict = friend_permission_get_response_instance.to_dict()
# create an instance of FriendPermissionGetResponse from a dict
friend_permission_get_response_from_dict = FriendPermissionGetResponse.from_dict(friend_permission_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


