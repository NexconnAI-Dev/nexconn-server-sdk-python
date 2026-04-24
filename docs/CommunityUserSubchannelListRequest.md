# CommunityUserSubchannelListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**user_id** | **str** |  | 
**page** | **int** |  | [optional] 
**page_size** | **int** |  | [optional] [default to 10]

## Example

```python
from ncsdk.models.community_user_subchannel_list_request import CommunityUserSubchannelListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityUserSubchannelListRequest from a JSON string
community_user_subchannel_list_request_instance = CommunityUserSubchannelListRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityUserSubchannelListRequest.to_json())

# convert the object into a dict
community_user_subchannel_list_request_dict = community_user_subchannel_list_request_instance.to_dict()
# create an instance of CommunityUserSubchannelListRequest from a dict
community_user_subchannel_list_request_from_dict = CommunityUserSubchannelListRequest.from_dict(community_user_subchannel_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


