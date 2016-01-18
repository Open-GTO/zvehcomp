# zvehcomp
Vehicle component system

# Provides functions

```Pawn
GetComponentTypeId(name[]);
GetComponentTypeName(type, name[], size = sizeof(name));
GetVehicleCompatibleTypes(model, array[MAX_COMPONENT_TYPES], &array_size);
GetComponentName(componentid, cname[], size = sizeof(cname));
GetVehicleCompatibleUpgrades(model, array[MAX_COMPONENTS], &array_size);
IsVehicleUpgradeCompatible(model, componentid);
```

# Provides constants

```Pawn
INVALID_COMPONENT_ID    (255)
MAX_COMPONENTS          (35)
MAX_COMPONENT_NAME      (64)
MAX_COMPONENT_TYPES     (14)
MAX_COMPONENT_TYPE_NAME (16)
```
