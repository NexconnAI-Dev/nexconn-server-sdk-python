# OpenChannelCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** | Legacy &#x60;chatroomId&#x60;. | 
**destroy_type** | **int** | &#39;0&#39; for inactive-time destroy and &#39;1&#39; for fixed-time destroy. | [optional] 
**ttl_minutes** | **int** | Legacy &#x60;destroyTime&#x60;. Valid range is 60 to 10080 minutes according to the PDF. | [optional] 
**should_freeze** | **bool** | Whether whole-channel freeze is enabled when the chatroom is created. | [optional] 
**allowed_senders_list** | **List[str]** | Allowed senders list applied when the chatroom is frozen. | [optional] 
**metadata_owner_id** | **str** | Legacy &#x60;entryOwnerId&#x60;. | [optional] 
**metadata** | **Dict[str, str]** | Legacy &#x60;entryInfo&#x60;. Open-channel metadata key/value pairs. | [optional] 

## Example

```python
from ncsdk.models.open_channel_create_request import OpenChannelCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OpenChannelCreateRequest from a JSON string
open_channel_create_request_instance = OpenChannelCreateRequest.from_json(json)
# print the JSON string representation of the object
print(OpenChannelCreateRequest.to_json())

# convert the object into a dict
open_channel_create_request_dict = open_channel_create_request_instance.to_dict()
# create an instance of OpenChannelCreateRequest from a dict
open_channel_create_request_from_dict = OpenChannelCreateRequest.from_dict(open_channel_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


