MySQL

MySQL 连接出现 Authentication plugin 'caching_sha2_password' cannot be loaded

解决方法

show databases;

use mysql;

select host,user,plugin from user where user='root';

更改密码插件，将之前用caching_sha2_password的地方更改为mysql_native_password

ALTER USER 'root'@'%' IDENTIFIED WITH mysql_native_password BY '123456';

'root'为caching_sha2_password的user，通过查询得出

'%'为caching_sha2_password的host，通过查询得出

'123456'为新密码