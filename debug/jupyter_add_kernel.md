## Jupyter Add Running Kernels

#### 1. Install ipykernel
```bash
$ conda activate env_name
```

make sure you have already installed __ipykernel__
```bash
$ (env_name) python -m ipykernel --version
```

if not, install it first
```bash
$ (env_name) python -m pip install ipykernel
```

#### 2. Add Kernels
```bash
$ python -m ipykernel install --user --name=python3 --display-name py37
```
you can change the name

#### 3. Check Kernel List
```bash
$ jupyter kernelspec list
```

#### 4. Remove Kernel
```bash
$ jupyter kernelspec remove kernelname
```