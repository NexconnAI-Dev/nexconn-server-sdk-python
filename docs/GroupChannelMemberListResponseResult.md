# GroupChannelMemberListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total_count** | **int** |  | [optional] 
**page_token** | **str** |  | [optional] 
**members** | [**List[GroupChannelMemberItem]**](GroupChannelMemberItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_member_list_response_result import GroupChannelMemberListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelMemberListResponseResult from a JSON string
group_channel_member_list_response_result_instance = GroupChannelMemberListResponseResult.from_json(json)
# print the JSON string representation of the object
print(GroupChannelMemberListResponseResult.to_json())

# convert the object into a dict
group_channel_member_list_response_result_dict = group_channel_member_list_response_result_instance.to_dict()
# create an instance of GroupChannelMemberListResponseResult from a dict
group_channel_member_list_response_result_from_dict = GroupChannelMemberListResponseResult.from_dict(group_channel_member_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


