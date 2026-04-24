# CommunityChannelCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** | Initial member to join after community creation. | 
**channel_id** | **str** | Legacy &#x60;groupId&#x60;. | 
**name** | **str** |  | 

## Example

```python
from ncsdk.models.community_channel_create_request import CommunityChannelCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelCreateRequest from a JSON string
community_channel_create_request_instance = CommunityChannelCreateRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelCreateRequest.to_json())

# convert the object into a dict
community_channel_create_request_dict = community_channel_create_request_instance.to_dict()
# create an instance of CommunityChannelCreateRequest from a dict
community_channel_create_request_from_dict = CommunityChannelCreateRequest.from_dict(community_channel_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


