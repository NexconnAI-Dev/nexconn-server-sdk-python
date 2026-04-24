# GroupChannelProfileListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**GroupChannelProfileListResponseResult**](GroupChannelProfileListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_profile_list_response import GroupChannelProfileListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelProfileListResponse from a JSON string
group_channel_profile_list_response_instance = GroupChannelProfileListResponse.from_json(json)
# print the JSON string representation of the object
print(GroupChannelProfileListResponse.to_json())

# convert the object into a dict
group_channel_profile_list_response_dict = group_channel_profile_list_response_instance.to_dict()
# create an instance of GroupChannelProfileListResponse from a dict
group_channel_profile_list_response_from_dict = GroupChannelProfileListResponse.from_dict(group_channel_profile_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


