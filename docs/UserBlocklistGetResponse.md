# UserBlocklistGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**UserBlocklistGetResponseResult**](UserBlocklistGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_blocklist_get_response import UserBlocklistGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserBlocklistGetResponse from a JSON string
user_blocklist_get_response_instance = UserBlocklistGetResponse.from_json(json)
# print the JSON string representation of the object
print(UserBlocklistGetResponse.to_json())

# convert the object into a dict
user_blocklist_get_response_dict = user_blocklist_get_response_instance.to_dict()
# create an instance of UserBlocklistGetResponse from a dict
user_blocklist_get_response_from_dict = UserBlocklistGetResponse.from_dict(user_blocklist_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


