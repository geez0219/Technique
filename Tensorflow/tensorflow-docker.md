## create a tensorflow jupyter notebook docker

nvidia-docker run --name tf2_notebook -p 8888:8888 -v /home/ubuntu/:/tf -w /tf tensorflow/tensorflow:2.0.0rc0-gpu-py3-jupyter

* **-p 8888:8888**: it will map the docker localhost:8888 to terminal localhost:8888
* **-v /home/ubuntu:/tf**: it will mount /home/ubuntu (in terminal) to /tf (in container)
* **-w /tf**: whenever you log into the container, the default working directory is /tf
