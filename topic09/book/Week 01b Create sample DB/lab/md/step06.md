##Create and test connection to server

###Start MySQL Workbench

Launch MySQL Workbench. You will be presented with the Home window. 


###Create new server instance 

To administer your MySQL Server, you must first create a Server Instance. The instance contains information about the target server, including how to connect to it. From the MySQL Workbench Home window, click New Server Instance. The Create New Server Instance Profile wizard will be displayed. 

![](../img/workbench1.png)

In this tutorial, you will connect to a locally installed server, so click Next. 


###Add connection details

Next you will set up a connection, or select an existing connection to use to connect to the server. Assuming that you have not already created a connection, you can use the default values here, although if your MySQL Server has a password set for the root account, you can enter it here by clicking Store in Vault. This enables you to connect to the server without needing to enter a password each time. It is also possible to use a different account to connect to the server by setting the user name and password here, if required. 

![](../img/workbench2.png)

You can now click Next. 


###Connection test

The connection will now be tested. You should see that the connection was successful. If not click Back and check that you have entered the information required. 

![](../img/workbench3.png)

If the connection test was successful, click Next. 


###Windows configuration settings

If a Windows server is used, then the Windows configuration parameters must be set.  You should see the service you created in Step 4 in the drop down list; select this service.  Click the ... icon next the 'path to configuration file' box and navigate to C:\\mysql and select the my-default.ini file.

![](../img/workbench4.png)

Check that everything is in order, then click Next.


###Test host settings

The wizard will now check that it is able to access the MySQL Server configuration file, and access the start and stop commands. 

![](../img/workbench5.png)

Once this is done, click Next to move on.


###Review settings

You now have a chance to review the configuration settings so far. The information displayed varies slightly depending on platform, connection method and installation type. 

![](../img/workbench6.png)

Review the information, then click Next.


###Complete setup

Finally you can give the server instance a suitable name. This will be used to select this particular instance from a list of available instances.  The default name of mysqld@localhost is fine. 

![](../img/workbench7.png)

Click Finish.


###Server Administration

You will now be returned to the Home window. You will see the new server instance you created, along with the new connection you created as part of the preceding procedure. From the Home window, double-click the Server Instance you created. The Administrator will open on the Startup configuration page. 

![](../img/workbench8.png)


###Start/stop the server

In the Startup/Shutdown tab of the Admin window, you can determine whether the database server instance is running.  Click Stop server to stop the database instance and Start to start it again.

![](../img/workbench9.png)









