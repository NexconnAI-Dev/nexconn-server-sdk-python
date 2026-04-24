# CommunityChannelMutedMemberItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 

## Example

```python
from ncsdk.models.community_channel_muted_member_item import CommunityChannelMutedMemberItem

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelMutedMemberItem from a JSON string
community_channel_muted_member_item_instance = CommunityChannelMutedMemberItem.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelMutedMemberItem.to_json())

# convert the object into a dict
community_channel_muted_member_item_dict = community_channel_muted_member_item_instance.to_dict()
# create an instance of CommunityChannelMutedMemberItem from a dict
community_channel_muted_member_item_from_dict = CommunityChannelMutedMemberItem.from_dict(community_channel_muted_member_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


