# ProfanityWordListResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**words** | [**List[ProfanityWordListedItem]**](ProfanityWordListedItem.md) |  | [optional] 

## Example

```python
from ncsdk.models.profanity_word_list_response_result import ProfanityWordListResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of ProfanityWordListResponseResult from a JSON string
profanity_word_list_response_result_instance = ProfanityWordListResponseResult.from_json(json)
# print the JSON string representation of the object
print(ProfanityWordListResponseResult.to_json())

# convert the object into a dict
profanity_word_list_response_result_dict = profanity_word_list_response_result_instance.to_dict()
# create an instance of ProfanityWordListResponseResult from a dict
profanity_word_list_response_result_from_dict = ProfanityWordListResponseResult.from_dict(profanity_word_list_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


