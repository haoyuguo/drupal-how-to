# Content Entity (Data)

## Add a new entity

### How-to

Assuming DrupalConsole is installed, use the following command to create a new content entity.

`drupal generate:entity:content`

It's an interactive process, and the following parameters are entered (if not specified, use default):

```
Enter the module name:
> MODULE_NAME

Enter the class of your new content entity [DefaultEntity]:
> DESIRED_CLASS_NAME_FOR_THE_ENTITY

Enter the name of your new content entity:
> DESIRED_(MACHINE?_)NAME_OF_THE_ENTITY

Enter the label of your new content entity:
> DESIRED_LABEL

Enter the base-path for the content entity routes [/admin/structure]:
> DESIRED_BASE_PATH
```
 
Per instruction provided at the end of the command, add this to your hook_theme:

```
  $theme['NAME_OF_THE_ENTITY'] = array(
    'render element' => 'elements',
    'file' => 'NAME_OF_THE_ENTITY.page.inc',
    'template' => 'NAME_OF_THE_ENTITY',
  );
```
 
Alternative use of the same command may be explored to eliminate the interactive process.

**Generated or updated files**

`modules/custom/MODULE_NAME/MODULE_NAME.permissions.yml`
`modules/custom/MODULE_NAME/MODULE_NAME.links.menu.yml`
`modules/custom/MODULE_NAME/MODULE_NAME.links.task.yml`
`modules/custom/MODULE_NAME/MODULE_NAME.links.action.yml`
`modules/custom/MODULE_NAME/src/ENTITY_CLASS_NAMEInterface.php`
`modules/custom/MODULE_NAME/src/ENTITY_CLASS_NAMEAccessControlHandler.php`
`modules/custom/MODULE_NAME/src/Entity/ENTITY_CLASS_NAME.php`
`modules/custom/MODULE_NAME/src/ENTITY_CLASS_NAMEHtmlRouteProvider.php`
`modules/custom/MODULE_NAME/src/Entity/ENTITY_CLASS_NAMEViewsData.php`
`modules/custom/MODULE_NAME/src/ENTITY_CLASS_NAMEListBuilder.php`
`modules/custom/MODULE_NAME/src/Form/ENTITY_CLASS_NAMESettingsForm.php`
`modules/custom/MODULE_NAME/src/Form/ENTITY_CLASS_NAMEForm.php`
`modules/custom/MODULE_NAME/src/Form/ENTITY_CLASS_NAMEDeleteForm.php`
`modules/custom/MODULE_NAME/ENTITY_NAME.page.inc`
`modules/custom/MODULE_NAME/templates/ENTITY_NAME.html.twig`

**Note that the instruction for theming causes numerous errors/warnings in log.  Not sure what to do with it yet.** 

One alternative is to move this part to theme, instead of keeping in module. 
