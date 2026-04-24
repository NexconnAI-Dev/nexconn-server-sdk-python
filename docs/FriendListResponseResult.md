# FriendListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_token** | **str** |  | [optional] 
**total_count** | **int** |  | [optional] 
**friends** | [**List[FriendItem]**](FriendItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.friend_list_response_result import FriendListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of FriendListResponseResult from a JSON string
friend_list_response_result_instance = FriendListResponseResult.from_json(json)
# print the JSON string representation of the object
print(FriendListResponseResult.to_json())

# convert the object into a dict
friend_list_response_result_dict = friend_list_response_result_instance.to_dict()
# create an instance of FriendListResponseResult from a dict
friend_list_response_result_from_dict = FriendListResponseResult.from_dict(friend_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


