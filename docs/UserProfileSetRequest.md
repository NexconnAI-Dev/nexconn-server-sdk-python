# UserProfileSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**user_profile** | **Dict[str, object]** | Basic profile payload. Either &#x60;userProfile&#x60; or &#x60;userExtProfile&#x60; must be provided. | [optional] 
**user_ext_profile** | **Dict[str, str]** | Extended profile payload. Keys are case-sensitive, should use the &#x60;ext_&#x60; prefix, and values must be strings. Either &#x60;userProfile&#x60; or &#x60;userExtProfile&#x60; must be provided.  | [optional] 

## Example

```python
from ncsdk.models.user_profile_set_request import UserProfileSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserProfileSetRequest from a JSON string
user_profile_set_request_instance = UserProfileSetRequest.from_json(json)
# print the JSON string representation of the object
print(UserProfileSetRequest.to_json())

# convert the object into a dict
user_profile_set_request_dict = user_profile_set_request_instance.to_dict()
# create an instance of UserProfileSetRequest from a dict
user_profile_set_request_from_dict = UserProfileSetRequest.from_dict(user_profile_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


