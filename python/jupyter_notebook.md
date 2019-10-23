## run jupyter notebook without browser
1. luanch jupyter notebook with command `jupyter notebook --no-browser`
2. map the remote localhost port to the local(the machine has browser) localhost using code
`` ssh -i gehc-explorer.pem -L 8000:localhost:8890 ubuntu@54.213.160.74 ``

## install kernel 
* pip install ipython
* pip install ipykernel 
* ipython kernel install --user --name=<kernel_name>
