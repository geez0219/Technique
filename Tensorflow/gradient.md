## How to compute gradient
All related computation need to happen under tf.GradientTape() to be able to compute the gradient.

``` python 
x = tf.Variable(10, dtype=tf.float32) 
with tf.GradientTape() as tape:
    y = x * x
grad = tape.gradient(y, x)
print(grad)
```

There are some cases that gradient cannot be derived.
1. **The vairable is not under watch** </br>
  By default, all trainable variables (created by tf.Variable or tf.compat.v1.get_variable, where trainable=True is default in both cases) are under watch.
  If the variable is not under watch (ex: tf.constant), users need to manually use <GradineTape>.watch(<variable>) to put them under oberservation. 
  
2. **The data type is not float**  </br>
  \<tape>.gradient() won't work if the variable type is not float </br>
  \# tf.Variable(10)  won't work
