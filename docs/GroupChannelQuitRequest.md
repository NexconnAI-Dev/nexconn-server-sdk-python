# GroupChannelQuitRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**user_ids** | **List[str]** |  | 
**should_delete_mute** | **int** | &#x60;0&#x60; means keep each leaving member&#39;s mute state and &#x60;1&#x60; means remove it. | [optional] 
**should_delete_allowed_senders_list** | **int** | &#x60;0&#x60; means keep each leaving member&#39;s allowed-senders-list state and &#x60;1&#x60; means remove it. | [optional] 
**should_delete_favorites** | **int** | &#x60;0&#x60; means keep each leaving member&#39;s favorites record and &#x60;1&#x60; means remove it. | [optional] 

## Example

```python
from ncsdk.models.group_channel_quit_request import GroupChannelQuitRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelQuitRequest from a JSON string
group_channel_quit_request_instance = GroupChannelQuitRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelQuitRequest.to_json())

# convert the object into a dict
group_channel_quit_request_dict = group_channel_quit_request_instance.to_dict()
# create an instance of GroupChannelQuitRequest from a dict
group_channel_quit_request_from_dict = GroupChannelQuitRequest.from_dict(group_channel_quit_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


