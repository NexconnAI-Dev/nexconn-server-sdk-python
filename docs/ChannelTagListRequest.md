# ChannelTagListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**tag_id** | **str** |  | 

## Example

```python
from ncsdk.models.channel_tag_list_request import ChannelTagListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelTagListRequest from a JSON string
channel_tag_list_request_instance = ChannelTagListRequest.from_json(json)
# print the JSON string representation of the object
print(ChannelTagListRequest.to_json())

# convert the object into a dict
channel_tag_list_request_dict = channel_tag_list_request_instance.to_dict()
# create an instance of ChannelTagListRequest from a dict
channel_tag_list_request_from_dict = ChannelTagListRequest.from_dict(channel_tag_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


