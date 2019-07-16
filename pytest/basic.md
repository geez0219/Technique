## install
pip install pytest

## How to use it
###	prerequisite
1.	test file with name starting with “test_”
2.	test function in the test file that have funtion name starting with “test_”

### running command 
``` pytest [-v] ``` </br>
or </br>
``` python -m pytest [-v] ``` </br>
it will recursively goes through all testing functions (function name start with “test_”) in all testing file (file name start with “test_”) in the current directory and run all testing functions. 

```
pytest [-v]  #(current directory)
pytest <path_of_directory> [-v]  #(specific directory)
pytest <path_of_file> [-v]     #(specific file)
pytest <path_of_file>::<function_name> #(specific file function)
```
Notice: even with specific searching region the file and function name should also be legit 

## How to write test file
1.	all files with test functions starting with name “test_” can be called as testing file.
2.	the files name should also start with name “test_”

e.g.
```
# in file “test_xxxxx1” (the file has file name starting with “test_”, check)

def “test_xxx” (the file has function starting with “test_”, check)
….
def “test_xxx” 
….
```

## How to write test function
Test function here is not the function that need to be tested, it is the function to test the function need to be tested.
1.	Test function should have name starting with “test_”
2.	The function has no argument, so it can be executed directly.
3.	The test function should be written with assert function. Usually in the format like: 
``` 
assert tested_function(testcase_input) == testcase_output 
```
4.	The test function will be considered as pass if system runs it without an error
  
e.g.
```
#  here we want to test the “add” function
def test_add():
	assert add(1,2) == 3
```

## want to print something while testing
need to add a argument -s
``` 
pytest -s
```
