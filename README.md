# zvehcomp
Vehicle components useful functions.

# Usage

```Pawn
new
    compatible_types[ZVEH_MAX_COMPONENT_TYPES],
    compatible_types_count;

GetVehicleCompatibleTypes(400, compatible_types, compatible_types_count);

for (new i = 0; i < compatible_types_count; i++) {
    printf("%d", compatible_types[i]);
}
```

# Functions

```Pawn
GetVehicleComponentTypeId(name[]);
GetVehicleComponentTypeName(type, name[], size = sizeof(name));
GetVehicleCompatibleTypes(model, array[ZVEH_MAX_COMPONENT_TYPES], &array_size);
GetVehicleComponentName(componentid, cname[], size = sizeof(cname));
GetVehicleCompatibleUpgrades(model, array[ZVEH_MAX_COMPONENTS], &array_size);
IsVehicleUpgradeCompatible(model, componentid);
IsVehicleHaveUpgrades(model);
```

# Directives

Directive | Default value | Can be redefined
----------|---------------|------------
ZVEH_INVALID_COMPONENT_ID | 255 | no
ZVEH_MAX_COMPONENTS | 48 | no
ZVEH_MAX_COMPONENT_NAME | 64 | no
ZVEH_MAX_COMPONENT_TYPES | 14 | no
ZVEH_MAX_COMPONENT_TYPE_NAME | 16 | no
