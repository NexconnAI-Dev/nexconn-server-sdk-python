# AccessTokenIssueRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **str** |  | 
**name** | **str** |  | 
**avatar_url** | **str** |  | [optional] 

## Example

```python
from ncsdk.models.access_token_issue_request import AccessTokenIssueRequest

# TODO update the JSON string below
json = "{}"
# create an instance of AccessTokenIssueRequest from a JSON string
access_token_issue_request_instance = AccessTokenIssueRequest.from_json(json)
# print the JSON string representation of the object
print(AccessTokenIssueRequest.to_json())

# convert the object into a dict
access_token_issue_request_dict = access_token_issue_request_instance.to_dict()
# create an instance of AccessTokenIssueRequest from a dict
access_token_issue_request_from_dict = AccessTokenIssueRequest.from_dict(access_token_issue_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


