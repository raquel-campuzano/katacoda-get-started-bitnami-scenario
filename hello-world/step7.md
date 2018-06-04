Sometimes something is going wrong with your installation and you don't know where exactly the issue is or how to debug it. To make your life easier when contact to the Bitnami Support Team, we have created the **Bitnami Support Tool**. 

The `bnsupport` CLI gathers prominent information for the Bitnami Support Team for debug specific issues in Bitnami Stacks. It is also a very useful tool specially for self-diagnosis and for troubleshooting common errors. 

**Let's see how to collect important information that you will asked by the Bitnami Support Team when open a case in the [Bitnami Community](https://community.bitnami.com/):**

1. Check if your stack includes or not the **bnsupport tool**, to do so, enter the following URL in your web browser: https://bitnami.com/stack/wordpress/changelog.txt

   > NOTE: This URL is valid for all Bitnami Stacks. You only need to replace "wordpress" with the application name of the stack you have deployed. For example, if you have launched Joomla, you will need to browse to https://bitnami.com/stack/joomla/changelog.txt.

   You should see an entry similar to this:

   ~~~
   Version 4.8.3-0      2017-11-02
   * Add bnsupport tool
   * Updated Apache to 2.4.29
   * Updated MySQL to 5.7.20
   * Updated OpenSSL to 1.0.2l
   * Updated PHP to 7.0.24
   * Updated WordPress to 4.8.3
   ~~~

In case that your stack doesn't include the `bnsupport` tool, [follow these instructions to download it](https://docs.bitnami.com/google/components/bnsupport/).

2. Run the Bitnami Support Tool:

   `sudo /opt/bitnami/bnsupport-tool`{{execute}}

3. Type "Y" when the tool asks you for updates (you are working with the latest version of WordPress). 
4. Enter the `/opt/bitnami` directory as installation directory.
5. Type "n" when you prompted to run Health Tools so it display a summary of the information. Press `Enter` to continue as many times as you are prompted to do it.

   > TIP: For self-diagnosis you can accept to run Health Check tools or the SMTP Test Recipent, for example, and see how the `bnsupport` tool works to help you debug issues on your installation. 

6. Type "y" to add the required information to the archive. This, creates a code that you must paste in your Bitnami Support ticket.

That's all, now you know how to use the `bnsupport` tool for being helped by the Bitnami Support Team!
