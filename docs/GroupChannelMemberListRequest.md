# GroupChannelMemberListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** | Group channel ID. | 
**member_role** | **int** | Member role filter. &#x60;0&#x60; all members, &#x60;1&#x60; regular members, &#x60;2&#x60; admins, &#x60;3&#x60; owner. | [optional] 
**page_token** | **str** | Pagination token returned by the previous request. Omit it for the first page. | [optional] 
**page_size** | **int** | Number of members to return per page. The official default is 50 and the maximum is 100. | [optional] 
**order** | **int** | Sort order by join time. &#x60;0&#x60; ascending and &#x60;1&#x60; descending. | [optional] 

## Example

```python
from ncsdk.models.group_channel_member_list_request import GroupChannelMemberListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelMemberListRequest from a JSON string
group_channel_member_list_request_instance = GroupChannelMemberListRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelMemberListRequest.to_json())

# convert the object into a dict
group_channel_member_list_request_dict = group_channel_member_list_request_instance.to_dict()
# create an instance of GroupChannelMemberListRequest from a dict
group_channel_member_list_request_from_dict = GroupChannelMemberListRequest.from_dict(group_channel_member_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


