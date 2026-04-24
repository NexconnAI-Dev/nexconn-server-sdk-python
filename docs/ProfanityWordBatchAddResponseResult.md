# ProfanityWordBatchAddResponseResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**remaining_quota** | **int** | Remaining quota for configured profanity words. | [optional] 

## Example

```python
from ncsdk.models.profanity_word_batch_add_response_result import ProfanityWordBatchAddResponseResult

# TODO update the JSON string below
json = "{}"
# create an instance of ProfanityWordBatchAddResponseResult from a JSON string
profanity_word_batch_add_response_result_instance = ProfanityWordBatchAddResponseResult.from_json(json)
# print the JSON string representation of the object
print(ProfanityWordBatchAddResponseResult.to_json())

# convert the object into a dict
profanity_word_batch_add_response_result_dict = profanity_word_batch_add_response_result_instance.to_dict()
# create an instance of ProfanityWordBatchAddResponseResult from a dict
profanity_word_batch_add_response_result_from_dict = ProfanityWordBatchAddResponseResult.from_dict(profanity_word_batch_add_response_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


