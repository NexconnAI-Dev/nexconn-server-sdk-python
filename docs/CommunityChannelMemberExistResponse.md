# CommunityChannelMemberExistResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**CommunityChannelMemberExistResponseResult**](CommunityChannelMemberExistResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.community_channel_member_exist_response import CommunityChannelMemberExistResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelMemberExistResponse from a JSON string
community_channel_member_exist_response_instance = CommunityChannelMemberExistResponse.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelMemberExistResponse.to_json())

# convert the object into a dict
community_channel_member_exist_response_dict = community_channel_member_exist_response_instance.to_dict()
# create an instance of CommunityChannelMemberExistResponse from a dict
community_channel_member_exist_response_from_dict = CommunityChannelMemberExistResponse.from_dict(community_channel_member_exist_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


