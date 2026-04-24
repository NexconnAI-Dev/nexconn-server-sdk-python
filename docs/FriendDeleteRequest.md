# FriendDeleteRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**target_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.friend_delete_request import FriendDeleteRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FriendDeleteRequest from a JSON string
friend_delete_request_instance = FriendDeleteRequest.from_json(json)
# print the JSON string representation of the object
print(FriendDeleteRequest.to_json())

# convert the object into a dict
friend_delete_request_dict = friend_delete_request_instance.to_dict()
# create an instance of FriendDeleteRequest from a dict
friend_delete_request_from_dict = FriendDeleteRequest.from_dict(friend_delete_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


