# MigrationTestingServer

Check the DB details in [https://github.com/SmithaVerity/IMS/inc/config/constants.php](https://github.com/SmithaVerity/IMS/blob/main/inc/config/constants.php) (localhost) 
and [https://github.com/SmithaVerity/IMS_migrated/inc/config/constants.php](https://github.com/SmithaVerity/IMS_migrated/blob/main/inc/config/constants.php) (RDS DB)

Create an ubuntu instance.
Make sure you are enabling ports 22, 80 and 3306 in the EC2 instance.
Connect the instance using putty and then run the below script
```
git clone https://github.com/SmithaVerity/MigrationTestingServer.git
cd MigrationTestingServer/
sh deployServer.sh
```

Access the applications with the folowing links
http://ipaddresss/IMS
http://ipaddresss/IMS_migrated
