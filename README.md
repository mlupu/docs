
## server 1 centos cat vrei tu
- apache 2.0 https://archive.apache.org/dist/httpd/httpd-2.0.65.tar.gz -
- php-4.3.11 https://museum.php.net/php4/php-4.3.11.tar.gz
- php-ul asta trebuie sa se conecteze la un oracle ptr asta trebuie instalat instant_client nu conteaza versiunea doar sa mearga

php trebuie configurat asa
```./configure --prefix=/usr/local/php 
--with-apxs2=/usr/local/apache/bin/apxs 
--with-zlib 
--with-gd 
--with-jpeg-dir 
--with-png-dir 
--enable-gd-native-ttf 
--with-ttf-dir=/usr/lib 
--with-freetype-dir=/usr/local/lib 
--with-mysql 
--with-curl 
--with-gettext 
--disable-pear 
--with-dom=/usr/lib  
--with-oci8=shared,instantclient,/opt/oracle/instantclient_19_3/
make
make install
```
## server 2 oracle nu conteaza ce versiune
