##Install MySQL as Windows service

###MySQL applications

MySQL comes with a number of applications, including mysqld.exe (the Server process), mysql.exe (a Client process that can interact with the Server) and mysqladmin.exe (an administrative application).  These applications can be run from a command prompt, and allow you to perform functions like starting/stopping the database.  However, it is much more convenient to install MySQL as a Windows service, which will allow us to start/stop the server from the Control Panel.  Also, to create a connection in MySQL Workbench (a graphical user interface for managing MySQL databases), we need to have MySQL running as a Windows service.

###Install MySQL as Windows service

Open a command prompt and type the following commands:


~~~
cd \mysql\bin

mysqld --install
~~~


![](../img/service1.png)


###Possible error:

If you receive the message "Install/Remove of Service Denied!" you will need to temporarily disable User Account Control (see User Accounts in the Control Panel), restart your computer, and then try again.  You can re-enable User Account Control once you have installed the service.
  
  

###View service in Control Panel

Go to Administrative Tools, Services (or run services.msc) - you should now see MySQL in the list of services.

![](../img/service2.png)  


###Start/stop service
  
Double-click on the MySQL service to edit its settings.  As the startup type you can choose Automatic (starts up whenever you start the computer) or Manual (must be started manually).  You can also now 'Start' and 'Stop' the service from here.

![](../img/service3.png)

