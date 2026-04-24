# ChannelPushSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_type** | **str** | Session / channel type as a string (&#x60;1&#x60; to &#x60;10&#x60; as accepted by the server). Matches &#x60;ChannelTypeRequestInput&#x60; in the service. | 
**request_id** | **str** | User ID whose channel notification setting is updated. | 
**channel_id** | **str** | Legacy &#x60;targetId&#x60;. | 
**subchannel_id** | **str** | Legacy &#x60;busChannel&#x60;. Used for community-channel subchannel level settings. | [optional] 
**no_disturb_level** | **int** | Do-not-disturb level (required by service validation; range &#x60;-1&#x60; to &#x60;5&#x60;). | 

## Example

```python
from ncsdk.models.channel_push_set_request import ChannelPushSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelPushSetRequest from a JSON string
channel_push_set_request_instance = ChannelPushSetRequest.from_json(json)
# print the JSON string representation of the object
print(ChannelPushSetRequest.to_json())

# convert the object into a dict
channel_push_set_request_dict = channel_push_set_request_instance.to_dict()
# create an instance of ChannelPushSetRequest from a dict
channel_push_set_request_from_dict = ChannelPushSetRequest.from_dict(channel_push_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


