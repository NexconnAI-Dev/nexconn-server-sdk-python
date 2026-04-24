# GroupChannelMemberBatchGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**GroupChannelMemberBatchGetResponseResult**](GroupChannelMemberBatchGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_member_batch_get_response import GroupChannelMemberBatchGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelMemberBatchGetResponse from a JSON string
group_channel_member_batch_get_response_instance = GroupChannelMemberBatchGetResponse.from_json(json)
# print the JSON string representation of the object
print(GroupChannelMemberBatchGetResponse.to_json())

# convert the object into a dict
group_channel_member_batch_get_response_dict = group_channel_member_batch_get_response_instance.to_dict()
# create an instance of GroupChannelMemberBatchGetResponse from a dict
group_channel_member_batch_get_response_from_dict = GroupChannelMemberBatchGetResponse.from_dict(group_channel_member_batch_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


