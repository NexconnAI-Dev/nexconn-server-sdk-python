# GroupChannelProfileListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_ids** | **List[str]** | Legacy &#x60;groupIds&#x60;. | 

## Example

```python
from ncsdk.models.group_channel_profile_list_request import GroupChannelProfileListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelProfileListRequest from a JSON string
group_channel_profile_list_request_instance = GroupChannelProfileListRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelProfileListRequest.to_json())

# convert the object into a dict
group_channel_profile_list_request_dict = group_channel_profile_list_request_instance.to_dict()
# create an instance of GroupChannelProfileListRequest from a dict
group_channel_profile_list_request_from_dict = GroupChannelProfileListRequest.from_dict(group_channel_profile_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


