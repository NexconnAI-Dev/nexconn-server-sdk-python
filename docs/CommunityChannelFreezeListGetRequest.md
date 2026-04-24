# CommunityChannelFreezeListGetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**channel_id** | **str** |  | 
**subchannel_id** | **str** |  | [optional] 
**page** | **int** | Pagination field from &#x60;CommunityAllowedSenderListInput&#x60; / &#x60;AbstractCommunityPagingInput&#x60; (present in Java model; not all server code paths consume it). | [optional] [default to 1]
**page_size** | **int** |  | [optional] [default to 50]

## Example

```python
from ncsdk.models.community_channel_freeze_list_get_request import CommunityChannelFreezeListGetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelFreezeListGetRequest from a JSON string
community_channel_freeze_list_get_request_instance = CommunityChannelFreezeListGetRequest.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelFreezeListGetRequest.to_json())

# convert the object into a dict
community_channel_freeze_list_get_request_dict = community_channel_freeze_list_get_request_instance.to_dict()
# create an instance of CommunityChannelFreezeListGetRequest from a dict
community_channel_freeze_list_get_request_from_dict = CommunityChannelFreezeListGetRequest.from_dict(community_channel_freeze_list_get_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


