# CommunitySubchannelListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subchannels** | [**List[CommunitySubchannelItem]**](CommunitySubchannelItem.md) | Lowercase property name from &#x60;CommunityChannelListResult&#x60; (&#x60;/v4/community-channel/subchannel/list&#x60;). | [optional] 

## Example

```python
from ncsdk.models.community_subchannel_list_response_result import CommunitySubchannelListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of CommunitySubchannelListResponseResult from a JSON string
community_subchannel_list_response_result_instance = CommunitySubchannelListResponseResult.from_json(json)
# print the JSON string representation of the object
print(CommunitySubchannelListResponseResult.to_json())

# convert the object into a dict
community_subchannel_list_response_result_dict = community_subchannel_list_response_result_instance.to_dict()
# create an instance of CommunitySubchannelListResponseResult from a dict
community_subchannel_list_response_result_from_dict = CommunitySubchannelListResponseResult.from_dict(community_subchannel_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


