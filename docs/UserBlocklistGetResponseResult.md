# UserBlocklistGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_token** | **str** | Next page cursor; matches &#x60;BlocklistListResult.pageToken&#x60; (not &#x60;next&#x60;). | [optional] 
**blocked_user_ids** | **List[str]** |  | [optional] 

## Example

```python
from ncsdk.models.user_blocklist_get_response_result import UserBlocklistGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of UserBlocklistGetResponseResult from a JSON string
user_blocklist_get_response_result_instance = UserBlocklistGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(UserBlocklistGetResponseResult.to_json())

# convert the object into a dict
user_blocklist_get_response_result_dict = user_blocklist_get_response_result_instance.to_dict()
# create an instance of UserBlocklistGetResponseResult from a dict
user_blocklist_get_response_result_from_dict = UserBlocklistGetResponseResult.from_dict(user_blocklist_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


