# Userdto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**username** | **str** |  | [optional] 
**password** | **str** |  | [optional] 

## Example

```python
from EFCrud.models.userdto import Userdto

# TODO update the JSON string below
json = "{}"
# create an instance of Userdto from a JSON string
userdto_instance = Userdto.from_json(json)
# print the JSON string representation of the object
print Userdto.to_json()

# convert the object into a dict
userdto_dict = userdto_instance.to_dict()
# create an instance of Userdto from a dict
userdto_form_dict = userdto.from_dict(userdto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


