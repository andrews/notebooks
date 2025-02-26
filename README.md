# Creating jupyter kernels
It would be nice to have different kernels for different projects or use-cases!

After installing `ipykernel`, you can create kernels from specific virtual environments using the below command. Make sure the virtual environment is activated first.
```
pip install ipykernel # if you didn't install it
python3 -m ipykernel install --user --name myenv --display-name "Python (myenv)"
```
To view the list of available kernels:
```
jupyter kernelspec list
```
If this doesn't work, make sure your jupyter packages are up to date. I needed to run this on Ubuntu 24.04. Originally, listing the kernels was only working when I activated a venv. This command let me run it even when outside of a venv.
```
sudo apt install jupyter
```
To create your own virtual environment:
```
python3 -m venv myenv
```
To delete a jupyter kernel:
```
jupyter kernelspec uninstall unwanted-kernel
```
