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

(May be used along with other options, such as username and password.  Although it's not working properly at this time. Using "standard" doesn't take much time anyway -- few minutes.)

`drush site-install standard --db-url='mysql://organized:organized@localhost/organized_d823' --site-name=Organized --account-name=admin --account-pass=password`
