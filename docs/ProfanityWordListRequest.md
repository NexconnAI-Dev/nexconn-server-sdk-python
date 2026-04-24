# ProfanityWordListRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**filter_type** | **str** | Legacy &#x60;type&#x60;. &#x60;0&#x60; for replacement words, &#x60;1&#x60; for blocked words, and &#x60;2&#x60; for all words. PDF documents this field as a string. | [optional] [default to '1']

## Example

```python
from ncsdk.models.profanity_word_list_request import ProfanityWordListRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ProfanityWordListRequest from a JSON string
profanity_word_list_request_instance = ProfanityWordListRequest.from_json(json)
# print the JSON string representation of the object
print(ProfanityWordListRequest.to_json())

# convert the object into a dict
profanity_word_list_request_dict = profanity_word_list_request_instance.to_dict()
# create an instance of ProfanityWordListRequest from a dict
profanity_word_list_request_from_dict = ProfanityWordListRequest.from_dict(profanity_word_list_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


