[medusa-extender](../README.md) / [Exports](../modules.md) / cli/commands/generate-component

# Module: cli/commands/generate-component

## Table of contents

### Namespaces

- [Internals](cli_commands_generate_component.Internals.md)

### Functions

- [createComponentIfNecessary](cli_commands_generate_component.md#createcomponentifnecessary)
- [generateComponent](cli_commands_generate_component.md#generatecomponent)
- [updateModuleImports](cli_commands_generate_component.md#updatemoduleimports)

## Functions

### createComponentIfNecessary

▸ **createComponentIfNecessary**(`__namedParameters`, `content`): `void`

Create the component file and fill it with the template content.

#### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | `Object` |
| `__namedParameters.componentFileName` | `string` |
| `__namedParameters.componentName` | `string` |
| `__namedParameters.fullDestinationPath` | `string` |
| `content` | `string` |

#### Returns

`void`

#### Defined in

[src/cli/commands/generate-component.ts:106](https://github.com/adrien2p/medusa-extender/blob/30feff3/src/cli/commands/generate-component.ts#L106)

___

### generateComponent

▸ **generateComponent**(`name`, `__namedParameters`): `void`

Generate the required components from the user command.

#### Parameters

| Name | Type |
| :------ | :------ |
| `name` | `string` |
| `__namedParameters` | [`Options`](cli_commands_generate_component.Internals.md#options) |

#### Returns

`void`

#### Defined in

[src/cli/commands/generate-component.ts:45](https://github.com/adrien2p/medusa-extender/blob/30feff3/src/cli/commands/generate-component.ts#L45)

___

### updateModuleImports

▸ **updateModuleImports**(`fullDestinationPath`): `void`

Lookup for the closest module from the component and update its imports.

#### Parameters

| Name | Type |
| :------ | :------ |
| `fullDestinationPath` | `string` |

#### Returns

`void`

#### Defined in

[src/cli/commands/generate-component.ts:133](https://github.com/adrien2p/medusa-extender/blob/30feff3/src/cli/commands/generate-component.ts#L133)