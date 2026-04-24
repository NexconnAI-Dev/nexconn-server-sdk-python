# FriendProfileSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**target_id** | **str** |  | 
**alias** | **str** | Omit this field to clear the existing alias. | [optional] 
**friend_ext_profile** | **Dict[str, str]** | Custom friend extension attributes. Keys should match &#x60;ext_xxxxx&#x60;, may contain letters, digits, and underscores, and support up to 10 entries.  | [optional] 

## Example

```python
from ncsdk.models.friend_profile_set_request import FriendProfileSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of FriendProfileSetRequest from a JSON string
friend_profile_set_request_instance = FriendProfileSetRequest.from_json(json)
# print the JSON string representation of the object
print(FriendProfileSetRequest.to_json())

# convert the object into a dict
friend_profile_set_request_dict = friend_profile_set_request_instance.to_dict()
# create an instance of FriendProfileSetRequest from a dict
friend_profile_set_request_from_dict = FriendProfileSetRequest.from_dict(friend_profile_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


