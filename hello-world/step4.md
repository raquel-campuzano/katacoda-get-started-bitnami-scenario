In the fourth step you will learn how is structured the files directory in any Bitnami application.

### Root directory

The installation process creates several sub-directories under the `/opt/bitnami` directory. To have an overview of the subdirectories and files you can find in it, execute the following:

1. To change the directory:

   `cd /opt/bitnami`{{execute}}

2. To list main subdirectories:

   `ls`{{execute}}

Now, let's see what it is in each subdirectory:

### Servers, databases, and related tools

#### Apache subdirectories

`ls /opt/bitnami/apache2`{{execute}}

* Apache log files:

  `ls /opt/bitnami/apache2/logs/`{{execute}}

* Apache server configuration file:

  `ls /opt/bitnami/apps/wordpress/conf/`{{execute}}

#### MySQL database subdirectories

`ls /opt/bitnami/mysql`{{execute}}

* MySQL configuration files:

  `ls /opt/bitnami/mysql/bitnami/`{{execute}}

### Languages

WordPress is using PHP language, so all the related files you can find under the `php` directory. List it to see its content:

`ls /opt/bitnami/php/`{{execute}}

### Common libraries

In this folder you can find the common libraries that are being used by WordPress. To see them:

`ls /opt/bitnami/common/lib`{{execute}}

### Licenses

This folder includes a list of the licenses of the components included in the stack. List the directory to see them:

`ls /opt/bitnami/licenses/`{{execute}}

### Application files

All the files related to the application are stored under the `apps/wordpress` directory:

`ls /opt/bitnami/apps/wordpress/`{{execute}}

* WordPress files:

  In this directory you can find the content of your WordPress blog, links, comments, login information, configuration, etc.

  `ls /opt/bitnami/apps/wordpress/htdocs`{{execute}}

  Let's try to check one of the files included in the *htdocs* section. In this case, we want to open the *wp-config.php* file so we need to use a text editor. You can use [`nano`](https://www.nano-editor.org/):

  `nano /opt/bitnami/apps/wordpress/htdocs/wp-config.php`{{execute}}

Doesn't work? It is because to check some of these files you need to have the superuser privileges. To do so, you only need to add `sudo` at the beginning of the command you want to execute. Let's try again:

`sudo nano /opt/bitnami/apps/wordpress/htdocs/wp-config.php`{{execute}}

Close the file as you have learned in the previous step.

* WordPress configuration files:

`ls /opt/bitnami/apps/wordpress/conf`{{execute}}
