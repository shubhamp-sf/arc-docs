[@sourceloop/audit-service](../README.md) / [Exports](../modules.md) / AuditLog

# Class: AuditLog

## Hierarchy

- `CoreEntity`<[`AuditLog`](AuditLog.md)\>

  ↳ **`AuditLog`**

## Indexable

▪ [prop: `string`]: `any`

## Table of contents

### Constructors

- [constructor](AuditLog.md#constructor)

### Properties

- [actedAt](AuditLog.md#actedat)
- [actedOn](AuditLog.md#actedon)
- [action](AuditLog.md#action)
- [actionGroup](AuditLog.md#actiongroup)
- [actionKey](AuditLog.md#actionkey)
- [actor](AuditLog.md#actor)
- [after](AuditLog.md#after)
- [before](AuditLog.md#before)
- [entityId](AuditLog.md#entityid)
- [id](AuditLog.md#id)

## Constructors

### constructor

• **new AuditLog**(`data?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `data?` | `Partial`<[`AuditLog`](AuditLog.md)\> |

#### Inherited from

CoreEntity<AuditLog\>.constructor

#### Defined in

packages/core/dist/models/core-entity.d.ts:3

## Properties

### actedAt

• **actedAt**: `Date`

#### Defined in

[services/audit-service/src/models/audit-log.model.ts:34](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/audit-service/src/models/audit-log.model.ts#L34)

___

### actedOn

• `Optional` **actedOn**: `string`

#### Defined in

[services/audit-service/src/models/audit-log.model.ts:40](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/audit-service/src/models/audit-log.model.ts#L40)

___

### action

• **action**: `Action`

#### Defined in

[services/audit-service/src/models/audit-log.model.ts:27](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/audit-service/src/models/audit-log.model.ts#L27)

___

### actionGroup

• `Optional` **actionGroup**: `string`

#### Defined in

[services/audit-service/src/models/audit-log.model.ts:76](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/audit-service/src/models/audit-log.model.ts#L76)

___

### actionKey

• **actionKey**: `string`

#### Defined in

[services/audit-service/src/models/audit-log.model.ts:47](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/audit-service/src/models/audit-log.model.ts#L47)

___

### actor

• **actor**: `string`

#### Defined in

[services/audit-service/src/models/audit-log.model.ts:60](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/audit-service/src/models/audit-log.model.ts#L60)

___

### after

• `Optional` **after**: `object`

#### Defined in

[services/audit-service/src/models/audit-log.model.ts:70](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/audit-service/src/models/audit-log.model.ts#L70)

___

### before

• `Optional` **before**: `object`

#### Defined in

[services/audit-service/src/models/audit-log.model.ts:65](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/audit-service/src/models/audit-log.model.ts#L65)

___

### entityId

• **entityId**: `string`

#### Defined in

[services/audit-service/src/models/audit-log.model.ts:54](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/audit-service/src/models/audit-log.model.ts#L54)

___

### id

• `Optional` **id**: `string`

#### Defined in

[services/audit-service/src/models/audit-log.model.ts:21](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/audit-service/src/models/audit-log.model.ts#L21)
