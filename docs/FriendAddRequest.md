# FriendAddRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**target_id** | **str** |  | 
**action** | **int** | &#x60;1&#x60; means add with verification and &#x60;2&#x60; means add directly. | [optional] 
**extra** | **str** |  | [optional] 

## Example

```python
from ncsdk.models.friend_add_request import FriendAddRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FriendAddRequest from a JSON string
friend_add_request_instance = FriendAddRequest.from_json(json)
# print the JSON string representation of the object
print(FriendAddRequest.to_json())

# convert the object into a dict
friend_add_request_dict = friend_add_request_instance.to_dict()
# create an instance of FriendAddRequest from a dict
friend_add_request_from_dict = FriendAddRequest.from_dict(friend_add_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


