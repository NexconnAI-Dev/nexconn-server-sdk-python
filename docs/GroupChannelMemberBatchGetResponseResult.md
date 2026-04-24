# GroupChannelMemberBatchGetResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_token** | **str** | From &#x60;EGMemberListResult.pageToken&#x60;. | [optional] 
**total_count** | **int** | From &#x60;EGMemberListResult.totalCount&#x60;. | [optional] 
**members** | [**List[GroupChannelMemberItem]**](GroupChannelMemberItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_member_batch_get_response_result import GroupChannelMemberBatchGetResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelMemberBatchGetResponseResult from a JSON string
group_channel_member_batch_get_response_result_instance = GroupChannelMemberBatchGetResponseResult.from_json(json)
# print the JSON string representation of the object
print(GroupChannelMemberBatchGetResponseResult.to_json())

# convert the object into a dict
group_channel_member_batch_get_response_result_dict = group_channel_member_batch_get_response_result_instance.to_dict()
# create an instance of GroupChannelMemberBatchGetResponseResult from a dict
group_channel_member_batch_get_response_result_from_dict = GroupChannelMemberBatchGetResponseResult.from_dict(group_channel_member_batch_get_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


