<a href="https://app.naas.ai/user-redirect/naas/downloader?url=https://raw.githubusercontent.com/jupyter-naas/awesome-notebooks/master/FTP/FTP_Connect.ipynb" target="_parent"><img src="https://naasai-public.s3.eu-west-3.amazonaws.com/open_in_naas.svg"/></a>

**Tags:** #ftp #file

## Input

### Import library


```python
from naas_drivers import ftp
```

### Variables


```python
path = "/path/to/file/in/ftp"
user = "my user"
passwd = "my passwd"
```

## Model

### Connect to ftp


```python
ftp = ftp.connect(user, passwd)
```

## Output

### Get the path


```python
ftp = ftp.connect(user, passwd)
ftp.get(path)
```