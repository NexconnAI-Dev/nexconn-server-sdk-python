# FriendRelationshipGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**target_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.friend_relationship_get_request import FriendRelationshipGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FriendRelationshipGetRequest from a JSON string
friend_relationship_get_request_instance = FriendRelationshipGetRequest.from_json(json)
# print the JSON string representation of the object
print(FriendRelationshipGetRequest.to_json())

# convert the object into a dict
friend_relationship_get_request_dict = friend_relationship_get_request_instance.to_dict()
# create an instance of FriendRelationshipGetRequest from a dict
friend_relationship_get_request_from_dict = FriendRelationshipGetRequest.from_dict(friend_relationship_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


