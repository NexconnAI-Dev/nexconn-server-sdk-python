# UserSoftDeletedListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] [default to 50]

## Example

```python
from ncsdk.models.user_soft_deleted_list_request import UserSoftDeletedListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserSoftDeletedListRequest from a JSON string
user_soft_deleted_list_request_instance = UserSoftDeletedListRequest.from_json(json)
# print the JSON string representation of the object
print(UserSoftDeletedListRequest.to_json())

# convert the object into a dict
user_soft_deleted_list_request_dict = user_soft_deleted_list_request_instance.to_dict()
# create an instance of UserSoftDeletedListRequest from a dict
user_soft_deleted_list_request_from_dict = UserSoftDeletedListRequest.from_dict(user_soft_deleted_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


