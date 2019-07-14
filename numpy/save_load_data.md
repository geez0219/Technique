
## .npz

save ndarray in .npz files
``` python
a = np.array([1,2,3])
b = np.array([4,5,6])
np.savez("my_file.npz", a=a, b=b)
```

load and use .npz files
``` python
data = np.load("my_file.npz")
a = data["a"] # a = data.f.a
b = data["b"] # b = data.f.b
```
