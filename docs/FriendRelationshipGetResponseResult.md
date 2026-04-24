# FriendRelationshipGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**friendships** | [**List[FriendRelationshipItem]**](FriendRelationshipItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.friend_relationship_get_response_result import FriendRelationshipGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of FriendRelationshipGetResponseResult from a JSON string
friend_relationship_get_response_result_instance = FriendRelationshipGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(FriendRelationshipGetResponseResult.to_json())

# convert the object into a dict
friend_relationship_get_response_result_dict = friend_relationship_get_response_result_instance.to_dict()
# create an instance of FriendRelationshipGetResponseResult from a dict
friend_relationship_get_response_result_from_dict = FriendRelationshipGetResponseResult.from_dict(friend_relationship_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


