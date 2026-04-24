# UserConnectionStatusRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 

## Example

```python
from ncsdk.models.user_connection_status_request import UserConnectionStatusRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserConnectionStatusRequest from a JSON string
user_connection_status_request_instance = UserConnectionStatusRequest.from_json(json)
# print the JSON string representation of the object
print(UserConnectionStatusRequest.to_json())

# convert the object into a dict
user_connection_status_request_dict = user_connection_status_request_instance.to_dict()
# create an instance of UserConnectionStatusRequest from a dict
user_connection_status_request_from_dict = UserConnectionStatusRequest.from_dict(user_connection_status_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


