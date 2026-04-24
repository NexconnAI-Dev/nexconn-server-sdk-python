# ChannelTagListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tag_id** | **str** |  | [optional] 
**channels** | [**List[ChannelTagTargetItem]**](ChannelTagTargetItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.channel_tag_list_response_result import ChannelTagListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelTagListResponseResult from a JSON string
channel_tag_list_response_result_instance = ChannelTagListResponseResult.from_json(json)
# print the JSON string representation of the object
print(ChannelTagListResponseResult.to_json())

# convert the object into a dict
channel_tag_list_response_result_dict = channel_tag_list_response_result_instance.to_dict()
# create an instance of ChannelTagListResponseResult from a dict
channel_tag_list_response_result_from_dict = ChannelTagListResponseResult.from_dict(channel_tag_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


