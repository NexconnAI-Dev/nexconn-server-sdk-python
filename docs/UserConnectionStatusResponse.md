# UserConnectionStatusResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**UserConnectionStatusResponseResult**](UserConnectionStatusResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_connection_status_response import UserConnectionStatusResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserConnectionStatusResponse from a JSON string
user_connection_status_response_instance = UserConnectionStatusResponse.from_json(json)
# print the JSON string representation of the object
print(UserConnectionStatusResponse.to_json())

# convert the object into a dict
user_connection_status_response_dict = user_connection_status_response_instance.to_dict()
# create an instance of UserConnectionStatusResponse from a dict
user_connection_status_response_from_dict = UserConnectionStatusResponse.from_dict(user_connection_status_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


