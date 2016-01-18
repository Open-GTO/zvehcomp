# zvehcomp
Vehicle component system

# Usage

```Pawn
new
    compatible_types[MAX_COMPONENT_TYPES],
    compatible_types_count;

GetVehicleCompatibleTypes(400, compatible_types, compatible_types_count);

for (new i = 0; i < compatible_types_count; i++) {
    printf("%d", compatible_types[i]);
}  
```

# Functions

```Pawn
GetComponentTypeId(name[]);
GetComponentTypeName(type, name[], size = sizeof(name));
GetVehicleCompatibleTypes(model, array[MAX_COMPONENT_TYPES], &array_size);
GetComponentName(componentid, cname[], size = sizeof(cname));
GetVehicleCompatibleUpgrades(model, array[MAX_COMPONENTS], &array_size);
IsVehicleUpgradeCompatible(model, componentid);
```

# Constants

```Pawn
INVALID_COMPONENT_ID    (255)
MAX_COMPONENTS          (41)
MAX_COMPONENT_NAME      (64)
MAX_COMPONENT_TYPES     (14)
MAX_COMPONENT_TYPE_NAME (16)
```
