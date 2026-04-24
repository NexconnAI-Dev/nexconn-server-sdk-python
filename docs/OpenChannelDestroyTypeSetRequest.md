# OpenChannelDestroyTypeSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**destroy_type** | **int** |  | [optional] 
**ttl_minutes** | **int** |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_destroy_type_set_request import OpenChannelDestroyTypeSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelDestroyTypeSetRequest from a JSON string
open_channel_destroy_type_set_request_instance = OpenChannelDestroyTypeSetRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelDestroyTypeSetRequest.to_json())

# convert the object into a dict
open_channel_destroy_type_set_request_dict = open_channel_destroy_type_set_request_instance.to_dict()
# create an instance of OpenChannelDestroyTypeSetRequest from a dict
open_channel_destroy_type_set_request_from_dict = OpenChannelDestroyTypeSetRequest.from_dict(open_channel_destroy_type_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


