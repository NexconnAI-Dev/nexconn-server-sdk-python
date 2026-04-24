# CommunityUserSubchannelListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sub_channels** | **List[str]** |  | [optional] 

## Example

```python
from ncsdk.models.community_user_subchannel_list_response_result import CommunityUserSubchannelListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityUserSubchannelListResponseResult from a JSON string
community_user_subchannel_list_response_result_instance = CommunityUserSubchannelListResponseResult.from_json(json)
# print the JSON string representation of the object
print(CommunityUserSubchannelListResponseResult.to_json())

# convert the object into a dict
community_user_subchannel_list_response_result_dict = community_user_subchannel_list_response_result_instance.to_dict()
# create an instance of CommunityUserSubchannelListResponseResult from a dict
community_user_subchannel_list_response_result_from_dict = CommunityUserSubchannelListResponseResult.from_dict(community_user_subchannel_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


