## django mariadb 연동

``` bash
$ pip install mysqlclient
```



- 원래 default setting

``` python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': BASE_DIR / 'db.sqlite3',  
    }
}
```

- 변경

``` python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'maria', ## 데이터베이스 이름 
        'USER': 'root', 
        'PASSWORD': 'mysql',
        'HOST': 'localhost',
        'PORT': '3306'
    }
}
```

 