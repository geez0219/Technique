## PYTHONPATH
### how to check system path
``` python
import sys
print(sys.path)
```
sys.path is the list of stream that store all system directories (the python import will search this directories)

### how to add system path
``` python
import sys, os
sys.path.append(<the_directory>)
sys.path.append(os.path.dirname(os.path.abspath(__file__))) # add the current file directory 
```


