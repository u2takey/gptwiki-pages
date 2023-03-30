# drush 
## chatgpt 
Drush is a command-line interface tool that allows users to manage and control different aspects of a Drupal website. It stands for "Drupal Shell" and can perform a variety of tasks such as site installation, module management, site updates, and backups.

The basic syntax of a Drush command is:

drush [command] [arguments] [options]

Some common drush commands are:

1. drush help - Displays a list of available commands and their descriptions.

2. drush status - Shows information about the Drupal installation, such as the Drupal version, default theme, and enabled modules.

3. drush dl [module name] - Downloads and installs a Drupal module.

4. drush up - Updates Drupal core, themes, and modules.

5. drush cc all - Clears all Drupal caches.

6. drush sql-dump - Generates a backup of the Drupal database.

7. drush pm-list - Lists all installed Drupal modules.

Overall, Drush is a powerful tool that can help streamline Drupal development and maintenance tasks for website administrators and developers. 

## tldr 
 
> A command-line shell and scripting interface for Drupal.
> More information: <https://www.drush.org>.

- Enable module "foo":

`drush en {{foo}}`

- Uninstall module "foo":

`drush pmu {{foo}}`

- Clear all caches:

`drush cr`

- Clear CSS and JavaScript caches:

`drush cc css-js`
