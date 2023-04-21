[@sourceloop/search-service](../README.md) / [Exports](../modules.md) / SearchQueryBuilder

# Class: SearchQueryBuilder<T\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `Model` |

## Hierarchy

- **`SearchQueryBuilder`**

  ↳ [`MySqlQueryBuilder`](MySqlQueryBuilder.md)

  ↳ [`PsqlQueryBuilder`](PsqlQueryBuilder.md)

## Table of contents

### Constructors

- [constructor](SearchQueryBuilder.md#constructor)

### Properties

- [\_placeholderIndex](SearchQueryBuilder.md#_placeholderindex)
- [baseQueryList](SearchQueryBuilder.md#basequerylist)
- [idType](SearchQueryBuilder.md#idtype)
- [limitQuery](SearchQueryBuilder.md#limitquery)
- [modelNameMap](SearchQueryBuilder.md#modelnamemap)
- [orderQuery](SearchQueryBuilder.md#orderquery)
- [query](SearchQueryBuilder.md#query)
- [schema](SearchQueryBuilder.md#schema)
- [unionString](SearchQueryBuilder.md#unionstring)

### Accessors

- [placeholder](SearchQueryBuilder.md#placeholder)

### Methods

- [\_formatColumnSameInDb](SearchQueryBuilder.md#_formatcolumnsameindb)
- [\_isQuery](SearchQueryBuilder.md#_isquery)
- [build](SearchQueryBuilder.md#build)
- [buildClauseFromExpress](SearchQueryBuilder.md#buildclausefromexpress)
- [buildColumnValueForExpression](SearchQueryBuilder.md#buildcolumnvalueforexpression)
- [buildExpression](SearchQueryBuilder.md#buildexpression)
- [getColumnListFromArray](SearchQueryBuilder.md#getcolumnlistfromarray)
- [getColumnListFromArrayOrMap](SearchQueryBuilder.md#getcolumnlistfromarrayormap)
- [getColumnListFromMap](SearchQueryBuilder.md#getcolumnlistfrommap)
- [getColumnName](SearchQueryBuilder.md#getcolumnname)
- [getModelName](SearchQueryBuilder.md#getmodelname)
- [getSchemaName](SearchQueryBuilder.md#getschemaname)
- [getTableName](SearchQueryBuilder.md#gettablename)
- [handleAndOr](SearchQueryBuilder.md#handleandor)
- [handleKeys](SearchQueryBuilder.md#handlekeys)
- [handleObjectValue](SearchQueryBuilder.md#handleobjectvalue)
- [limit](SearchQueryBuilder.md#limit)
- [order](SearchQueryBuilder.md#order)
- [paramString](SearchQueryBuilder.md#paramstring)
- [paramsBuild](SearchQueryBuilder.md#paramsbuild)
- [parseIdPlaceholder](SearchQueryBuilder.md#parseidplaceholder)
- [queryBuild](SearchQueryBuilder.md#querybuild)
- [search](SearchQueryBuilder.md#search)
- [toArrayPropTypes](SearchQueryBuilder.md#toarrayproptypes)
- [toColumnValue](SearchQueryBuilder.md#tocolumnvalue)
- [toDateType](SearchQueryBuilder.md#todatetype)
- [whereBuild](SearchQueryBuilder.md#wherebuild)

## Constructors

### constructor

• **new SearchQueryBuilder**<`T`\>(`query`, `schema?`)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `Model`<`T`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `query` | `DataObject`<[`SearchQuery`](SearchQuery.md)\> |
| `schema?` | `string` |

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:46](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L46)

## Properties

### \_placeholderIndex

• `Protected` **\_placeholderIndex**: `number` = `0`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:35](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L35)

___

### baseQueryList

• `Protected` **baseQueryList**: [`Query`](../modules.md#query)[]

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:29](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L29)

___

### idType

• `Protected` `Optional` **idType**: `string` = `'uuid'`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:34](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L34)

___

### limitQuery

• `Protected` **limitQuery**: `string`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:30](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L30)

___

### modelNameMap

• `Protected` **modelNameMap**: `Map`<`string`, `string`\>

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:36](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L36)

___

### orderQuery

• `Protected` **orderQuery**: `string`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:31](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L31)

___

### query

• `Protected` **query**: `DataObject`<[`SearchQuery`](SearchQuery.md)\>

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:32](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L32)

___

### schema

• `Protected` `Optional` **schema**: `string`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:33](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L33)

___

### unionString

• `Abstract` **unionString**: `string`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:56](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L56)

## Accessors

### placeholder

• `Protected` `get` **placeholder**(): `string`

#### Returns

`string`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:37](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L37)

• `Protected` `set` **placeholder**(`val`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `string` \| `number` |

#### Returns

`void`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:41](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L41)

## Methods

### \_formatColumnSameInDb

▸ `Private` **_formatColumnSameInDb**(`modelColumn`, `dbColumn`): `string` \| keyof `T`

#### Parameters

| Name | Type |
| :------ | :------ |
| `modelColumn` | keyof `T` |
| `dbColumn` | `string` |

#### Returns

`string` \| keyof `T`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:578](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L578)

___

### \_isQuery

▸ `Private` **_isQuery**(`query`): query is Query

#### Parameters

| Name | Type |
| :------ | :------ |
| `query` | [`ShortHandEqualType`](../modules.md#shorthandequaltype) \| [`Query`](../modules.md#query) |

#### Returns

query is Query

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:574](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L574)

___

### build

▸ **build**(`models`, `ignoredColumns?`, `type?`, `idType?`): `Object`

#### Parameters

| Name | Type |
| :------ | :------ |
| `models` | (typeof `Model` \| [`SearchableModel`](SearchableModel.md)<`T`, typeof `Model`\>)[] |
| `ignoredColumns?` | `Exclude`<keyof `T`, ``"toJSON"`` \| ``"toObject"`` \| ``"getId"`` \| ``"getIdObject"``\>[] |
| `type?` | typeof `Model` |
| `idType?` | `string` |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `params` | `AnyObject` \| (`string` \| `AnyObject`)[] |
| `query` | `string` |

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:58](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L58)

___

### buildClauseFromExpress

▸ **buildClauseFromExpress**(`values`, `separator`, `grouping`, `getPlaceholder`): [`Query`](../modules.md#query)

#### Parameters

| Name | Type |
| :------ | :------ |
| `values` | [`ShortHandEqualType`](../modules.md#shorthandequaltype) \| [`Query`](../modules.md#query) \| ([`ShortHandEqualType`](../modules.md#shorthandequaltype) \| [`Query`](../modules.md#query))[] |
| `separator` | `string` |
| `grouping` | `boolean` |
| `getPlaceholder` | () => `string` |

#### Returns

[`Query`](../modules.md#query)

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:523](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L523)

___

### buildColumnValueForExpression

▸ **buildColumnValueForExpression**(`expressionValue`, `p`): `any`[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `expressionValue` | [`PredicateValueType`](../modules.md#predicatevaluetype)<[`ShortHandEqualType`](../modules.md#shorthandequaltype)\> |
| `p` | `PropertyDefinition` |

#### Returns

`any`[]

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:362](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L362)

___

### buildExpression

▸ **buildExpression**(`columnName`, `prop`, `operator`, `value`, `model`): `Object`

#### Parameters

| Name | Type |
| :------ | :------ |
| `columnName` | keyof `T` |
| `prop` | `PropertyDefinition` |
| `operator` | `string` |
| `value` | [`ShortHandEqualType`](../modules.md#shorthandequaltype) \| [`Query`](../modules.md#query) \| ([`ShortHandEqualType`](../modules.md#shorthandequaltype) \| [`Query`](../modules.md#query))[] |
| `model` | typeof `Model` |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `params` | [`ShortHandEqualType`](../modules.md#shorthandequaltype)[] |
| `sql` | `string` |

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:459](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L459)

___

### getColumnListFromArray

▸ **getColumnListFromArray**(`model`, `columns`, `filter`): `Object`

#### Parameters

| Name | Type |
| :------ | :------ |
| `model` | typeof `Model` |
| `columns` | keyof `T`[] |
| `filter` | keyof `T`[] |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `columnList` | `string` |
| `selectors` | `string` |

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:173](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L173)

___

### getColumnListFromArrayOrMap

▸ **getColumnListFromArrayOrMap**(`model`, `columns`, `filter`): `Object`

#### Parameters

| Name | Type |
| :------ | :------ |
| `model` | typeof `Model` |
| `columns` | keyof `T`[] \| [`ColumnMap`](../modules.md#columnmap)<`T`\> |
| `filter` | keyof `T`[] |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `columnList` | `string` |
| `selectors` | `string` |

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:132](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L132)

___

### getColumnListFromMap

▸ **getColumnListFromMap**(`model`, `columns`, `filter`): `Object`

#### Parameters

| Name | Type |
| :------ | :------ |
| `model` | typeof `Model` |
| `columns` | [`ColumnMap`](../modules.md#columnmap)<`T`\> |
| `filter` | keyof `T`[] |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `columnList` | `string` |
| `selectors` | `string` |

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:144](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L144)

___

### getColumnName

▸ **getColumnName**(`model`, `name`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `model` | typeof `Model` |
| `name` | keyof `T` |

#### Returns

`any`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:385](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L385)

___

### getModelName

▸ **getModelName**(`model`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `model` | typeof `Model` |

#### Returns

`string`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:569](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L569)

___

### getSchemaName

▸ **getSchemaName**(`model`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `model` | typeof `Model` |

#### Returns

`string`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:565](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L565)

___

### getTableName

▸ **getTableName**(`model`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `model` | typeof `Model` |

#### Returns

`string`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:561](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L561)

___

### handleAndOr

▸ **handleAndOr**<`S`\>(`where`, `key`, `model`): `undefined` \| [`Query`](../modules.md#query)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `S` | extends typeof `Model` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `where` | [`SearchWhereFilter`](../modules.md#searchwherefilter)<`AnyObject`\> |
| `key` | `never` |
| `model` | `S` |

#### Returns

`undefined` \| [`Query`](../modules.md#query)

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:306](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L306)

___

### handleKeys

▸ **handleKeys**(`model`, `key`, `where`): `undefined` \| [`Query`](../modules.md#query) \| [`Queries`](../modules.md#queries)

#### Parameters

| Name | Type |
| :------ | :------ |
| `model` | typeof `Model` |
| `key` | `never` |
| `where` | [`SearchWhereFilter`](../modules.md#searchwherefilter)<`AnyObject`\> |

#### Returns

`undefined` \| [`Query`](../modules.md#query) \| [`Queries`](../modules.md#queries)

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:263](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L263)

___

### handleObjectValue

▸ **handleObjectValue**<`S`\>(`expression`, `p`, `key`, `model`): `undefined` \| [`Query`](../modules.md#query)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `S` | extends typeof `Model` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `expression` | [`PredicateComparison`](../modules.md#predicatecomparison)<[`ShortHandEqualType`](../modules.md#shorthandequaltype)\> |
| `p` | `PropertyDefinition` |
| `key` | `never` |
| `model` | `S` |

#### Returns

`undefined` \| [`Query`](../modules.md#query)

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:337](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L337)

___

### limit

▸ **limit**(): `void`

#### Returns

`void`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:77](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L77)

___

### order

▸ **order**(`columns`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `columns` | keyof `T`[] |

#### Returns

`void`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:102](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L102)

___

### paramString

▸ **paramString**(`index`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `index` | `number` |

#### Returns

`string`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:202](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L202)

___

### paramsBuild

▸ **paramsBuild**(`param`): `AnyObject` \| (`string` \| `AnyObject`)[]

#### Parameters

| Name | Type |
| :------ | :------ |
| `param` | `string` |

#### Returns

`AnyObject` \| (`string` \| `AnyObject`)[]

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:194](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L194)

___

### parseIdPlaceholder

▸ **parseIdPlaceholder**(`prop`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `prop` | `PropertyDefinition` |

#### Returns

`string`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:377](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L377)

___

### queryBuild

▸ **queryBuild**(`models`, `ignoredColumns?`, `type?`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `models` | (typeof `Model` \| [`SearchableModel`](SearchableModel.md)<`T`, typeof `Model`\>)[] |
| `ignoredColumns?` | keyof `T`[] |
| `type?` | typeof `Model` |

#### Returns

`string`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:206](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L206)

___

### search

▸ `Abstract` **search**(`model`, `columns`, `ignoredColumns`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `model` | typeof `Model` |
| `columns` | keyof `T`[] \| [`ColumnMap`](../modules.md#columnmap)<`T`\> |
| `ignoredColumns` | keyof `T`[] |

#### Returns

`void`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:50](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L50)

___

### toArrayPropTypes

▸ **toArrayPropTypes**<`R`\>(`prop`, `val`): `any`

#### Type parameters

| Name |
| :------ |
| `R` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `prop` | `PropertyDefinition` |
| `val` | `R` \| `R`[] |

#### Returns

`any`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:441](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L441)

___

### toColumnValue

▸ **toColumnValue**(`prop`, `val`): `any`

#### Parameters

| Name | Type |
| :------ | :------ |
| `prop` | `PropertyDefinition` |
| `val` | [`PredicateValueType`](../modules.md#predicatevaluetype)<[`ShortHandEqualType`](../modules.md#shorthandequaltype)\> |

#### Returns

`any`

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:392](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L392)

___

### toDateType

▸ **toDateType**(`val`): `Object`

#### Parameters

| Name | Type |
| :------ | :------ |
| `val` | `string` \| `Date` |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `params` | `string`[] |
| `sql` | `string` |

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:428](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L428)

___

### whereBuild

▸ **whereBuild**<`S`\>(`model`, `where?`): `Object`

#### Type parameters

| Name | Type |
| :------ | :------ |
| `S` | extends typeof `Model` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `model` | `S` |
| `where?` | [`SearchWhereFilter`](../modules.md#searchwherefilter)<`AnyObject`\> |

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `params` | [`ShortHandEqualType`](../modules.md#shorthandequaltype)[] |
| `sql` | `string` |

#### Defined in

[services/search-service/src/classes/base/query.builder.ts:249](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/6c16af104/services/search-service/src/classes/base/query.builder.ts#L249)
