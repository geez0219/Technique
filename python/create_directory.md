## create directory

``` python
import os
os.mkdir(<dir_path>) # this will not create the parent dir if they don't exist
                     # the <dir_path> cannot have existed dir
```

``` python
import os
os.makedirs(<dir_path>, exist_ok=<bool>) # this will create the parent dir
                                         # the <dir_path> can have existed dir
```
