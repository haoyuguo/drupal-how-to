# Content Type (Node)

## Add an entity bundle

### How-to

Assuming DrupalConsole is installed, use the following command to create a new content type bundle.

`drupal generate:entity:bundle`

It's an interactive process, and the following parameters are entered (if not specified, use default):

```
Enter the module name:
> MODULE_NAME

Enter the machine name of your new content type:
> MACHINE_NAME_FOR_THE_DATA_ENTITY

Enter the human-readable name of your new content type [default]:
> NAME_OF_THE_DATA_ENTITY
```

Alternative use of the same command may be explored to eliminate the interactive process.

### Entity Files Creates Initially

`modules/custom/MODULE_NAME/config/install/core.entity_form_display.node.entity_ENTITY_MACHINE_NAME.default.yml`
`modules/custom/MODULE_NAME/config/install/core.entity_view_display.node.entity_ENTITY_MACHINE_NAME.default.yml`
`modules/custom/MODULE_NAME/config/install/core.entity_view_display.node.entity_ENTITY_MACHINE_NAME.teaser.yml`
`modules/custom/MODULE_NAME/config/install/field.field.node.entity_ENTITY_MACHINE_NAME.body.yml`
`modules/custom/MODULE_NAME/config/install/node.type.entity_ENTITY_MACHINE_NAME.yml`
