In the first step we will show you how to connect to the server through SSH. Since Linux come bundled with an SSH client, you only need to perform two steps:

1. Set the permissions for your private key file (*.pem) to 600 using the following command:

`chmod 600 KEYFILE`{{execute}}

2. Connect to the server:

`ssh -i KEYFILE bitnami@SERVER-IP`{{execute}}
