# CommunitySubchannelTypeUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**subchannel_id** | **str** |  | 
**channel_visibility** | **int** | &#39;0&#39; for public and &#39;1&#39; for private. | [optional] 

## Example

```python
from ncsdk.models.community_subchannel_type_update_request import CommunitySubchannelTypeUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunitySubchannelTypeUpdateRequest from a JSON string
community_subchannel_type_update_request_instance = CommunitySubchannelTypeUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(CommunitySubchannelTypeUpdateRequest.to_json())

# convert the object into a dict
community_subchannel_type_update_request_dict = community_subchannel_type_update_request_instance.to_dict()
# create an instance of CommunitySubchannelTypeUpdateRequest from a dict
community_subchannel_type_update_request_from_dict = CommunitySubchannelTypeUpdateRequest.from_dict(community_subchannel_type_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


