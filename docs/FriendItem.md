# FriendItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**alias** | **str** |  | [optional] 
**friend_ext_profile** | **Dict[str, object]** |  | [optional] 
**added_at** | **int** |  | [optional] 

## Example

```python
from ncsdk.models.friend_item import FriendItem

# TODO update the JSON string below
json = "{}"
# create an instance of FriendItem from a JSON string
friend_item_instance = FriendItem.from_json(json)
# print the JSON string representation of the object
print(FriendItem.to_json())

# convert the object into a dict
friend_item_dict = friend_item_instance.to_dict()
# create an instance of FriendItem from a dict
friend_item_from_dict = FriendItem.from_dict(friend_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


