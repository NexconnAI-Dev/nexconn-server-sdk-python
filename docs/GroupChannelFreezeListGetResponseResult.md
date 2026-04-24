# GroupChannelFreezeListGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**freeze_statuses** | [**List[GroupChannelFreezeStatusItem]**](GroupChannelFreezeStatusItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_freeze_list_get_response_result import GroupChannelFreezeListGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelFreezeListGetResponseResult from a JSON string
group_channel_freeze_list_get_response_result_instance = GroupChannelFreezeListGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(GroupChannelFreezeListGetResponseResult.to_json())

# convert the object into a dict
group_channel_freeze_list_get_response_result_dict = group_channel_freeze_list_get_response_result_instance.to_dict()
# create an instance of GroupChannelFreezeListGetResponseResult from a dict
group_channel_freeze_list_get_response_result_from_dict = GroupChannelFreezeListGetResponseResult.from_dict(group_channel_freeze_list_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


