# ChannelTagAddRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**tag_id** | **str** |  | 
**channels** | [**List[ChannelTagTargetItem]**](ChannelTagTargetItem.md) |  | 

## Example

```python
from ncsdk.models.channel_tag_add_request import ChannelTagAddRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelTagAddRequest from a JSON string
channel_tag_add_request_instance = ChannelTagAddRequest.from_json(json)
# print the JSON string representation of the object
print(ChannelTagAddRequest.to_json())

# convert the object into a dict
channel_tag_add_request_dict = channel_tag_add_request_instance.to_dict()
# create an instance of ChannelTagAddRequest from a dict
channel_tag_add_request_from_dict = ChannelTagAddRequest.from_dict(channel_tag_add_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


