# CommunityChannelDismissRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 

## Example

```python
from ncsdk.models.community_channel_dismiss_request import CommunityChannelDismissRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelDismissRequest from a JSON string
community_channel_dismiss_request_instance = CommunityChannelDismissRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelDismissRequest.to_json())

# convert the object into a dict
community_channel_dismiss_request_dict = community_channel_dismiss_request_instance.to_dict()
# create an instance of CommunityChannelDismissRequest from a dict
community_channel_dismiss_request_from_dict = CommunityChannelDismissRequest.from_dict(community_channel_dismiss_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


