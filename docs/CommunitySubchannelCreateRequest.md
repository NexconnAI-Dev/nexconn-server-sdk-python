# CommunitySubchannelCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**subchannel_id** | **str** | Legacy &#x60;busChannel&#x60;. | 
**channel_visibility** | **int** | Legacy &#x60;type&#x60;. &#x60;0&#x60; for public and &#x60;1&#x60; for private. | [optional] 

## Example

```python
from ncsdk.models.community_subchannel_create_request import CommunitySubchannelCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunitySubchannelCreateRequest from a JSON string
community_subchannel_create_request_instance = CommunitySubchannelCreateRequest.from_json(json)
# print the JSON string representation of the object
print(CommunitySubchannelCreateRequest.to_json())

# convert the object into a dict
community_subchannel_create_request_dict = community_subchannel_create_request_instance.to_dict()
# create an instance of CommunitySubchannelCreateRequest from a dict
community_subchannel_create_request_from_dict = CommunitySubchannelCreateRequest.from_dict(community_subchannel_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


