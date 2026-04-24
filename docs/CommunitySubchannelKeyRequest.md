# CommunitySubchannelKeyRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**subchannel_id** | **str** |  | 

## Example

```python
from ncsdk.models.community_subchannel_key_request import CommunitySubchannelKeyRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunitySubchannelKeyRequest from a JSON string
community_subchannel_key_request_instance = CommunitySubchannelKeyRequest.from_json(json)
# print the JSON string representation of the object
print(CommunitySubchannelKeyRequest.to_json())

# convert the object into a dict
community_subchannel_key_request_dict = community_subchannel_key_request_instance.to_dict()
# create an instance of CommunitySubchannelKeyRequest from a dict
community_subchannel_key_request_from_dict = CommunitySubchannelKeyRequest.from_dict(community_subchannel_key_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


