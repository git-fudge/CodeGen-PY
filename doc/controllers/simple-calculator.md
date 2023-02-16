# Simple Calculator

```python
simple_calculator_controller = client.simple_calculator
```

## Class Name

`SimpleCalculatorController`


# Get Calculate

Calculates the expression using the specified operation.

```python
def get_calculate(self,
                 options=dict())
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `operation` | [`OperationTypeEnum`](../../doc/models/operation-type-enum.md) | Template, Required | The operator to apply on the variables |
| `x` | `float` | Query, Required | The LHS value |
| `y` | `float` | Query, Required | The RHS value |
| `z` | `string` | Query, Required | asd |

## Response Type

`float`

## Example Usage

```python
collect = {}
operation = OperationTypeEnum.MULTIPLY
collect['operation'] = operation

x = 222.14
collect['x'] = x

y = 165.14
collect['y'] = y

z = 'z4'
collect['z'] = z

result = simple_calculator_controller.get_calculate(collect)
```

