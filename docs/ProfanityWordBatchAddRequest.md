# ProfanityWordBatchAddRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**words** | [**List[ProfanityWordItem]**](ProfanityWordItem.md) |  | 

## Example

```python
from ncsdk.models.profanity_word_batch_add_request import ProfanityWordBatchAddRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ProfanityWordBatchAddRequest from a JSON string
profanity_word_batch_add_request_instance = ProfanityWordBatchAddRequest.from_json(json)
# print the JSON string representation of the object
print(ProfanityWordBatchAddRequest.to_json())

# convert the object into a dict
profanity_word_batch_add_request_dict = profanity_word_batch_add_request_instance.to_dict()
# create an instance of ProfanityWordBatchAddRequest from a dict
profanity_word_batch_add_request_from_dict = ProfanityWordBatchAddRequest.from_dict(profanity_word_batch_add_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


