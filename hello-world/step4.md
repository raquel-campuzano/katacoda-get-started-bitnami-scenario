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

`ls apache2`{{execute}}

* Apache log files:

`ls apache2/logs/`{{execute}}

* Apache server configuration file:

`ls apps/wordpress/conf/`{{execute}}

#### MySQL database subdirectories

`ls mysql`{{execute}}

* MySQL configuration files:

`ls mysql/bitnami/`{{execute}}

### Languages

WordPress is using PHP language, so all the related files you can find under the `php` directory. List it to see its content:

`ls php/`{{execute}}

### Common libraries

In this folder you can find the common libraries that are being used by WordPress. To see them:

`ls common/lib`{{execute}}

### Licenses

This folder includes a list of the licenses of the components included in the stack. List the directory to see them:

`ls licenses/`{{execute}}

### Application files

All the files related to the application are stored under the `apps/wordpress` directory:

`ls apps/wordpress/`{{execute}}

* WordPress files:

  In this directory you can find the content of your WordPress blog, links, comments, login information, configuration, etc.

  `ls apps/wordpress/htdocs`{{execute}}

  To check some of these files you need to have the superuser privileges. To do so, you only need to add `sudo` at the beginning of the command you want to execute. In this case, we want to open the *wp-config.php* file so we need to use a text editor such as [`cat`](https://www.linux.com/blog/using-cat-text-editor):

  `sudo cat apps/wordpress/htdocs/wp-config.php`{{execute}}

* WordPress configuration files:

`ls apps/wordpress/conf`{{execute}}
~
