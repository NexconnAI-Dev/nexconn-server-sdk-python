# GroupChannelAliasSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**user_id** | **str** |  | 
**alias** | **str** |  | 

## Example

```python
from ncsdk.models.group_channel_alias_set_request import GroupChannelAliasSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelAliasSetRequest from a JSON string
group_channel_alias_set_request_instance = GroupChannelAliasSetRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelAliasSetRequest.to_json())

# convert the object into a dict
group_channel_alias_set_request_dict = group_channel_alias_set_request_instance.to_dict()
# create an instance of GroupChannelAliasSetRequest from a dict
group_channel_alias_set_request_from_dict = GroupChannelAliasSetRequest.from_dict(group_channel_alias_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


