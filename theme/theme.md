# Theme Related

## Admin toolbar menu item icon

The following works (maybe not the best way):

1. Create new menu link under "admin"

2. Identify the CSS class name of the new menu link.  It should be something like ".toolbar-icon-XXXX".

3. Create a custom theme by extending default "Seven" theme for administration side

4. Create a icon and place it under ADMIN_THEME/images 

5. Create a css file that includes the following 

```
.toolbar-icon-ntsb-XXXX:before {
    background-image: url(/themes/custom/ADMIN_THEME/images/TOOLBAR_ICON_FILE_NAME);
}
```

6. Create a library that applies to all pages, include the above CSS file in the library

7. Choose the new admin theme for administration side

**Known Issue**

Admin page header and breadcrumb are missing.