# UserIdsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_ids** | **List[str]** | User ID array. | 

## Example

```python
from ncsdk.models.user_ids_request import UserIdsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserIdsRequest from a JSON string
user_ids_request_instance = UserIdsRequest.from_json(json)
# print the JSON string representation of the object
print(UserIdsRequest.to_json())

# convert the object into a dict
user_ids_request_dict = user_ids_request_instance.to_dict()
# create an instance of UserIdsRequest from a dict
user_ids_request_from_dict = UserIdsRequest.from_dict(user_ids_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


