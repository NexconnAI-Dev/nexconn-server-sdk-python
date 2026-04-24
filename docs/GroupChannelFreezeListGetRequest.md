# GroupChannelFreezeListGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_ids** | **List[str]** | Optional specific group channel IDs to query. | [optional] 
**page** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_freeze_list_get_request import GroupChannelFreezeListGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelFreezeListGetRequest from a JSON string
group_channel_freeze_list_get_request_instance = GroupChannelFreezeListGetRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelFreezeListGetRequest.to_json())

# convert the object into a dict
group_channel_freeze_list_get_request_dict = group_channel_freeze_list_get_request_instance.to_dict()
# create an instance of GroupChannelFreezeListGetRequest from a dict
group_channel_freeze_list_get_request_from_dict = GroupChannelFreezeListGetRequest.from_dict(group_channel_freeze_list_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


