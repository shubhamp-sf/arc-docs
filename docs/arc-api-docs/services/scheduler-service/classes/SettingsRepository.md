[@sourceloop/scheduler-service](../README.md) / [Exports](../modules.md) / SettingsRepository

# Class: SettingsRepository

## Hierarchy

- `DefaultUserModifyCrudRepository`<[`Settings`](Settings.md), `undefined` \| `string`, {}, `this`\> & `DefaultCrudRepository`<[`Settings`](Settings.md), `undefined` \| `string`, `object`, `this`\>

  ↳ **`SettingsRepository`**

## Table of contents

### Constructors

- [constructor](SettingsRepository.md#constructor)

### Properties

- [getAuditLogRepository](SettingsRepository.md#getauditlogrepository)
- [getCurrentUser](SettingsRepository.md#getcurrentuser)

## Constructors

### constructor

• **new SettingsRepository**(`dataSource`, `getCurrentUser`, `getAuditLogRepository`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `dataSource` | `DataSource` |
| `getCurrentUser` | `Getter`<`undefined` \| `IAuthUserWithPermissions`<`string`, `string`, `string`\>\> |
| `getAuditLogRepository` | `Getter`<[`AuditLogRepository`](AuditLogRepository.md)\> |

#### Overrides

ConditionalAuditRepositoryMixin(
  DefaultUserModifyCrudRepository&lt;Settings, typeof Settings.prototype.id, {}\&gt;,
  SettingsAuditOpts,
).constructor

#### Defined in

[services/scheduler-service/src/repositories/settings.repository.ts:27](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/bc2553587/services/scheduler-service/src/repositories/settings.repository.ts#L27)

## Properties

### getAuditLogRepository

• **getAuditLogRepository**: `Getter`<[`AuditLogRepository`](AuditLogRepository.md)\>

#### Defined in

[services/scheduler-service/src/repositories/settings.repository.ts:35](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/bc2553587/services/scheduler-service/src/repositories/settings.repository.ts#L35)

___

### getCurrentUser

• `Protected` `Readonly` **getCurrentUser**: `Getter`<`undefined` \| `IAuthUserWithPermissions`<`string`, `string`, `string`\>\>

#### Inherited from

ConditionalAuditRepositoryMixin(
  DefaultUserModifyCrudRepository<Settings, typeof Settings.prototype.id, {}\>,
  SettingsAuditOpts,
).getCurrentUser

#### Defined in

[services/scheduler-service/src/repositories/settings.repository.ts:31](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/bc2553587/services/scheduler-service/src/repositories/settings.repository.ts#L31)
