# UserProfileListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **int** |  | [optional] [default to 1]
**page_size** | **int** |  | [optional] [default to 20]
**order** | **int** | &#x60;0&#x60; for ascending order and &#x60;1&#x60; for descending order. | [optional] 

## Example

```python
from ncsdk.models.user_profile_list_request import UserProfileListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserProfileListRequest from a JSON string
user_profile_list_request_instance = UserProfileListRequest.from_json(json)
# print the JSON string representation of the object
print(UserProfileListRequest.to_json())

# convert the object into a dict
user_profile_list_request_dict = user_profile_list_request_instance.to_dict()
# create an instance of UserProfileListRequest from a dict
user_profile_list_request_from_dict = UserProfileListRequest.from_dict(user_profile_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


