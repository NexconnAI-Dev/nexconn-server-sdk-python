# OpenChannelGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | [optional] 
**created_at** | **int** |  | [optional] 
**participant_count** | **int** |  | [optional] 
**destroy_type** | **int** |  | [optional] 
**ttl_minutes** | **int** |  | [optional] 
**is_frozen** | **bool** | Whole-channel mute status. | [optional] 

## Example

```python
from ncsdk.models.open_channel_get_response_result import OpenChannelGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelGetResponseResult from a JSON string
open_channel_get_response_result_instance = OpenChannelGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(OpenChannelGetResponseResult.to_json())

# convert the object into a dict
open_channel_get_response_result_dict = open_channel_get_response_result_instance.to_dict()
# create an instance of OpenChannelGetResponseResult from a dict
open_channel_get_response_result_from_dict = OpenChannelGetResponseResult.from_dict(open_channel_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


