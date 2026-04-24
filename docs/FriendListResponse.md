# FriendListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**FriendListResponseResult**](FriendListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.friend_list_response import FriendListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FriendListResponse from a JSON string
friend_list_response_instance = FriendListResponse.from_json(json)
# print the JSON string representation of the object
print(FriendListResponse.to_json())

# convert the object into a dict
friend_list_response_dict = friend_list_response_instance.to_dict()
# create an instance of FriendListResponse from a dict
friend_list_response_from_dict = FriendListResponse.from_dict(friend_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


