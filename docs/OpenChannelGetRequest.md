# OpenChannelGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 

## Example

```python
from ncsdk.models.open_channel_get_request import OpenChannelGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelGetRequest from a JSON string
open_channel_get_request_instance = OpenChannelGetRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelGetRequest.to_json())

# convert the object into a dict
open_channel_get_request_dict = open_channel_get_request_instance.to_dict()
# create an instance of OpenChannelGetRequest from a dict
open_channel_get_request_from_dict = OpenChannelGetRequest.from_dict(open_channel_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


