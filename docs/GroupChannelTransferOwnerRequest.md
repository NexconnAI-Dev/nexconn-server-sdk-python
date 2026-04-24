# GroupChannelTransferOwnerRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**new_owner** | **str** |  | 
**should_leave** | **int** | &#x60;0&#x60; means keep the previous owner in the group and &#x60;1&#x60; means leave the group. | [optional] 
**should_delete_mute** | **int** | &#x60;0&#x60; means keep the previous owner&#39;s mute state and &#x60;1&#x60; means remove it. | [optional] 
**should_delete_allowed_senders_list** | **int** | &#x60;0&#x60; means keep the previous owner&#39;s allowed-senders-list state and &#x60;1&#x60; means remove it. | [optional] 
**should_delete_favorites** | **int** | &#x60;0&#x60; means keep favorites and &#x60;1&#x60; means remove them. | [optional] 

## Example

```python
from ncsdk.models.group_channel_transfer_owner_request import GroupChannelTransferOwnerRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelTransferOwnerRequest from a JSON string
group_channel_transfer_owner_request_instance = GroupChannelTransferOwnerRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelTransferOwnerRequest.to_json())

# convert the object into a dict
group_channel_transfer_owner_request_dict = group_channel_transfer_owner_request_instance.to_dict()
# create an instance of GroupChannelTransferOwnerRequest from a dict
group_channel_transfer_owner_request_from_dict = GroupChannelTransferOwnerRequest.from_dict(group_channel_transfer_owner_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


