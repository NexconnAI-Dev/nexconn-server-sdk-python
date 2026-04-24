# FriendRelationshipGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**FriendRelationshipGetResponseResult**](FriendRelationshipGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.friend_relationship_get_response import FriendRelationshipGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FriendRelationshipGetResponse from a JSON string
friend_relationship_get_response_instance = FriendRelationshipGetResponse.from_json(json)
# print the JSON string representation of the object
print(FriendRelationshipGetResponse.to_json())

# convert the object into a dict
friend_relationship_get_response_dict = friend_relationship_get_response_instance.to_dict()
# create an instance of FriendRelationshipGetResponse from a dict
friend_relationship_get_response_from_dict = FriendRelationshipGetResponse.from_dict(friend_relationship_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


