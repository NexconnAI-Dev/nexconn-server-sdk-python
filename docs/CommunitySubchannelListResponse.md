# CommunitySubchannelListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**CommunitySubchannelListResponseResult**](CommunitySubchannelListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.community_subchannel_list_response import CommunitySubchannelListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CommunitySubchannelListResponse from a JSON string
community_subchannel_list_response_instance = CommunitySubchannelListResponse.from_json(json)
# print the JSON string representation of the object
print(CommunitySubchannelListResponse.to_json())

# convert the object into a dict
community_subchannel_list_response_dict = community_subchannel_list_response_instance.to_dict()
# create an instance of CommunitySubchannelListResponse from a dict
community_subchannel_list_response_from_dict = CommunitySubchannelListResponse.from_dict(community_subchannel_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


