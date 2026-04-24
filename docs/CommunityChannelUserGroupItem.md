# CommunityChannelUserGroupItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_group_id** | **str** |  | 

## Example

```python
from ncsdk.models.community_channel_user_group_item import CommunityChannelUserGroupItem

# TODO update the JSON string below
json = "{}"
# create an instance of CommunityChannelUserGroupItem from a JSON string
community_channel_user_group_item_instance = CommunityChannelUserGroupItem.from_json(json)
# print the JSON string representation of the object
print(CommunityChannelUserGroupItem.to_json())

# convert the object into a dict
community_channel_user_group_item_dict = community_channel_user_group_item_instance.to_dict()
# create an instance of CommunityChannelUserGroupItem from a dict
community_channel_user_group_item_from_dict = CommunityChannelUserGroupItem.from_dict(community_channel_user_group_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


