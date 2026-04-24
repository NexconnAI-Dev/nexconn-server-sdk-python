# UserOperationResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**operation_id** | **str** | Operation identifier returned by the service. | [optional] 

## Example

```python
from ncsdk.models.user_operation_response_result import UserOperationResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of UserOperationResponseResult from a JSON string
user_operation_response_result_instance = UserOperationResponseResult.from_json(json)
# print the JSON string representation of the object
print(UserOperationResponseResult.to_json())

# convert the object into a dict
user_operation_response_result_dict = user_operation_response_result_instance.to_dict()
# create an instance of UserOperationResponseResult from a dict
user_operation_response_result_from_dict = UserOperationResponseResult.from_dict(user_operation_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


