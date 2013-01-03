install
=======

A makefile is a macro for installing Drupal. It contains a list of files that can be fetched using the power of drush, the command line tool for administering Drupal.  

eduerp.make is the EduERP makefile that fetches Drupal, EduERP modules and other dependencies for a functional EduERP installation 

eduerp.enable is a simple shell script that runs drush commands to establish a default EduERP installation.  


Requirements:  
Web server - Apache or alternative  
Database server - MySQL 4.1 or higher, PostgreSQL 7.1  
PHP - Drupal 6: PHP 4.4.0 or higher (5.3 recommended)  
Drush
