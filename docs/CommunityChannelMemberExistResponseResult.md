# CommunityChannelMemberExistResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_member** | **bool** |  | [optional] 

## Example

```python
from ncsdk.models.community_channel_member_exist_response_result import CommunityChannelMemberExistResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelMemberExistResponseResult from a JSON string
community_channel_member_exist_response_result_instance = CommunityChannelMemberExistResponseResult.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelMemberExistResponseResult.to_json())

# convert the object into a dict
community_channel_member_exist_response_result_dict = community_channel_member_exist_response_result_instance.to_dict()
# create an instance of CommunityChannelMemberExistResponseResult from a dict
community_channel_member_exist_response_result_from_dict = CommunityChannelMemberExistResponseResult.from_dict(community_channel_member_exist_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


