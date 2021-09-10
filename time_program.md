## timeit
``` python
import timeit

def test_func():
  print("hello world")

time = timeit(lambda: test_function(), number=100)
print("the average run time of the function is {} secs".format(time))

```

