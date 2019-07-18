## how to set global variable

### using fixture as variable

``` python 
import pytest
@pytest.fixture()
def variableA():
  return 10

def test_something(variableA):
  print(variableA)
```
In this way, variableA is like the project constant. 
