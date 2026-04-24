# GroupChannelJoinedListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_token** | **str** |  | [optional] 
**groups** | [**List[GroupChannelJoinedItem]**](GroupChannelJoinedItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_joined_list_response_result import GroupChannelJoinedListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelJoinedListResponseResult from a JSON string
group_channel_joined_list_response_result_instance = GroupChannelJoinedListResponseResult.from_json(json)
# print the JSON string representation of the object
print(GroupChannelJoinedListResponseResult.to_json())

# convert the object into a dict
group_channel_joined_list_response_result_dict = group_channel_joined_list_response_result_instance.to_dict()
# create an instance of GroupChannelJoinedListResponseResult from a dict
group_channel_joined_list_response_result_from_dict = GroupChannelJoinedListResponseResult.from_dict(group_channel_joined_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


