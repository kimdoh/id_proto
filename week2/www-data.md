Our server as setup last week requires us to use `sudo` to create and edit files on the server, since the `ubuntu` user does not by default have access to 



```
sudo adduser ubuntu www-data
sudo chown -R www-data:www-data /var/www
sudo chmod -R g+rwX /var/www
exit
```

