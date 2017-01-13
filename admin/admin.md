# Admin

## Command line installation with Drush

Reference: 

https://www.drupal.org/documentation/install/developers

Download:

`drush dl drupal --drupal-project-rename=example`

Install:

`drush site-install standard --db-url='mysql://[db_user]:[db_pass]@localhost/[db_name]' --site-name=Example --account-name=admin --account-pass=[useruser_pass]`

Reset:

`drush site-install minimal --site-name=MYSITE`

(May be used along with other options, such as username and password.  Although using "standard" doesn't take much time anyway -- few minutes.)

## Command line theme download and installation with DrupalConsole

This is for an existing theme project on Drupal.org (contributed theme).

Download:

`drupal theme:download THEME-PROJECT-NAME`

Install:

`drupal theme:install THEME-PROJECT-NAME [--set-default]` 

## Command line theme download, installation, and activation with Drush

This is for an existing theme project on Drupal.org (contributed theme).

Download:

`drush dl THEME-PROJECT-NAME`

Install:

`drush en THEME-PROJECT-NAME`

Activate:

`drush config-set system.theme default THEME-PROJECT-NAME'

