# GroupChannelFreezeListGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**GroupChannelFreezeListGetResponseResult**](GroupChannelFreezeListGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_freeze_list_get_response import GroupChannelFreezeListGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelFreezeListGetResponse from a JSON string
group_channel_freeze_list_get_response_instance = GroupChannelFreezeListGetResponse.from_json(json)
# print the JSON string representation of the object
print(GroupChannelFreezeListGetResponse.to_json())

# convert the object into a dict
group_channel_freeze_list_get_response_dict = group_channel_freeze_list_get_response_instance.to_dict()
# create an instance of GroupChannelFreezeListGetResponse from a dict
group_channel_freeze_list_get_response_from_dict = GroupChannelFreezeListGetResponse.from_dict(group_channel_freeze_list_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


