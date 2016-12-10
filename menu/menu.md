# Menu Related

## Add an admin menu

To add a new item under admin menu, add something like this to the 

```
entity.new_menu_item.collection:
  title: 'New Menu Item'
  route_name: A.VALID.ROUTE.NAME.DEFINED.ELSEWHERE
  parent: system.admin
```

or 

```
entity.new_menu_item.collection:
  title: 'New Menu Item'
  url: 'A VALID EXTERNAL URL STARTING WITH HTTP OR HTTPS'
  parent: system.admin
```

