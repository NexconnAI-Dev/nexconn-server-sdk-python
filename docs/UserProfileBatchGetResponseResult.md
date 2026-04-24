# UserProfileBatchGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**users** | [**List[UserProfileItem]**](UserProfileItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_profile_batch_get_response_result import UserProfileBatchGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of UserProfileBatchGetResponseResult from a JSON string
user_profile_batch_get_response_result_instance = UserProfileBatchGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(UserProfileBatchGetResponseResult.to_json())

# convert the object into a dict
user_profile_batch_get_response_result_dict = user_profile_batch_get_response_result_instance.to_dict()
# create an instance of UserProfileBatchGetResponseResult from a dict
user_profile_batch_get_response_result_from_dict = UserProfileBatchGetResponseResult.from_dict(user_profile_batch_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


