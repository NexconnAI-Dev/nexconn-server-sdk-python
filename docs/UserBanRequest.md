# UserBanRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_ids** | **List[str]** |  | 
**duration_minutes** | **int** |  | 

## Example

```python
from ncsdk.models.user_ban_request import UserBanRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserBanRequest from a JSON string
user_ban_request_instance = UserBanRequest.from_json(json)
# print the JSON string representation of the object
print(UserBanRequest.to_json())

# convert the object into a dict
user_ban_request_dict = user_ban_request_instance.to_dict()
# create an instance of UserBanRequest from a dict
user_ban_request_from_dict = UserBanRequest.from_dict(user_ban_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


