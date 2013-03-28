install
=======

A makefile is a macro for installing Drupal. It contains a list of files that can be fetched using the power of drush, the command line tool for administering Drupal.  

eduerp.make is the EduERP makefile that fetches Drupal, EduERP modules and other dependencies and libraries for a functional EduERP installation 

eduerp.enable is a simple shell script that runs drush commands to establish a default EduERP installation.  


**Requirements**  
1. Web server - Apache or alternative  
2. Database server - MySQL 4.1 or higher, PostgreSQL 7.1  
3. PHP - Drupal 6: PHP 4.4.0 or higher (5.3 recommended)  
4. Drush (preferably from PEAR channel - pear.drush.org)

**Usage**  
+ Create Apache virtualhost for the domain where EduERP will be hosted e.g http://domain.edu.ng  
+ Change directory to the webroot and download the installation files.  
<pre><code>wget --no-check-certificate https://raw.github.com/eduerp/install/master/eduerp.enable</code></pre>
<pre><code>wget --no-check-certificate https://raw.github.com/eduerp/install/master/eduerp.make</code></pre>
+ Run eduerp.make and agree to download -  (downloads Drupal, EduERP, dependent modules and libraries)   
          <pre><code>drush make eduerp.make</code></pre> 
+ Go to URL of the virtualhost e.g http://domain.edu.ng and complete the installation.  
+ Go back to webroot, make eduerp.enable executable and run it  
          <pre><code>chmod a+x eduerp.enable</code></pre> 
          <pre><code>sh eduerp.enable</code></pre>
+ Follow next steps for [Post-Install Config](https://github.com/eduerp/eduerp/wiki/EduERP-Post-Install "Post-Install config")
