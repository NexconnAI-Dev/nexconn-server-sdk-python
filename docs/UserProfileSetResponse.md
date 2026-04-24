# UserProfileSetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**profile_key** | **str** | Returns the failed profile key when the update fails. | [optional] 

## Example

```python
from ncsdk.models.user_profile_set_response import UserProfileSetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserProfileSetResponse from a JSON string
user_profile_set_response_instance = UserProfileSetResponse.from_json(json)
# print the JSON string representation of the object
print(UserProfileSetResponse.to_json())

# convert the object into a dict
user_profile_set_response_dict = user_profile_set_response_instance.to_dict()
# create an instance of UserProfileSetResponse from a dict
user_profile_set_response_from_dict = UserProfileSetResponse.from_dict(user_profile_set_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


