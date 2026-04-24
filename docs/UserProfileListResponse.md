# UserProfileListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**UserProfileListResponseResult**](UserProfileListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_profile_list_response import UserProfileListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserProfileListResponse from a JSON string
user_profile_list_response_instance = UserProfileListResponse.from_json(json)
# print the JSON string representation of the object
print(UserProfileListResponse.to_json())

# convert the object into a dict
user_profile_list_response_dict = user_profile_list_response_instance.to_dict()
# create an instance of UserProfileListResponse from a dict
user_profile_list_response_from_dict = UserProfileListResponse.from_dict(user_profile_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


