# OpenChannelPriorityMessageTypeListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message_types** | **List[str]** |  | 

## Example

```python
from ncsdk.models.open_channel_priority_message_type_list_request import OpenChannelPriorityMessageTypeListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelPriorityMessageTypeListRequest from a JSON string
open_channel_priority_message_type_list_request_instance = OpenChannelPriorityMessageTypeListRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelPriorityMessageTypeListRequest.to_json())

# convert the object into a dict
open_channel_priority_message_type_list_request_dict = open_channel_priority_message_type_list_request_instance.to_dict()
# create an instance of OpenChannelPriorityMessageTypeListRequest from a dict
open_channel_priority_message_type_list_request_from_dict = OpenChannelPriorityMessageTypeListRequest.from_dict(open_channel_priority_message_type_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


