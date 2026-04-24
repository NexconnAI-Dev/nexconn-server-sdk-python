# OpenChannelAllowedSenderListGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**OpenChannelAllowedSenderListGetResponseResult**](OpenChannelAllowedSenderListGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_allowed_sender_list_get_response import OpenChannelAllowedSenderListGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelAllowedSenderListGetResponse from a JSON string
open_channel_allowed_sender_list_get_response_instance = OpenChannelAllowedSenderListGetResponse.from_json(json)
# print the JSON string representation of the object
print(OpenChannelAllowedSenderListGetResponse.to_json())

# convert the object into a dict
open_channel_allowed_sender_list_get_response_dict = open_channel_allowed_sender_list_get_response_instance.to_dict()
# create an instance of OpenChannelAllowedSenderListGetResponse from a dict
open_channel_allowed_sender_list_get_response_from_dict = OpenChannelAllowedSenderListGetResponse.from_dict(open_channel_allowed_sender_list_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


