# UserBlocklistRemoveRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**blocked_user_ids** | **List[str]** |  | 

## Example

```python
from ncsdk.models.user_blocklist_remove_request import UserBlocklistRemoveRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserBlocklistRemoveRequest from a JSON string
user_blocklist_remove_request_instance = UserBlocklistRemoveRequest.from_json(json)
# print the JSON string representation of the object
print(UserBlocklistRemoveRequest.to_json())

# convert the object into a dict
user_blocklist_remove_request_dict = user_blocklist_remove_request_instance.to_dict()
# create an instance of UserBlocklistRemoveRequest from a dict
user_blocklist_remove_request_from_dict = UserBlocklistRemoveRequest.from_dict(user_blocklist_remove_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


