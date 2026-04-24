# UserTagBatchGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**users** | [**List[UserTagBatchGetItem]**](UserTagBatchGetItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_tag_batch_get_response_result import UserTagBatchGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of UserTagBatchGetResponseResult from a JSON string
user_tag_batch_get_response_result_instance = UserTagBatchGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(UserTagBatchGetResponseResult.to_json())

# convert the object into a dict
user_tag_batch_get_response_result_dict = user_tag_batch_get_response_result_instance.to_dict()
# create an instance of UserTagBatchGetResponseResult from a dict
user_tag_batch_get_response_result_from_dict = UserTagBatchGetResponseResult.from_dict(user_tag_batch_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


