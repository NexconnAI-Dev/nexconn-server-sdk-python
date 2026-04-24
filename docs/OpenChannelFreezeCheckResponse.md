# OpenChannelFreezeCheckResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**OpenChannelFreezeCheckResponseResult**](OpenChannelFreezeCheckResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_freeze_check_response import OpenChannelFreezeCheckResponse

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelFreezeCheckResponse from a JSON string
open_channel_freeze_check_response_instance = OpenChannelFreezeCheckResponse.from_json(json)
# print the JSON string representation of the object
print(OpenChannelFreezeCheckResponse.to_json())

# convert the object into a dict
open_channel_freeze_check_response_dict = open_channel_freeze_check_response_instance.to_dict()
# create an instance of OpenChannelFreezeCheckResponse from a dict
open_channel_freeze_check_response_from_dict = OpenChannelFreezeCheckResponse.from_dict(open_channel_freeze_check_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


