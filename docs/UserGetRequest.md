# UserGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 

## Example

```python
from ncsdk.models.user_get_request import UserGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserGetRequest from a JSON string
user_get_request_instance = UserGetRequest.from_json(json)
# print the JSON string representation of the object
print(UserGetRequest.to_json())

# convert the object into a dict
user_get_request_dict = user_get_request_instance.to_dict()
# create an instance of UserGetRequest from a dict
user_get_request_from_dict = UserGetRequest.from_dict(user_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


