# ProfanityWordListedItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**word** | **str** | Profanity word content. | [optional] 
**replacement** | **str** | Replacement content. Empty means the word is blocked. | [optional] 
**filter_type** | **str** | Result type. &#x60;0&#x60; means replacement word and &#x60;1&#x60; means blocked word. | [optional] 

## Example

```python
from ncsdk.models.profanity_word_listed_item import ProfanityWordListedItem

# TODO update the JSON string below
json = "{}"
# create an instance of ProfanityWordListedItem from a JSON string
profanity_word_listed_item_instance = ProfanityWordListedItem.from_json(json)
# print the JSON string representation of the object
print(ProfanityWordListedItem.to_json())

# convert the object into a dict
profanity_word_listed_item_dict = profanity_word_listed_item_instance.to_dict()
# create an instance of ProfanityWordListedItem from a dict
profanity_word_listed_item_from_dict = ProfanityWordListedItem.from_dict(profanity_word_listed_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


