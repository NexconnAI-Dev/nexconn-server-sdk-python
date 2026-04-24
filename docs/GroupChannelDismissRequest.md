# GroupChannelDismissRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 

## Example

```python
from ncsdk.models.group_channel_dismiss_request import GroupChannelDismissRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelDismissRequest from a JSON string
group_channel_dismiss_request_instance = GroupChannelDismissRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelDismissRequest.to_json())

# convert the object into a dict
group_channel_dismiss_request_dict = group_channel_dismiss_request_instance.to_dict()
# create an instance of GroupChannelDismissRequest from a dict
group_channel_dismiss_request_from_dict = GroupChannelDismissRequest.from_dict(group_channel_dismiss_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


