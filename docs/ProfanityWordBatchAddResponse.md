# ProfanityWordBatchAddResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **int** |  | 
**result** | [**ProfanityWordBatchAddResponseResult**](ProfanityWordBatchAddResponseResult.md) |  | [optional] 

## Example

```python
from ncsdk.models.profanity_word_batch_add_response import ProfanityWordBatchAddResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ProfanityWordBatchAddResponse from a JSON string
profanity_word_batch_add_response_instance = ProfanityWordBatchAddResponse.from_json(json)
# print the JSON string representation of the object
print(ProfanityWordBatchAddResponse.to_json())

# convert the object into a dict
profanity_word_batch_add_response_dict = profanity_word_batch_add_response_instance.to_dict()
# create an instance of ProfanityWordBatchAddResponse from a dict
profanity_word_batch_add_response_from_dict = ProfanityWordBatchAddResponse.from_dict(profanity_word_batch_add_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


