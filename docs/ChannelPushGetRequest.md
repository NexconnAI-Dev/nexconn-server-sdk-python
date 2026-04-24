# ChannelPushGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_type** | **str** | Session / channel type as a string (&#x60;1&#x60; to &#x60;10&#x60; as accepted by the server). | 
**request_id** | **str** | User ID whose channel notification setting is queried. | 
**channel_id** | **str** | Legacy &#x60;targetId&#x60;. | 
**subchannel_id** | **str** | Legacy &#x60;busChannel&#x60;. Used for community-channel subchannel level settings. | [optional] 

## Example

```python
from ncsdk.models.channel_push_get_request import ChannelPushGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelPushGetRequest from a JSON string
channel_push_get_request_instance = ChannelPushGetRequest.from_json(json)
# print the JSON string representation of the object
print(ChannelPushGetRequest.to_json())

# convert the object into a dict
channel_push_get_request_dict = channel_push_get_request_instance.to_dict()
# create an instance of ChannelPushGetRequest from a dict
channel_push_get_request_from_dict = ChannelPushGetRequest.from_dict(channel_push_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


