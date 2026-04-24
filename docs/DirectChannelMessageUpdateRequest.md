# DirectChannelMessageUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**from_user_id** | **str** |  | 
**target_id** | **str** | Direct-channel target user ID. | 
**message_id** | **str** |  | 
**content** | **str** |  | 

## Example

```python
from ncsdk.models.direct_channel_message_update_request import DirectChannelMessageUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of DirectChannelMessageUpdateRequest from a JSON string
direct_channel_message_update_request_instance = DirectChannelMessageUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(DirectChannelMessageUpdateRequest.to_json())

# convert the object into a dict
direct_channel_message_update_request_dict = direct_channel_message_update_request_instance.to_dict()
# create an instance of DirectChannelMessageUpdateRequest from a dict
direct_channel_message_update_request_from_dict = DirectChannelMessageUpdateRequest.from_dict(direct_channel_message_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


