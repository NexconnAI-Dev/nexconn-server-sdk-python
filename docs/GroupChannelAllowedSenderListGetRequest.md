# GroupChannelAllowedSenderListGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 

## Example

```python
from ncsdk.models.group_channel_allowed_sender_list_get_request import GroupChannelAllowedSenderListGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelAllowedSenderListGetRequest from a JSON string
group_channel_allowed_sender_list_get_request_instance = GroupChannelAllowedSenderListGetRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelAllowedSenderListGetRequest.to_json())

# convert the object into a dict
group_channel_allowed_sender_list_get_request_dict = group_channel_allowed_sender_list_get_request_instance.to_dict()
# create an instance of GroupChannelAllowedSenderListGetRequest from a dict
group_channel_allowed_sender_list_get_request_from_dict = GroupChannelAllowedSenderListGetRequest.from_dict(group_channel_allowed_sender_list_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


