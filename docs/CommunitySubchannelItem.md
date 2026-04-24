# CommunitySubchannelItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**subchannel_id** | **str** |  | [optional] 
**created_at** | **str** | Channel creation time returned by the source API. | [optional] 
**channel_visibility** | **int** |  | [optional] 

## Example

```python
from ncsdk.models.community_subchannel_item import CommunitySubchannelItem

# TODO update the JSON string below
json = "{}"
# create an instance of CommunitySubchannelItem from a JSON string
community_subchannel_item_instance = CommunitySubchannelItem.from_json(json)
# print the JSON string representation of the object
print(CommunitySubchannelItem.to_json())

# convert the object into a dict
community_subchannel_item_dict = community_subchannel_item_instance.to_dict()
# create an instance of CommunitySubchannelItem from a dict
community_subchannel_item_from_dict = CommunitySubchannelItem.from_dict(community_subchannel_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


