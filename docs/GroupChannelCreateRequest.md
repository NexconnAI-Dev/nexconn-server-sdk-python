# GroupChannelCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** | Legacy &#x60;groupId&#x60;. | 
**name** | **str** |  | 
**owner** | **str** | Group owner user ID. | 
**user_ids** | **List[str]** | Invited user IDs. The PDF limits this array to 30 users per request. | [optional] 
**group_profile** | **Dict[str, object]** | Group basic profile object. Common keys include &#x60;introduction&#x60;, &#x60;announcement&#x60;, and &#x60;portraitUrl&#x60;. | [optional] 
**permissions** | **Dict[str, object]** | Group permission object defined by the source API. | [optional] 
**group_ext_profile** | **Dict[str, object]** | Group extra profile object. Keys must start with &#x60;ext_&#x60; according to the PDF. | [optional] 

## Example

```python
from ncsdk.models.group_channel_create_request import GroupChannelCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GroupChannelCreateRequest from a JSON string
group_channel_create_request_instance = GroupChannelCreateRequest.from_json(json)
# print the JSON string representation of the object
print(GroupChannelCreateRequest.to_json())

# convert the object into a dict
group_channel_create_request_dict = group_channel_create_request_instance.to_dict()
# create an instance of GroupChannelCreateRequest from a dict
group_channel_create_request_from_dict = GroupChannelCreateRequest.from_dict(group_channel_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


