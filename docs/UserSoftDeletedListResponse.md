# UserSoftDeletedListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**UserSoftDeletedListResponseResult**](UserSoftDeletedListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_soft_deleted_list_response import UserSoftDeletedListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserSoftDeletedListResponse from a JSON string
user_soft_deleted_list_response_instance = UserSoftDeletedListResponse.from_json(json)
# print the JSON string representation of the object
print(UserSoftDeletedListResponse.to_json())

# convert the object into a dict
user_soft_deleted_list_response_dict = user_soft_deleted_list_response_instance.to_dict()
# create an instance of UserSoftDeletedListResponse from a dict
user_soft_deleted_list_response_from_dict = UserSoftDeletedListResponse.from_dict(user_soft_deleted_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


