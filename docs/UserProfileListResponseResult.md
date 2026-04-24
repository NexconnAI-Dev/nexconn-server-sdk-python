# UserProfileListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**users** | [**List[UserProfileListItem]**](UserProfileListItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_profile_list_response_result import UserProfileListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of UserProfileListResponseResult from a JSON string
user_profile_list_response_result_instance = UserProfileListResponseResult.from_json(json)
# print the JSON string representation of the object
print(UserProfileListResponseResult.to_json())

# convert the object into a dict
user_profile_list_response_result_dict = user_profile_list_response_result_instance.to_dict()
# create an instance of UserProfileListResponseResult from a dict
user_profile_list_response_result_from_dict = UserProfileListResponseResult.from_dict(user_profile_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


