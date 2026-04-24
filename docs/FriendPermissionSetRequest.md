# FriendPermissionSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_ids** | **List[str]** |  | 
**permission_type** | **int** | &#x60;1&#x60; allows everyone, &#x60;2&#x60; requires approval, and &#x60;3&#x60; rejects all requests. | 

## Example

```python
from ncsdk.models.friend_permission_set_request import FriendPermissionSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FriendPermissionSetRequest from a JSON string
friend_permission_set_request_instance = FriendPermissionSetRequest.from_json(json)
# print the JSON string representation of the object
print(FriendPermissionSetRequest.to_json())

# convert the object into a dict
friend_permission_set_request_dict = friend_permission_set_request_instance.to_dict()
# create an instance of FriendPermissionSetRequest from a dict
friend_permission_set_request_from_dict = FriendPermissionSetRequest.from_dict(friend_permission_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


