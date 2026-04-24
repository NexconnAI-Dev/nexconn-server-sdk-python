# UserBlocklistAddRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**target_user_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.user_blocklist_add_request import UserBlocklistAddRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserBlocklistAddRequest from a JSON string
user_blocklist_add_request_instance = UserBlocklistAddRequest.from_json(json)
# print the JSON string representation of the object
print(UserBlocklistAddRequest.to_json())

# convert the object into a dict
user_blocklist_add_request_dict = user_blocklist_add_request_instance.to_dict()
# create an instance of UserBlocklistAddRequest from a dict
user_blocklist_add_request_from_dict = UserBlocklistAddRequest.from_dict(user_blocklist_add_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


