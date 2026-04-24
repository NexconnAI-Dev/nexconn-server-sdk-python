# UserBanListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**UserBanListResponseResult**](UserBanListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_ban_list_response import UserBanListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UserBanListResponse from a JSON string
user_ban_list_response_instance = UserBanListResponse.from_json(json)
# print the JSON string representation of the object
print(UserBanListResponse.to_json())

# convert the object into a dict
user_ban_list_response_dict = user_ban_list_response_instance.to_dict()
# create an instance of UserBanListResponse from a dict
user_ban_list_response_from_dict = UserBanListResponse.from_dict(user_ban_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


