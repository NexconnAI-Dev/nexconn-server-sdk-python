# OpenChannelAllowedSenderListGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**participant_ids** | **List[str]** |  | [optional] 

## Example

```python
from ncsdk.models.open_channel_allowed_sender_list_get_response_result import OpenChannelAllowedSenderListGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelAllowedSenderListGetResponseResult from a JSON string
open_channel_allowed_sender_list_get_response_result_instance = OpenChannelAllowedSenderListGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(OpenChannelAllowedSenderListGetResponseResult.to_json())

# convert the object into a dict
open_channel_allowed_sender_list_get_response_result_dict = open_channel_allowed_sender_list_get_response_result_instance.to_dict()
# create an instance of OpenChannelAllowedSenderListGetResponseResult from a dict
open_channel_allowed_sender_list_get_response_result_from_dict = OpenChannelAllowedSenderListGetResponseResult.from_dict(open_channel_allowed_sender_list_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


