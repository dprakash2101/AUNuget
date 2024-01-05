# Employee


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**employee_id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**age** | **int** |  | [optional] 
**department** | **str** |  | [optional] 
**experience** | **int** |  | [optional] 
**blood_group** | **str** |  | [optional] 
**father_name** | **str** |  | [optional] 
**is_deleted** | **bool** |  | [optional] 
**is_active** | **bool** |  | [optional] 
**date_of_created** | **datetime** |  | [optional] 
**date_of_updated** | **datetime** |  | [optional] 
**roles** | **str** |  | [optional] 
**is_supervisor** | **bool** |  | [optional] 
**is_manager** | **bool** |  | [optional] 

## Example

```python
from EFCrud.models.employee import Employee

# TODO update the JSON string below
json = "{}"
# create an instance of Employee from a JSON string
employee_instance = Employee.from_json(json)
# print the JSON string representation of the object
print Employee.to_json()

# convert the object into a dict
employee_dict = employee_instance.to_dict()
# create an instance of Employee from a dict
employee_form_dict = employee.from_dict(employee_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


