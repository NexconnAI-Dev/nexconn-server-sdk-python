# OpenChannelFreezeListGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**OpenChannelFreezeListGetResponseResult**](OpenChannelFreezeListGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_freeze_list_get_response import OpenChannelFreezeListGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelFreezeListGetResponse from a JSON string
open_channel_freeze_list_get_response_instance = OpenChannelFreezeListGetResponse.from_json(json)
# print the JSON string representation of the object
print(OpenChannelFreezeListGetResponse.to_json())

# convert the object into a dict
open_channel_freeze_list_get_response_dict = open_channel_freeze_list_get_response_instance.to_dict()
# create an instance of OpenChannelFreezeListGetResponse from a dict
open_channel_freeze_list_get_response_from_dict = OpenChannelFreezeListGetResponse.from_dict(open_channel_freeze_list_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


