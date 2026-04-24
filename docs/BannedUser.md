# BannedUser


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**ban_expires_at** | **str** | Ban expiry time as returned by the server (&#x60;BannedUserItem&#x60; uses string). | [optional] 

## Example

```python
from ncsdk.models.banned_user import BannedUser

# TODO update the JSON string below
json = "{}"
# create an instance of BannedUser from a JSON string
banned_user_instance = BannedUser.from_json(json)
# print the JSON string representation of the object
print(BannedUser.to_json())

# convert the object into a dict
banned_user_dict = banned_user_instance.to_dict()
# create an instance of BannedUser from a dict
banned_user_from_dict = BannedUser.from_dict(banned_user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


