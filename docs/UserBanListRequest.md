# UserBanListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] [default to 50]

## Example

```python
from ncsdk.models.user_ban_list_request import UserBanListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserBanListRequest from a JSON string
user_ban_list_request_instance = UserBanListRequest.from_json(json)
# print the JSON string representation of the object
print(UserBanListRequest.to_json())

# convert the object into a dict
user_ban_list_request_dict = user_ban_list_request_instance.to_dict()
# create an instance of UserBanListRequest from a dict
user_ban_list_request_from_dict = UserBanListRequest.from_dict(user_ban_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


