# OpenChannelMessageTypeListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**OpenChannelMessageTypeListResponseResult**](OpenChannelMessageTypeListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_message_type_list_response import OpenChannelMessageTypeListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelMessageTypeListResponse from a JSON string
open_channel_message_type_list_response_instance = OpenChannelMessageTypeListResponse.from_json(json)
# print the JSON string representation of the object
print(OpenChannelMessageTypeListResponse.to_json())

# convert the object into a dict
open_channel_message_type_list_response_dict = open_channel_message_type_list_response_instance.to_dict()
# create an instance of OpenChannelMessageTypeListResponse from a dict
open_channel_message_type_list_response_from_dict = OpenChannelMessageTypeListResponse.from_dict(open_channel_message_type_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


