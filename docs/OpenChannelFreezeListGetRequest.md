# OpenChannelFreezeListGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **int** |  | [optional] [default to 1]
**page_size** | **int** |  | [optional] [default to 50]

## Example

```python
from ncsdk.models.open_channel_freeze_list_get_request import OpenChannelFreezeListGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelFreezeListGetRequest from a JSON string
open_channel_freeze_list_get_request_instance = OpenChannelFreezeListGetRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelFreezeListGetRequest.to_json())

# convert the object into a dict
open_channel_freeze_list_get_request_dict = open_channel_freeze_list_get_request_instance.to_dict()
# create an instance of OpenChannelFreezeListGetRequest from a dict
open_channel_freeze_list_get_request_from_dict = OpenChannelFreezeListGetRequest.from_dict(open_channel_freeze_list_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


