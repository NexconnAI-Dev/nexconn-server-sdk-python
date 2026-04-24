# GroupChannelProfileUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** | Legacy &#x60;groupId&#x60;. | 
**group_profile** | **Dict[str, object]** | Group basic profile object defined by the source API. | [optional] 
**permissions** | **Dict[str, object]** | Group permission object defined by the source API. | [optional] 
**group_ext_profile** | **Dict[str, str]** | Group extra profile object. Keys should use the &#x60;ext_&#x60; prefix and support up to 10 entries. | [optional] 

## Example

```python
from ncsdk.models.group_channel_profile_update_request import GroupChannelProfileUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelProfileUpdateRequest from a JSON string
group_channel_profile_update_request_instance = GroupChannelProfileUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelProfileUpdateRequest.to_json())

# convert the object into a dict
group_channel_profile_update_request_dict = group_channel_profile_update_request_instance.to_dict()
# create an instance of GroupChannelProfileUpdateRequest from a dict
group_channel_profile_update_request_from_dict = GroupChannelProfileUpdateRequest.from_dict(group_channel_profile_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


