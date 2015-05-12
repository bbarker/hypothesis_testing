
Add something like this to the appropriate (port 80 usually) VirtualHost section of your apache config:

```
  <Directory /users/e-prints/htdocstest>
      Order deny,allow
      Allow from all
  </Directory>
  Alias /testing      /users/e-prints/htdocstest

```