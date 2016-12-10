# Controller Related

## How to Use DrupalConsole to Create a Controller

Assuming DrupalConsole is installed, use the following command to create a new controller.

`drupal generate:controller`

It's an interactive process, and the following parameters are entered (if not specified, use default):

```
Enter the module name:
> MODULE_NAME

Enter the Controller class name:
> DESIRED_CONTROLLER_CLASS_NAME

Enter the Controller method title (leave empty and press enter when done):
> DESIRED_CONTROLLER_METHOD_TITLE

Enter the action method name:
> DESIRED_CONTROLLER_METHOD(_FUNCTION)_NAME

Enter the route path:
> DESIRED_ROUTE_PATH (e.g. /home/hello)
```

**Generated or updated files**

`modules/custom/MODULE_NAME/src/Controller/DESIRED_CONTROLLER_CLASS_NAME.php`
`modules/custom/MODULE_NAME/MODULE_NAME.routing.yml`
`modules/custom/MODULE_NAME/Tests/Controller/DESIRED_CONTROLLER_CLASS_NAMETest.php`

_Note that permissions are not set in the end of the process.  This will need to be done separately._

## How to Use DrupalConsole to Rebuild Routers

`drupal router:rebuild`
