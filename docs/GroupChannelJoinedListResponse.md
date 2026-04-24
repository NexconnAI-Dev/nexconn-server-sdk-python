# GroupChannelJoinedListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**GroupChannelJoinedListResponseResult**](GroupChannelJoinedListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_joined_list_response import GroupChannelJoinedListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelJoinedListResponse from a JSON string
group_channel_joined_list_response_instance = GroupChannelJoinedListResponse.from_json(json)
# print the JSON string representation of the object
print(GroupChannelJoinedListResponse.to_json())

# convert the object into a dict
group_channel_joined_list_response_dict = group_channel_joined_list_response_instance.to_dict()
# create an instance of GroupChannelJoinedListResponse from a dict
group_channel_joined_list_response_from_dict = GroupChannelJoinedListResponse.from_dict(group_channel_joined_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


