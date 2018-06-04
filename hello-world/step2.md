In the second step we are going to see how to stop, start, or restart the server and/or the services using the Bitnami control script. The script is located at `/opt/bitnami/ctlscript.sh`. 

Let's try the following options:

1. Start all services:

   `sudo /opt/bitnami/ctlscript.sh start`{{execute}}

2. Restart a single service such as Apache:

   `sudo /opt/bitnami/ctlscript.sh restart apache`{{execute}}

3. Stop all services:

   `sudo /opt/bitnami/ctlscript.sh stop`{{execute}}

4. Restart all the services:

   `sudo /opt/bitnami/ctlscript.sh restart`{{execute}}

5. List of available services and operations:

   `sudo /opt/bitnami/ctlscript.sh`{{execute}}
