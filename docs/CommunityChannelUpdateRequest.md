# CommunityChannelUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**name** | **str** |  | 

## Example

```python
from ncsdk.models.community_channel_update_request import CommunityChannelUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelUpdateRequest from a JSON string
community_channel_update_request_instance = CommunityChannelUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelUpdateRequest.to_json())

# convert the object into a dict
community_channel_update_request_dict = community_channel_update_request_instance.to_dict()
# create an instance of CommunityChannelUpdateRequest from a dict
community_channel_update_request_from_dict = CommunityChannelUpdateRequest.from_dict(community_channel_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


