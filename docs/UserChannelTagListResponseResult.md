# UserChannelTagListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**tags** | [**List[UserChannelTagListItem]**](UserChannelTagListItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.user_channel_tag_list_response_result import UserChannelTagListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of UserChannelTagListResponseResult from a JSON string
user_channel_tag_list_response_result_instance = UserChannelTagListResponseResult.from_json(json)
# print the JSON string representation of the object
print(UserChannelTagListResponseResult.to_json())

# convert the object into a dict
user_channel_tag_list_response_result_dict = user_channel_tag_list_response_result_instance.to_dict()
# create an instance of UserChannelTagListResponseResult from a dict
user_channel_tag_list_response_result_from_dict = UserChannelTagListResponseResult.from_dict(user_channel_tag_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


