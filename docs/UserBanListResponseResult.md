# UserBanListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**banned_users** | [**List[BannedUser]**](BannedUser.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_ban_list_response_result import UserBanListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of UserBanListResponseResult from a JSON string
user_ban_list_response_result_instance = UserBanListResponseResult.from_json(json)
# print the JSON string representation of the object
print(UserBanListResponseResult.to_json())

# convert the object into a dict
user_ban_list_response_result_dict = user_ban_list_response_result_instance.to_dict()
# create an instance of UserBanListResponseResult from a dict
user_ban_list_response_result_from_dict = UserBanListResponseResult.from_dict(user_ban_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


