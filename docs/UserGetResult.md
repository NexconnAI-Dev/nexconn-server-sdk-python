# UserGetResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | User display name. | [optional] 
**avatar_url** | **str** | User avatar URL. | [optional] 
**created_at** | **str** | User creation time as returned by the server (&#x60;GetUserInfoResult&#x60; serializes this as a string, e.g. formatted date-time). | [optional] 

## Example

```python
from ncsdk.models.user_get_result import UserGetResult

# TODO update the JSON string below
json = "{}"
# create an instance of UserGetResult from a JSON string
user_get_result_instance = UserGetResult.from_json(json)
# print the JSON string representation of the object
print(UserGetResult.to_json())

# convert the object into a dict
user_get_result_dict = user_get_result_instance.to_dict()
# create an instance of UserGetResult from a dict
user_get_result_from_dict = UserGetResult.from_dict(user_get_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


