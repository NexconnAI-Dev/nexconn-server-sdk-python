# GroupChannelJoinResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**GroupChannelProfileItem**](GroupChannelProfileItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.group_channel_join_response import GroupChannelJoinResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelJoinResponse from a JSON string
group_channel_join_response_instance = GroupChannelJoinResponse.from_json(json)
# print the JSON string representation of the object
print(GroupChannelJoinResponse.to_json())

# convert the object into a dict
group_channel_join_response_dict = group_channel_join_response_instance.to_dict()
# create an instance of GroupChannelJoinResponse from a dict
group_channel_join_response_from_dict = GroupChannelJoinResponse.from_dict(group_channel_join_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


