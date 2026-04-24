# ChannelTagListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**ChannelTagListResponseResult**](ChannelTagListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.channel_tag_list_response import ChannelTagListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelTagListResponse from a JSON string
channel_tag_list_response_instance = ChannelTagListResponse.from_json(json)
# print the JSON string representation of the object
print(ChannelTagListResponse.to_json())

# convert the object into a dict
channel_tag_list_response_dict = channel_tag_list_response_instance.to_dict()
# create an instance of ChannelTagListResponse from a dict
channel_tag_list_response_from_dict = ChannelTagListResponse.from_dict(channel_tag_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


