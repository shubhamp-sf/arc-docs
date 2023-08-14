[@sourceloop/authentication-service](../README.md) / [Exports](../modules.md) / User

# Class: User<T\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `DataObject`<`Model`\> |

## Hierarchy

- `UserModifiableEntity`<`T` & [`User`](User.md)\>

  ↳ **`User`**

## Implements

- `IAuthUser`

## Table of contents

### Constructors

- [constructor](User.md#constructor)

### Properties

- [authClientIds](User.md#authclientids)
- [createdBy](User.md#createdby)
- [createdOn](User.md#createdon)
- [credentials](User.md#credentials)
- [defaultTenantId](User.md#defaulttenantid)
- [dob](User.md#dob)
- [email](User.md#email)
- [firstName](User.md#firstname)
- [gender](User.md#gender)
- [id](User.md#id)
- [lastLogin](User.md#lastlogin)
- [lastName](User.md#lastname)
- [middleName](User.md#middlename)
- [modifiedBy](User.md#modifiedby)
- [modifiedOn](User.md#modifiedon)
- [phone](User.md#phone)
- [userTenants](User.md#usertenants)
- [username](User.md#username)

## Constructors

### constructor

• **new User**<`T`\>(`data?`)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `DataObject`<`Model`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `data?` | `Partial`<`T` & [`User`](User.md)<`DataObject`<`Model`\>\>\> |

#### Inherited from

UserModifiableEntity<T & User\>.constructor

#### Defined in

packages/core/dist/models/base-entity.model.d.ts:6

## Properties

### authClientIds

• `Optional` **authClientIds**: `string`

#### Defined in

[services/authentication-service/src/models/user.model.ts:80](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/authentication-service/src/models/user.model.ts#L80)

___

### createdBy

• `Optional` **createdBy**: `string`

#### Inherited from

UserModifiableEntity.createdBy

#### Defined in

packages/core/dist/models/user-modifiable-entity.model.d.ts:4

___

### createdOn

• `Optional` **createdOn**: `Date`

#### Inherited from

UserModifiableEntity.createdOn

#### Defined in

packages/core/dist/models/base-entity.model.d.ts:4

___

### credentials

• **credentials**: [`UserCredentials`](UserCredentials.md)

#### Defined in

[services/authentication-service/src/models/user.model.ts:107](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/authentication-service/src/models/user.model.ts#L107)

___

### defaultTenantId

• **defaultTenantId**: `string`

#### Defined in

[services/authentication-service/src/models/user.model.ts:117](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/authentication-service/src/models/user.model.ts#L117)

___

### dob

• **dob**: `Date`

#### Defined in

[services/authentication-service/src/models/user.model.ts:94](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/authentication-service/src/models/user.model.ts#L94)

___

### email

• `Optional` **email**: `string`

#### Defined in

[services/authentication-service/src/models/user.model.ts:66](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/authentication-service/src/models/user.model.ts#L66)

___

### firstName

• **firstName**: `string`

#### Defined in

[services/authentication-service/src/models/user.model.ts:43](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/authentication-service/src/models/user.model.ts#L43)

___

### gender

• `Optional` **gender**: `Gender`

#### Defined in

[services/authentication-service/src/models/user.model.ts:104](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/authentication-service/src/models/user.model.ts#L104)

___

### id

• `Optional` **id**: `string`

#### Implementation of

IAuthUser.id

#### Defined in

[services/authentication-service/src/models/user.model.ts:36](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/authentication-service/src/models/user.model.ts#L36)

___

### lastLogin

• `Optional` **lastLogin**: `Date`

#### Defined in

[services/authentication-service/src/models/user.model.ts:89](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/authentication-service/src/models/user.model.ts#L89)

___

### lastName

• **lastName**: `string`

#### Defined in

[services/authentication-service/src/models/user.model.ts:49](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/authentication-service/src/models/user.model.ts#L49)

___

### middleName

• `Optional` **middleName**: `string`

#### Defined in

[services/authentication-service/src/models/user.model.ts:55](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/authentication-service/src/models/user.model.ts#L55)

___

### modifiedBy

• `Optional` **modifiedBy**: `string`

#### Inherited from

UserModifiableEntity.modifiedBy

#### Defined in

packages/core/dist/models/user-modifiable-entity.model.d.ts:5

___

### modifiedOn

• `Optional` **modifiedOn**: `Date`

#### Inherited from

UserModifiableEntity.modifiedOn

#### Defined in

packages/core/dist/models/base-entity.model.d.ts:5

___

### phone

• `Optional` **phone**: `string`

#### Defined in

[services/authentication-service/src/models/user.model.ts:74](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/authentication-service/src/models/user.model.ts#L74)

___

### userTenants

• **userTenants**: [`UserTenant`](UserTenant.md)[]

#### Defined in

[services/authentication-service/src/models/user.model.ts:120](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/authentication-service/src/models/user.model.ts#L120)

___

### username

• **username**: `string`

#### Implementation of

IAuthUser.username

#### Defined in

[services/authentication-service/src/models/user.model.ts:61](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/authentication-service/src/models/user.model.ts#L61)
