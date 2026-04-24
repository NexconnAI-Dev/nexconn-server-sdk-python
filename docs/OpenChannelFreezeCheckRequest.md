# OpenChannelFreezeCheckRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 

## Example

```python
from ncsdk.models.open_channel_freeze_check_request import OpenChannelFreezeCheckRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelFreezeCheckRequest from a JSON string
open_channel_freeze_check_request_instance = OpenChannelFreezeCheckRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelFreezeCheckRequest.to_json())

# convert the object into a dict
open_channel_freeze_check_request_dict = open_channel_freeze_check_request_instance.to_dict()
# create an instance of OpenChannelFreezeCheckRequest from a dict
open_channel_freeze_check_request_from_dict = OpenChannelFreezeCheckRequest.from_dict(open_channel_freeze_check_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


