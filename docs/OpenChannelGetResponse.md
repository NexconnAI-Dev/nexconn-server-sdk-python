# OpenChannelGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**OpenChannelGetResponseResult**](OpenChannelGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_get_response import OpenChannelGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelGetResponse from a JSON string
open_channel_get_response_instance = OpenChannelGetResponse.from_json(json)
# print the JSON string representation of the object
print(OpenChannelGetResponse.to_json())

# convert the object into a dict
open_channel_get_response_dict = open_channel_get_response_instance.to_dict()
# create an instance of OpenChannelGetResponse from a dict
open_channel_get_response_from_dict = OpenChannelGetResponse.from_dict(open_channel_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


