<!--
https://readme42.com
-->


[![](https://img.shields.io/pypi/v/django-site-local-middleware.svg?maxAge=3600)](https://pypi.org/project/django-site-local-middleware/)
[![](https://img.shields.io/badge/License-Unlicense-blue.svg?longCache=True)](https://unlicense.org/)
[![](https://github.com/andrewp-as-is/django-site-local-middleware.py/workflows/tests42/badge.svg)](https://github.com/andrewp-as-is/django-site-local-middleware.py/actions)

### Installation
```bash
$ [sudo] pip install django-site-local-middleware
```

#### Examples
`settings.py`

```python
DEBUG=True

MIDDLEWARE = [
    ...
    'django_site_local_middleware.middleware.SiteLocalMiddleware'
    ...
]
```

`/etc/hosts`
```
127.0.0.1   site.com.local
```


```bash
$ python manage.py runserver 0.0.0.0:8000
```

before|after
-|-
`<a href="http://site.com/">`|`<a href="http://site.com.local:8000/">`

<p align="center">
    <a href="https://readme42.com/">readme42.com</a>
</p>
