
Instance- 1
__________________


root user without the proper authorisation.
You already have a root password set, so you can safely answer 'n'.
Change the root password? [Y/n] n
 ... skipping.
By default, a MariaDB installation has an anonymous user, allowing anyone
to log into MariaDB without having to have a user account created for
them.  This is intended only for testing, and to make the installation
go a bit smoother.  You should remove them before moving into a
production environment.
Remove anonymous users? [Y/n] n
 ... skipping.
Normally, root should only be allowed to connect from 'localhost'.  This
ensures that someone cannot guess at the root password from the network.
Disallow root login remotely? [Y/n] y
 ... Success!
By default, MariaDB comes with a database named 'test' that anyone can
access.  This is also intended only for testing, and should be removed
before moving into a production environment.
Remove test database and access to it? [Y/n] y
 - Dropping test database...
 ... Success!
 - Removing privileges on test database...
 ... Success!
Reloading the privilege tables will ensure that all changes made so far
will take effect immediately.
Reload privilege tables now? [Y/n] y
 ... Success!
Cleaning up...
All done!  If you've completed all of the above steps, your MariaDB
installation should now be secure.


____________________



Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 16
Server version: 5.5.56-MariaDB MariaDB Server

Copyright (c) 2000, 2017, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [(none)]> flush privileges;
Query OK, 0 rows affected (0.00 sec)

MariaDB [(none)]> flush privileges;
Query OK, 0 rows affected (0.00 sec)

MariaDB [(none)]> grant all on *.* to 'temp'@'%' identified by 'temp' with grant option;
Query OK, 0 rows affected (0.00 sec)
MariaDB [(none)]> flush privileges
    -> ;
Query OK, 0 rows affected (0.00 sec)
MariaDB [(none)]> create database scm DEFAULT CHARACTER SET utf8;
Query OK, 1 row affected (0.00 sec)
MariaDB [(none)]> create database rman  DEFAULT CHARACTER SET utf8;
Query OK, 1 row affected (0.00 sec)
MariaDB [(none)]> create database hive DEFAULT CHARACTER SET utf8;
Query OK, 1 row affected (0.00 sec)
MariaDB [(none)]> create database oozie DEFAULT CHARACTER SET utf8;
Query OK, 1 row affected (0.00 sec)
MariaDB [(none)]> create database hue DEFAULT CHARACTER SET utf8;
Query OK, 1 row affected (0.00 sec)
MariaDB [(none)]> create database sentry DEFAULT CHARACTER SET utf8;
Query OK, 1 row affected (0.00 sec)
MariaDB [(none)]>  
MariaDB [(none)]> 
MariaDB [(none)]> grant all on scm.* TO 'scm'@'%' IDENTIFIED BY 'bigdata';
Query OK, 0 rows affected (0.00 sec)
MariaDB [(none)]> grant all on rman.* TO 'rman'@'%' IDENTIFIED BY 'bigdata'; 
Query OK, 0 rows affected (0.00 sec)
MariaDB [(none)]> grant all on hive.* TO 'hive'@'%' IDENTIFIED BY 'bigdata';
Query OK, 0 rows affected (0.00 sec)
MariaDB [(none)]> grant all on oozie.* TO 'oozie'@'%' IDENTIFIED BY 'bigdata';
Query OK, 0 rows affected (0.00 sec)
MariaDB [(none)]> grant all on hue.* TO 'hue'@'%' IDENTIFIED BY 'bigdata'; 
Query OK, 0 rows affected (0.00 sec)
MariaDB [(none)]> grant all on sentry.* TO 'sentry'@'%' IDENTIFIED BY 'bigdata'; 
Query OK, 0 rows affected (0.00 sec)
MariaDB [(none)]> 
MariaDB [(none)]> flush privileges





__________________



