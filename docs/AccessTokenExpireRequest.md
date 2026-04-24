# AccessTokenExpireRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_ids** | **List[str]** |  | 
**expires_at** | **int** | Expiration timestamp in milliseconds. | 

## Example

```python
from ncsdk.models.access_token_expire_request import AccessTokenExpireRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AccessTokenExpireRequest from a JSON string
access_token_expire_request_instance = AccessTokenExpireRequest.from_json(json)
# print the JSON string representation of the object
print(AccessTokenExpireRequest.to_json())

# convert the object into a dict
access_token_expire_request_dict = access_token_expire_request_instance.to_dict()
# create an instance of AccessTokenExpireRequest from a dict
access_token_expire_request_from_dict = AccessTokenExpireRequest.from_dict(access_token_expire_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


