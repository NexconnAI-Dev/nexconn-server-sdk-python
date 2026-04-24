# UserGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**UserGetResult**](UserGetResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_get_response import UserGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserGetResponse from a JSON string
user_get_response_instance = UserGetResponse.from_json(json)
# print the JSON string representation of the object
print(UserGetResponse.to_json())

# convert the object into a dict
user_get_response_dict = user_get_response_instance.to_dict()
# create an instance of UserGetResponse from a dict
user_get_response_from_dict = UserGetResponse.from_dict(user_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


