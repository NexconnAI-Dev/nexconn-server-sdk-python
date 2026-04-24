# GroupChannelListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**GroupChannelListResponseResult**](GroupChannelListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_list_response import GroupChannelListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelListResponse from a JSON string
group_channel_list_response_instance = GroupChannelListResponse.from_json(json)
# print the JSON string representation of the object
print(GroupChannelListResponse.to_json())

# convert the object into a dict
group_channel_list_response_dict = group_channel_list_response_instance.to_dict()
# create an instance of GroupChannelListResponse from a dict
group_channel_list_response_from_dict = GroupChannelListResponse.from_dict(group_channel_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


