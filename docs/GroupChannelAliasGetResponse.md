# GroupChannelAliasGetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**GroupChannelAliasGetResponseResult**](GroupChannelAliasGetResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_alias_get_response import GroupChannelAliasGetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelAliasGetResponse from a JSON string
group_channel_alias_get_response_instance = GroupChannelAliasGetResponse.from_json(json)
# print the JSON string representation of the object
print(GroupChannelAliasGetResponse.to_json())

# convert the object into a dict
group_channel_alias_get_response_dict = group_channel_alias_get_response_instance.to_dict()
# create an instance of GroupChannelAliasGetResponse from a dict
group_channel_alias_get_response_from_dict = GroupChannelAliasGetResponse.from_dict(group_channel_alias_get_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


