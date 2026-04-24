# UserTagBatchSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_ids** | **List[str]** |  | 
**tags** | **List[str]** | Full replacement set of user tags. Sending an empty array clears all tags. | 

## Example

```python
from ncsdk.models.user_tag_batch_set_request import UserTagBatchSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserTagBatchSetRequest from a JSON string
user_tag_batch_set_request_instance = UserTagBatchSetRequest.from_json(json)
# print the JSON string representation of the object
print(UserTagBatchSetRequest.to_json())

# convert the object into a dict
user_tag_batch_set_request_dict = user_tag_batch_set_request_instance.to_dict()
# create an instance of UserTagBatchSetRequest from a dict
user_tag_batch_set_request_from_dict = UserTagBatchSetRequest.from_dict(user_tag_batch_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


