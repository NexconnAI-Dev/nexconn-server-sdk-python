# FriendRelationshipItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**result** | **int** | Friend relationship result defined by the source API. &#x60;1&#x60; means both users are not friends, &#x60;2&#x60; and &#x60;3&#x60; are reserved, and &#x60;4&#x60; means the friendship is mutual.  | [optional] 

## Example

```python
from ncsdk.models.friend_relationship_item import FriendRelationshipItem

# TODO update the JSON string below
json = "{}"
# create an instance of FriendRelationshipItem from a JSON string
friend_relationship_item_instance = FriendRelationshipItem.from_json(json)
# print the JSON string representation of the object
print(FriendRelationshipItem.to_json())

# convert the object into a dict
friend_relationship_item_dict = friend_relationship_item_instance.to_dict()
# create an instance of FriendRelationshipItem from a dict
friend_relationship_item_from_dict = FriendRelationshipItem.from_dict(friend_relationship_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


