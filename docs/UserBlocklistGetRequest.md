# UserBlocklistGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**page_token** | **str** |  | [optional] 
**page_size** | **int** |  | [optional] [default to 1000]
**order** | **int** | From &#x60;PageableInput.order&#x60;. | [optional] [default to 0]

## Example

```python
from ncsdk.models.user_blocklist_get_request import UserBlocklistGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UserBlocklistGetRequest from a JSON string
user_blocklist_get_request_instance = UserBlocklistGetRequest.from_json(json)
# print the JSON string representation of the object
print(UserBlocklistGetRequest.to_json())

# convert the object into a dict
user_blocklist_get_request_dict = user_blocklist_get_request_instance.to_dict()
# create an instance of UserBlocklistGetRequest from a dict
user_blocklist_get_request_from_dict = UserBlocklistGetRequest.from_dict(user_blocklist_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


