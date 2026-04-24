# OpenChannelDestroyRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_ids** | **List[str]** | Legacy &#x60;chatroomIds&#x60;. | 

## Example

```python
from ncsdk.models.open_channel_destroy_request import OpenChannelDestroyRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelDestroyRequest from a JSON string
open_channel_destroy_request_instance = OpenChannelDestroyRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelDestroyRequest.to_json())

# convert the object into a dict
open_channel_destroy_request_dict = open_channel_destroy_request_instance.to_dict()
# create an instance of OpenChannelDestroyRequest from a dict
open_channel_destroy_request_from_dict = OpenChannelDestroyRequest.from_dict(open_channel_destroy_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


