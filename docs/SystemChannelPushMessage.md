# SystemChannelPushMessage


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **str** |  | 
**message_type** | **str** |  | 
**disable_update_last_msg** | **bool** |  | [optional] 

## Example

```python
from ncsdk.models.system_channel_push_message import SystemChannelPushMessage

# TODO update the JSON string below
json = "{}"
# create an instance of SystemChannelPushMessage from a JSON string
system_channel_push_message_instance = SystemChannelPushMessage.from_json(json)
# print the JSON string representation of the object
print(SystemChannelPushMessage.to_json())

# convert the object into a dict
system_channel_push_message_dict = system_channel_push_message_instance.to_dict()
# create an instance of SystemChannelPushMessage from a dict
system_channel_push_message_from_dict = SystemChannelPushMessage.from_dict(system_channel_push_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


