# UserTagBatchGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.user_tag_batch_get_request import UserTagBatchGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserTagBatchGetRequest from a JSON string
user_tag_batch_get_request_instance = UserTagBatchGetRequest.from_json(json)
# print the JSON string representation of the object
print(UserTagBatchGetRequest.to_json())

# convert the object into a dict
user_tag_batch_get_request_dict = user_tag_batch_get_request_instance.to_dict()
# create an instance of UserTagBatchGetRequest from a dict
user_tag_batch_get_request_from_dict = UserTagBatchGetRequest.from_dict(user_tag_batch_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


