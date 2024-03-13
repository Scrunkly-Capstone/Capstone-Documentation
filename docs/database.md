# Database

## Install

1. Navigate to this URL https://www.pgadmin.org/download/
2. Under the heading that says pgAdmin 4, select the operating system you are using.
3. Follow the intallation instructions it gives you.

## Connet to the Database

1. Open pgAdmin 4: Launch the pgAdmin 4 application on your computer.
2. Register a new server: In the pgAdmin 4 interface, right-click on "Servers" in the left-side browser tree, and select "Register” -> “Server"
3. Configure server details: In the "Register - Server" window, you will see multiple tabs - "General", "Connection", "SSL", and others. Fill in the following details:
    + General tab
        + Name: Provide a name for the connection (e.g., "myAzureFlexInstance").
    + Connection tab
        + Hostname/address: Enter nature-dex.postgres.database.azure.com
        + Port: Leave the port number as is (default is 5432) if you don't want to connect through pgBouncer. If you are using PgBouncer for connection pooling, change the port number to 6432.
        + Maintenance database: Leave the default
        + Username: Enter naturedex
        + Password: Click on the "Save password" checkbox if you want the password to be preserved and enter the corresponding password for the user.
4. Save the configuration: Click the "Save" button to save the server registration. pgAdmin 4 will now establish a connection to your Azure Database for PostgreSQL Flexible Server.
5. Access the database: Once connected, you can expand the server in the browser tree to view databases, schemas, and tables. You can also interact with the server using the built-in query tool and manage your database objects.
