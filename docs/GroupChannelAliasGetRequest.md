# GroupChannelAliasGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**user_id** | **str** |  | 

## Example

```python
from ncsdk.models.group_channel_alias_get_request import GroupChannelAliasGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelAliasGetRequest from a JSON string
group_channel_alias_get_request_instance = GroupChannelAliasGetRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelAliasGetRequest.to_json())

# convert the object into a dict
group_channel_alias_get_request_dict = group_channel_alias_get_request_instance.to_dict()
# create an instance of GroupChannelAliasGetRequest from a dict
group_channel_alias_get_request_from_dict = GroupChannelAliasGetRequest.from_dict(group_channel_alias_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


