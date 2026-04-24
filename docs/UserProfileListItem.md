# UserProfileListItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**version** | **int** | Profile version from &#x60;UserProfileItemResult&#x60;. | [optional] 
**user_profile** | **Dict[str, object]** |  | [optional] 
**user_ext_profile** | **Dict[str, object]** |  | [optional] 

## Example

```python
from ncsdk.models.user_profile_list_item import UserProfileListItem

# TODO update the JSON string below
json = "{}"
# create an instance of UserProfileListItem from a JSON string
user_profile_list_item_instance = UserProfileListItem.from_json(json)
# print the JSON string representation of the object
print(UserProfileListItem.to_json())

# convert the object into a dict
user_profile_list_item_dict = user_profile_list_item_instance.to_dict()
# create an instance of UserProfileListItem from a dict
user_profile_list_item_from_dict = UserProfileListItem.from_dict(user_profile_list_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


