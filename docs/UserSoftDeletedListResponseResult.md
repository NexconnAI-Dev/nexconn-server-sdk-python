# UserSoftDeletedListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_ids** | **List[str]** | Soft-deleted user IDs. Legacy response field name is &#x60;users&#x60;. | [optional] 

## Example

```python
from ncsdk.models.user_soft_deleted_list_response_result import UserSoftDeletedListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of UserSoftDeletedListResponseResult from a JSON string
user_soft_deleted_list_response_result_instance = UserSoftDeletedListResponseResult.from_json(json)
# print the JSON string representation of the object
print(UserSoftDeletedListResponseResult.to_json())

# convert the object into a dict
user_soft_deleted_list_response_result_dict = user_soft_deleted_list_response_result_instance.to_dict()
# create an instance of UserSoftDeletedListResponseResult from a dict
user_soft_deleted_list_response_result_from_dict = UserSoftDeletedListResponseResult.from_dict(user_soft_deleted_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


