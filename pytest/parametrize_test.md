## How to parametrize test function

``` python
import pytest

@pytest.mark.parametrize("<variableA>", "<variableB>", ...,
                          [(<variableA_value1>, <variableB_value1>),
                           (<variableA_value2>, <variableB_value2>),
                           ,...])
def some_testing(<variableA>, <variableB>):
  ...

```
