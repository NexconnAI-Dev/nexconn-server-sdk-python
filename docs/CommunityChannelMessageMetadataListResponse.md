# CommunityChannelMessageMetadataListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**CommunityChannelMessageMetadataListResponseResult**](CommunityChannelMessageMetadataListResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.community_channel_message_metadata_list_response import CommunityChannelMessageMetadataListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelMessageMetadataListResponse from a JSON string
community_channel_message_metadata_list_response_instance = CommunityChannelMessageMetadataListResponse.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelMessageMetadataListResponse.to_json())

# convert the object into a dict
community_channel_message_metadata_list_response_dict = community_channel_message_metadata_list_response_instance.to_dict()
# create an instance of CommunityChannelMessageMetadataListResponse from a dict
community_channel_message_metadata_list_response_from_dict = CommunityChannelMessageMetadataListResponse.from_dict(community_channel_message_metadata_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


