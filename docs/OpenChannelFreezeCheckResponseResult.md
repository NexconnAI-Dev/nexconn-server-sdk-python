# OpenChannelFreezeCheckResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **int** | &#39;1&#39; means frozen and &#39;0&#39; means not frozen. | [optional] 

## Example

```python
from ncsdk.models.open_channel_freeze_check_response_result import OpenChannelFreezeCheckResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelFreezeCheckResponseResult from a JSON string
open_channel_freeze_check_response_result_instance = OpenChannelFreezeCheckResponseResult.from_json(json)
# print the JSON string representation of the object
print(OpenChannelFreezeCheckResponseResult.to_json())

# convert the object into a dict
open_channel_freeze_check_response_result_dict = open_channel_freeze_check_response_result_instance.to_dict()
# create an instance of OpenChannelFreezeCheckResponseResult from a dict
open_channel_freeze_check_response_result_from_dict = OpenChannelFreezeCheckResponseResult.from_dict(open_channel_freeze_check_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


