# UserConnectionStatusResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** | &#x60;1&#x60; means online and &#x60;0&#x60; means offline. | [optional] 

## Example

```python
from ncsdk.models.user_connection_status_response_result import UserConnectionStatusResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of UserConnectionStatusResponseResult from a JSON string
user_connection_status_response_result_instance = UserConnectionStatusResponseResult.from_json(json)
# print the JSON string representation of the object
print(UserConnectionStatusResponseResult.to_json())

# convert the object into a dict
user_connection_status_response_result_dict = user_connection_status_response_result_instance.to_dict()
# create an instance of UserConnectionStatusResponseResult from a dict
user_connection_status_response_result_from_dict = UserConnectionStatusResponseResult.from_dict(user_connection_status_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


