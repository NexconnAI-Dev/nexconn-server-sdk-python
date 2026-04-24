# UserTagBatchGetItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | [optional] 
**tags** | **List[str]** |  | [optional] 

## Example

```python
from ncsdk.models.user_tag_batch_get_item import UserTagBatchGetItem

# TODO update the JSON string below
json = "{}"
# create an instance of UserTagBatchGetItem from a JSON string
user_tag_batch_get_item_instance = UserTagBatchGetItem.from_json(json)
# print the JSON string representation of the object
print(UserTagBatchGetItem.to_json())

# convert the object into a dict
user_tag_batch_get_item_dict = user_tag_batch_get_item_instance.to_dict()
# create an instance of UserTagBatchGetItem from a dict
user_tag_batch_get_item_from_dict = UserTagBatchGetItem.from_dict(user_tag_batch_get_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


