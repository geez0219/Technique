## create tensorboard log file

To have tensorboard logging file, users need to:
1. instantiate file writer (associate with folder path) 
2. invoke tf.summary method within <file_writer>.as_default() context manager 

Example: 
``` python 
# instantiate summary writer
summary_writer = tf.summary.create_file_writer('summaries') # 

# wrap summary writting code with summary writer content manager
with summary_writer.as_default():
    tf.summary.scalar('loss', 0.1, step=42) 
    tf.summary.scalar('loss', 0.2, step=43)
    tf.summary.scalar('loss', 0.3, step=44)
    tf.summary.scalar('loss', 0.7, step=45)
```

Note: the tf.summary.scalar needs to be invoked in the order of step, otherwise the time sequence graph will be messed up.

Example: 
``` python 
tf.summary.scalar('loss', 0.1, step=42) 
tf.summary.scalar('loss', 0.2, step=43)
tf.summary.scalar('loss', 0.3, step=44)
tf.summary.scalar('loss', 0.7, step=45)
```
is different from...
``` python 
tf.summary.scalar('loss', 0.7, step=45)
tf.summary.scalar('loss', 0.1, step=42) 
tf.summary.scalar('loss', 0.2, step=43)
tf.summary.scalar('loss', 0.3, step=44)
```
