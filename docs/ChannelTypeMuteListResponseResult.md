# ChannelTypeMuteListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total_count** | **int** |  | [optional] 
**muted_user_ids** | **List[str]** |  | [optional] 

## Example

```python
from ncsdk.models.channel_type_mute_list_response_result import ChannelTypeMuteListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of ChannelTypeMuteListResponseResult from a JSON string
channel_type_mute_list_response_result_instance = ChannelTypeMuteListResponseResult.from_json(json)
# print the JSON string representation of the object
print(ChannelTypeMuteListResponseResult.to_json())

# convert the object into a dict
channel_type_mute_list_response_result_dict = channel_type_mute_list_response_result_instance.to_dict()
# create an instance of ChannelTypeMuteListResponseResult from a dict
channel_type_mute_list_response_result_from_dict = ChannelTypeMuteListResponseResult.from_dict(channel_type_mute_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


