====
Django Channel Featuring API
===

This is a simple API using django-channel (https://github.com/django/channels). We can make it as a separate application from our main django project

Prequisites
----------

This module depends on 'channel' and 'asgi_redis' (or other channel backend). You can change this on your settings.py

Quick starti
-----------

1. Add 'channel_api' to your INSTALLED_APPS setting like this

    ````
    INSTALLED_APPS = [
        ...
	'channel',
	'asgi_redis',
        'channel_api',
    ]
   ```

2. Include the django-channel-api URLconf in your project urls.py
    `url(r'^channel/', include('channel_api.urls')),`

