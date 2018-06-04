In the third step, you will learn how to use one of the most popular open source editors to work with the Bitnami application files: `[nano](https://www.nano-editor.org/)`. To edit the application files, you can use the text editor of your choice such as Vim or emacs. This is only an example.

This examples show you the basics: how to open, edit, and save the changes you have performed in the file. 

| TIP: Learn more about how to use `nano` in the [GNU nano official documentation](https://www.nano-editor.org/docs.php).

Let's try to edit a file and change one line. Then, we will back to the original version so you can have two opportunities for learning how to use `nano`. To do so:

1. Install nano:

   `sudo apt-get install nano`{{execute}}

2. List the `/opt/bitnami/apps/wordpress/conf/` directory to check all the configuration files present in the WordPress server:

   `ls /opt/bitnami/apps/wordpress/conf/`{{execute}}

3. Open the `banner.conf` file. This is the file where the Bitnami configuration is.

   `nano /opt/bitnami/apps/wordpress/confbanner.conf`{{execute}}

   Does something catch your attention? Not? Look at the bottom of the file, it says: `[ File '/opt/bitnami/apps/wordpress/conf/banner.conf' is unwritable ]`.

   This is because you don't have permissions to edit these kind of files. You need to use `sudo` to write the content of this file. Try again: 

   `sudo nano /opt/bitnami/apps/wordpress/confbanner.conf`{{execute}}

4. Change "YES" to "NO" in the `SetEnv  "DISABLE_BANNER" "YES"` line. 
5. Press the "Control" and the "X" key to exit the file. You will be prompted to save the changes. Type "Y" to confirm. Then, press "M" to save the changes under the same filename. 

Repeat the process to restore the original version to the file: 

6. Reopen the `banner.conf` file.

   `sudo nano /opt/bitnami/apps/wordpress/confbanner.conf`{{execute}}

7. Change "NO" to "YES" in the `SetEnv  "DISABLE_BANNER" "NO"` line. 
8. Press the "Control" and the "X" keys to exit the file. You will be prompted to save the changes. Type "Y" to confirm. Then, press "M" to save the changes under the same filename. 

Do you want to check if your changes have been saved? Let's try one more time:

9. Reopen the `banner.conf` file.

   `sudo nano /opt/bitnami/apps/wordpress/confbanner.conf`{{execute}}

10. Once you make sure that the changes are saved, just press the "Control" and the "X" keys. That's all!
