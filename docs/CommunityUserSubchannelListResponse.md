# CommunityUserSubchannelListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**CommunityUserSubchannelListResponseResult**](CommunityUserSubchannelListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.community_user_subchannel_list_response import CommunityUserSubchannelListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityUserSubchannelListResponse from a JSON string
community_user_subchannel_list_response_instance = CommunityUserSubchannelListResponse.from_json(json)
# print the JSON string representation of the object
print(CommunityUserSubchannelListResponse.to_json())

# convert the object into a dict
community_user_subchannel_list_response_dict = community_user_subchannel_list_response_instance.to_dict()
# create an instance of CommunityUserSubchannelListResponse from a dict
community_user_subchannel_list_response_from_dict = CommunityUserSubchannelListResponse.from_dict(community_user_subchannel_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


