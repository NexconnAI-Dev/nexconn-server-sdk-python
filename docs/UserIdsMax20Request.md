# UserIdsMax20Request


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_ids** | **List[str]** | User ID array, up to 20 items per request. | 

## Example

```python
from ncsdk.models.user_ids_max20_request import UserIdsMax20Request

# TODO update the JSON string below
json = "{}"
# create an instance of UserIdsMax20Request from a JSON string
user_ids_max20_request_instance = UserIdsMax20Request.from_json(json)
# print the JSON string representation of the object
print(UserIdsMax20Request.to_json())

# convert the object into a dict
user_ids_max20_request_dict = user_ids_max20_request_instance.to_dict()
# create an instance of UserIdsMax20Request from a dict
user_ids_max20_request_from_dict = UserIdsMax20Request.from_dict(user_ids_max20_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


