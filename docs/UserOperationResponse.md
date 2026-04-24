# UserOperationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**UserOperationResponseResult**](UserOperationResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_operation_response import UserOperationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserOperationResponse from a JSON string
user_operation_response_instance = UserOperationResponse.from_json(json)
# print the JSON string representation of the object
print(UserOperationResponse.to_json())

# convert the object into a dict
user_operation_response_dict = user_operation_response_instance.to_dict()
# create an instance of UserOperationResponse from a dict
user_operation_response_from_dict = UserOperationResponse.from_dict(user_operation_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


