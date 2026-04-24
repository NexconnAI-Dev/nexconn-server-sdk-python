# UserIdsMax100Request


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_ids** | **List[str]** | User ID array, up to 100 items per request. | 

## Example

```python
from ncsdk.models.user_ids_max100_request import UserIdsMax100Request

# TODO update the JSON string below
json = "{}"
# create an instance of UserIdsMax100Request from a JSON string
user_ids_max100_request_instance = UserIdsMax100Request.from_json(json)
# print the JSON string representation of the object
print(UserIdsMax100Request.to_json())

# convert the object into a dict
user_ids_max100_request_dict = user_ids_max100_request_instance.to_dict()
# create an instance of UserIdsMax100Request from a dict
user_ids_max100_request_from_dict = UserIdsMax100Request.from_dict(user_ids_max100_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


