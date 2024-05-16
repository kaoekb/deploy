# Деплой сайта

How To Configure SSH Key-Based Authentication on a Linux Server

Настройка аутентификации на базе ключей SSH на сервере Linux

```
https://www.digitalocean.com/community/tutorials/how-to-configure-ssh-key-based-authentication-on-a-linux-server#step-4-disabling-password-authentication-on-your-server
```

```
cat ~/.ssh/id_rsa.pub | ssh name@ip_name  "mkdir -p ~/.ssh && cat >> ~/.ssh/authorized_keys"
```

How To Install the Apache Web Server on Debian 11

Установка Apache
```
https://www.digitalocean.com/community/tutorials/how-to-install-the-apache-web-server-on-debian-11
```
```
WWW                        ALLOW       Anywhere                  
8080                       ALLOW       Anywhere                  
443                        ALLOW       Anywhere                  
8443                       ALLOW       Anywhere                  
22                         ALLOW       Anywhere         
```
Отправка файлов
```
 scp -r /home/sergiy/photos root@losst.pro:/root/
```

Выдача сертификата для https
```
https://certbot.eff.org/instructions?ws=apache&os=debianbuster&tab=standard
```


Закрыть возможность просматривать папки пользователям
```
https://stackoverflow.com/questions/2530372/how-do-i-disable-directory-browsing
```

Тест 
```
sudo apt install apache2-utils
ab -n 100 -c 50 https://.../
```
