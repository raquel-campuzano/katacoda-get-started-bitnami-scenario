In the fifth step, you will learn how to remove the Bitnami badge. 

It contains information about the installed application and links to documentation. It is very useful when you first deploy WordPress and are trying it out, but **you should remove it once your WordPress blog/site starts receiving "real" visitors.**

1. To remove the Bitnami badge, execute this command:

   `sudo /opt/bitnami/apps/wordpress/bnconfig --disable_banner 1`{{execute}}

2. To check if the banner has been removed, navigate to the "Access application" tab. The banner has disappeared from the bottom right corner.
