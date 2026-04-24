# GroupChannelProfileListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**profiles** | [**List[GroupChannelProfileItem]**](GroupChannelProfileItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_profile_list_response_result import GroupChannelProfileListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelProfileListResponseResult from a JSON string
group_channel_profile_list_response_result_instance = GroupChannelProfileListResponseResult.from_json(json)
# print the JSON string representation of the object
print(GroupChannelProfileListResponseResult.to_json())

# convert the object into a dict
group_channel_profile_list_response_result_dict = group_channel_profile_list_response_result_instance.to_dict()
# create an instance of GroupChannelProfileListResponseResult from a dict
group_channel_profile_list_response_result_from_dict = GroupChannelProfileListResponseResult.from_dict(group_channel_profile_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


