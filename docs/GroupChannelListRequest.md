# GroupChannelListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_token** | **str** |  | [optional] 
**page_size** | **int** |  | [optional] 
**order** | **int** |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_list_request import GroupChannelListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelListRequest from a JSON string
group_channel_list_request_instance = GroupChannelListRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelListRequest.to_json())

# convert the object into a dict
group_channel_list_request_dict = group_channel_list_request_instance.to_dict()
# create an instance of GroupChannelListRequest from a dict
group_channel_list_request_from_dict = GroupChannelListRequest.from_dict(group_channel_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


