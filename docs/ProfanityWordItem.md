# ProfanityWordItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**word** | **str** | Profanity word content. | 
**replacement** | **str** | Replacement content. When omitted, messages containing the word are blocked instead of replaced. | [optional] 

## Example

```python
from ncsdk.models.profanity_word_item import ProfanityWordItem

# TODO update the JSON string below
json = "{}"
# create an instance of ProfanityWordItem from a JSON string
profanity_word_item_instance = ProfanityWordItem.from_json(json)
# print the JSON string representation of the object
print(ProfanityWordItem.to_json())

# convert the object into a dict
profanity_word_item_dict = profanity_word_item_instance.to_dict()
# create an instance of ProfanityWordItem from a dict
profanity_word_item_from_dict = ProfanityWordItem.from_dict(profanity_word_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


