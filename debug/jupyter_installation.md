## Jupyter Notebook Linux

### Installation
#### 1. Enter Virtual Environments
```bash
$ conda activate env_name
```

#### 2. Install
```bash
$ pip install jupyter
```

#### 3. Generate Config File
```bash
$ jupyter notebook --generate-config
```

#### 4. Set Password
```bash
$ python
```

```python
from IPython.lib import passwd
passwd()
# Enter password:
# Verify password: 
```
You will get a password string here

#### 5. Edit Config File
```bash
$ vim ~/.jupyter/jupyter_notebook_config.py
```
add some information here

```
c.NotebookApp.allow_remote_access = True
c.NotebookApp.ip = '*'
c.NotebookApp.open_browser = False    # we don't want to open it directly on the Server, set False
c.NotebookApp.password = 'sha1:1058604ee835:4fb758cac6ee47f2ff8d80c1735e219f26e34d98'    # the password
c.NotebookApp.port = 8888    # any port you like
```

#### 6. Start
```bash
$ jupyter notebook
```