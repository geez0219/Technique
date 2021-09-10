## get `Function` graph

```python
@tf.function
def test():
  ....

test.get_concrete_function().graph
```

# get graph node
``` python
graph = <Graph>
print("the graph node number is {}".format(len(graph.as_graph_def().node))
```
