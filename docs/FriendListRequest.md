# FriendListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**page_token** | **str** |  | [optional] 
**page_size** | **int** |  | [optional] [default to 50]
**order** | **int** | &#x60;0&#x60; for ascending order and &#x60;1&#x60; for descending order. | [optional] 

## Example

```python
from ncsdk.models.friend_list_request import FriendListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FriendListRequest from a JSON string
friend_list_request_instance = FriendListRequest.from_json(json)
# print the JSON string representation of the object
print(FriendListRequest.to_json())

# convert the object into a dict
friend_list_request_dict = friend_list_request_instance.to_dict()
# create an instance of FriendListRequest from a dict
friend_list_request_from_dict = FriendListRequest.from_dict(friend_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


