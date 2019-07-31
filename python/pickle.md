Pickle and save ANY object to file (list, dict, class, function... literaly any object)
## install
don't need to install pickle! it is defaultly in python 

## save 
```
pickle.dump(<object>, <file_object>, [save_protocol])
```
* `object`: the object you want to save
* `file_object`: the file object you want to save to. It is the object return by calling **open(<filename>, "wb")**
* `save_protocol`: the saving protocol, pickle.HIGHEST_PROTOCOL, pickle.DEFAULT_PROTOCOL

## load
```
<object> = pickle.load(<file_object>)
```

* `object`: the variable for your loading project
* `file_object`: the file object you want to load. It is the object return by calling **open(<filename>, "rb")**

