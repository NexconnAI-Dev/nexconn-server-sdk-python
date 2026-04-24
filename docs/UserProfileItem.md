# UserProfileItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**version** | **int** |  | [optional] 
**user_profile** | **Dict[str, object]** |  | [optional] 
**user_ext_profile** | **Dict[str, object]** |  | [optional] 

## Example

```python
from ncsdk.models.user_profile_item import UserProfileItem

# TODO update the JSON string below
json = "{}"
# create an instance of UserProfileItem from a JSON string
user_profile_item_instance = UserProfileItem.from_json(json)
# print the JSON string representation of the object
print(UserProfileItem.to_json())

# convert the object into a dict
user_profile_item_dict = user_profile_item_instance.to_dict()
# create an instance of UserProfileItem from a dict
user_profile_item_from_dict = UserProfileItem.from_dict(user_profile_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


