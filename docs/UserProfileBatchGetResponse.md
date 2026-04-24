# UserProfileBatchGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**UserProfileBatchGetResponseResult**](UserProfileBatchGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_profile_batch_get_response import UserProfileBatchGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserProfileBatchGetResponse from a JSON string
user_profile_batch_get_response_instance = UserProfileBatchGetResponse.from_json(json)
# print the JSON string representation of the object
print(UserProfileBatchGetResponse.to_json())

# convert the object into a dict
user_profile_batch_get_response_dict = user_profile_batch_get_response_instance.to_dict()
# create an instance of UserProfileBatchGetResponse from a dict
user_profile_batch_get_response_from_dict = UserProfileBatchGetResponse.from_dict(user_profile_batch_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


