[medusa-extender](../README.md) / [Exports](../modules.md) / [medusa-event-emitter](../modules/medusa_event_emitter.md) / [Internals](../modules/medusa_event_emitter.Internals.md) / MedusaEventEmitter

# Class: MedusaEventEmitter

[medusa-event-emitter](../modules/medusa_event_emitter.md).[Internals](../modules/medusa_event_emitter.Internals.md).MedusaEventEmitter

Extended event emitter to register methods that must be call when certain events are triggered and relay the handling to the API package

## Hierarchy

- `EventEmitter`

  ↳ **`MedusaEventEmitter`**

## Table of contents

### Constructors

- [constructor](medusa_event_emitter.Internals.MedusaEventEmitter.md#constructor)

### Properties

- [#listeners](medusa_event_emitter.Internals.MedusaEventEmitter.md##listeners)

### Methods

- [emitAsync](medusa_event_emitter.Internals.MedusaEventEmitter.md#emitasync)
- [register](medusa_event_emitter.Internals.MedusaEventEmitter.md#register)
- [registerListeners](medusa_event_emitter.Internals.MedusaEventEmitter.md#registerlisteners)
- [unregisterListeners](medusa_event_emitter.Internals.MedusaEventEmitter.md#unregisterlisteners)

## Constructors

### constructor

• **new MedusaEventEmitter**()

#### Overrides

EventEmitter.constructor

#### Defined in

[medusa-event-emitter.ts:20](https://github.com/adrien2p/medusa-extender/blob/2b98a6d/src/medusa-event-emitter.ts#L20)

## Properties

### #listeners

• `Private` **#listeners**: `Set`<[`ListenerDescriptor`](../modules/medusa_event_emitter.Internals.md#listenerdescriptor)<`unknown`\>\>

#### Defined in

[medusa-event-emitter.ts:18](https://github.com/adrien2p/medusa-extender/blob/2b98a6d/src/medusa-event-emitter.ts#L18)

## Methods

### emitAsync

▸ **emitAsync**(`eventName`, `values`): `Promise`<`any`\>

Emit an asynchrone event entity based and wait for the result.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `eventName` | `string` \| `symbol` | The event that must be triggered |
| `values` | `Record`<`string`, `unknown`\> | The data that are passed to the event handler |

#### Returns

`Promise`<`any`\>

#### Defined in

[medusa-event-emitter.ts:71](https://github.com/adrien2p/medusa-extender/blob/2b98a6d/src/medusa-event-emitter.ts#L71)

___

### register

▸ **register**<`T`\>(`eventName`, `propertyName`, `metatype`): `void`

Register a new event handler.

#### Type parameters

| Name |
| :------ |
| `T` |

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `eventName` | `string` \| `symbol` | The name of the event that has to be triggered |
| `propertyName` | `string` | The name of the class property that will handle the event |
| `metatype` | [`Metatype`](../modules/types.md#metatype)<`T`\> | The object that contains the property above |

#### Returns

`void`

#### Defined in

[medusa-event-emitter.ts:30](https://github.com/adrien2p/medusa-extender/blob/2b98a6d/src/medusa-event-emitter.ts#L30)

___

### registerListeners

▸ **registerListeners**(`container`): `void`

Apply all event handlers hold by the `listenerDescriptor`.

#### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `container` | `AwilixContainer`<`any`\> | The IoC container that allow to resolve instance |

#### Returns

`void`

#### Defined in

[medusa-event-emitter.ts:42](https://github.com/adrien2p/medusa-extender/blob/2b98a6d/src/medusa-event-emitter.ts#L42)

___

### unregisterListeners

▸ **unregisterListeners**(): `void`

#### Returns

`void`

#### Defined in

[medusa-event-emitter.ts:59](https://github.com/adrien2p/medusa-extender/blob/2b98a6d/src/medusa-event-emitter.ts#L59)