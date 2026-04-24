# CommunitySubchannelListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**page** | **int** |  | [optional] [default to 1]
**page_size** | **int** |  | [optional] [default to 20]
**order** | **int** | Sort order from &#x60;CommunityChannelPageInput&#x60;. | [optional] 

## Example

```python
from ncsdk.models.community_subchannel_list_request import CommunitySubchannelListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunitySubchannelListRequest from a JSON string
community_subchannel_list_request_instance = CommunitySubchannelListRequest.from_json(json)
# print the JSON string representation of the object
print(CommunitySubchannelListRequest.to_json())

# convert the object into a dict
community_subchannel_list_request_dict = community_subchannel_list_request_instance.to_dict()
# create an instance of CommunitySubchannelListRequest from a dict
community_subchannel_list_request_from_dict = CommunitySubchannelListRequest.from_dict(community_subchannel_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


