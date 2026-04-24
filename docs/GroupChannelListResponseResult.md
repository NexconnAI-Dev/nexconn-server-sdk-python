# GroupChannelListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_token** | **str** |  | [optional] 
**groups** | [**List[GroupChannelSummaryItem]**](GroupChannelSummaryItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_list_response_result import GroupChannelListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelListResponseResult from a JSON string
group_channel_list_response_result_instance = GroupChannelListResponseResult.from_json(json)
# print the JSON string representation of the object
print(GroupChannelListResponseResult.to_json())

# convert the object into a dict
group_channel_list_response_result_dict = group_channel_list_response_result_instance.to_dict()
# create an instance of GroupChannelListResponseResult from a dict
group_channel_list_response_result_from_dict = GroupChannelListResponseResult.from_dict(group_channel_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


