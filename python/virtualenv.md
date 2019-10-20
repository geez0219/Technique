## install
```
pip install virtualenv
```
## Usage
### create virtual environment (using python that virtualenv was install in)
```
virtualenv <env_name> 
```
### create virtual environment (specify python version)
```
virtualenv <env_name> --python=<path_to_python_bin>
```


This command will create an folder in current directory called <env_name>.
The path of this folder in the following article will be called <env_path>

### acitvate environment 
```
source <env_path>/bin/activate
```

### deactivate environment
```
deactivate
```
