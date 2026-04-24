# UserTagBatchGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**UserTagBatchGetResponseResult**](UserTagBatchGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_tag_batch_get_response import UserTagBatchGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserTagBatchGetResponse from a JSON string
user_tag_batch_get_response_instance = UserTagBatchGetResponse.from_json(json)
# print the JSON string representation of the object
print(UserTagBatchGetResponse.to_json())

# convert the object into a dict
user_tag_batch_get_response_dict = user_tag_batch_get_response_instance.to_dict()
# create an instance of UserTagBatchGetResponse from a dict
user_tag_batch_get_response_from_dict = UserTagBatchGetResponse.from_dict(user_tag_batch_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


