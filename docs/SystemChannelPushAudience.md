# SystemChannelPushAudience


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **List[str]** |  | [optional] 
**tag** | **List[str]** |  | [optional] 
**tag_or** | **List[str]** |  | [optional] 
**package_name** | **str** |  | [optional] 
**is_to_all** | **bool** |  | [optional] 

## Example

```python
from ncsdk.models.system_channel_push_audience import SystemChannelPushAudience

# TODO update the JSON string below
json = "{}"
# create an instance of SystemChannelPushAudience from a JSON string
system_channel_push_audience_instance = SystemChannelPushAudience.from_json(json)
# print the JSON string representation of the object
print(SystemChannelPushAudience.to_json())

# convert the object into a dict
system_channel_push_audience_dict = system_channel_push_audience_instance.to_dict()
# create an instance of SystemChannelPushAudience from a dict
system_channel_push_audience_from_dict = SystemChannelPushAudience.from_dict(system_channel_push_audience_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


