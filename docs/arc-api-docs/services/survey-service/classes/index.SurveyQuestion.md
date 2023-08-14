[@sourceloop/survey-service](../README.md) / [Modules](../modules.md) / [index](../modules/index.md) / SurveyQuestion

# Class: SurveyQuestion<T\>

[index](../modules/index.md).SurveyQuestion

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `DataObject`<`Model`\> |

## Hierarchy

- `UserModifiableEntity`<`T` & [`SurveyQuestion`](index.SurveyQuestion.md)\>

  ↳ **`SurveyQuestion`**

  ↳↳ [`SurveyQuestionDto`](index.SurveyQuestionDto.md)

## Table of contents

### Constructors

- [constructor](index.SurveyQuestion.md#constructor)

### Properties

- [createdBy](index.SurveyQuestion.md#createdby)
- [createdByUser](index.SurveyQuestion.md#createdbyuser)
- [createdOn](index.SurveyQuestion.md#createdon)
- [dependentOnQuestionId](index.SurveyQuestion.md#dependentonquestionid)
- [displayOrder](index.SurveyQuestion.md#displayorder)
- [extId](index.SurveyQuestion.md#extid)
- [extMetadata](index.SurveyQuestion.md#extmetadata)
- [id](index.SurveyQuestion.md#id)
- [isMandatory](index.SurveyQuestion.md#ismandatory)
- [modifiedBy](index.SurveyQuestion.md#modifiedby)
- [modifiedByUser](index.SurveyQuestion.md#modifiedbyuser)
- [modifiedOn](index.SurveyQuestion.md#modifiedon)
- [questionId](index.SurveyQuestion.md#questionid)
- [sectionId](index.SurveyQuestion.md#sectionid)
- [surveyId](index.SurveyQuestion.md#surveyid)
- [weight](index.SurveyQuestion.md#weight)

## Constructors

### constructor

• **new SurveyQuestion**<`T`\>(`data?`)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `DataObject`<`Model`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `data?` | `Partial`<`T` & [`SurveyQuestion`](index.SurveyQuestion.md)<`DataObject`<`Model`\>\>\> |

#### Inherited from

UserModifiableEntity<
  T & SurveyQuestion
\>.constructor

#### Defined in

packages/core/dist/models/base-entity.model.d.ts:6

## Properties

### createdBy

• `Optional` **createdBy**: `string`

#### Inherited from

UserModifiableEntity.createdBy

#### Defined in

packages/core/dist/models/user-modifiable-entity.model.d.ts:4

___

### createdByUser

• `Optional` **createdByUser**: `string`

#### Defined in

[services/survey-service/src/models/survey-question.model.ts:64](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/survey-service/src/models/survey-question.model.ts#L64)

___

### createdOn

• `Optional` **createdOn**: `Date`

#### Inherited from

UserModifiableEntity.createdOn

#### Defined in

packages/core/dist/models/base-entity.model.d.ts:4

___

### dependentOnQuestionId

• `Optional` **dependentOnQuestionId**: `string`

#### Defined in

[services/survey-service/src/models/survey-question.model.ts:53](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/survey-service/src/models/survey-question.model.ts#L53)

___

### displayOrder

• **displayOrder**: `number`

#### Defined in

[services/survey-service/src/models/survey-question.model.ts:30](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/survey-service/src/models/survey-question.model.ts#L30)

___

### extId

• `Optional` **extId**: `string`

#### Defined in

[services/survey-service/src/models/survey-question.model.ts:113](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/survey-service/src/models/survey-question.model.ts#L113)

___

### extMetadata

• `Optional` **extMetadata**: `AnyObject`

#### Defined in

[services/survey-service/src/models/survey-question.model.ts:119](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/survey-service/src/models/survey-question.model.ts#L119)

___

### id

• `Optional` **id**: `string`

#### Defined in

[services/survey-service/src/models/survey-question.model.ts:23](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/survey-service/src/models/survey-question.model.ts#L23)

___

### isMandatory

• **isMandatory**: `boolean`

#### Defined in

[services/survey-service/src/models/survey-question.model.ts:37](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/survey-service/src/models/survey-question.model.ts#L37)

___

### modifiedBy

• `Optional` **modifiedBy**: `string`

#### Inherited from

UserModifiableEntity.modifiedBy

#### Defined in

packages/core/dist/models/user-modifiable-entity.model.d.ts:5

___

### modifiedByUser

• `Optional` **modifiedByUser**: `string`

#### Defined in

[services/survey-service/src/models/survey-question.model.ts:66](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/survey-service/src/models/survey-question.model.ts#L66)

___

### modifiedOn

• `Optional` **modifiedOn**: `Date`

#### Inherited from

UserModifiableEntity.modifiedOn

#### Defined in

packages/core/dist/models/base-entity.model.d.ts:5

___

### questionId

• **questionId**: `string`

#### Defined in

[services/survey-service/src/models/survey-question.model.ts:92](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/survey-service/src/models/survey-question.model.ts#L92)

___

### sectionId

• `Optional` **sectionId**: `string`

#### Defined in

[services/survey-service/src/models/survey-question.model.ts:107](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/survey-service/src/models/survey-question.model.ts#L107)

___

### surveyId

• **surveyId**: `string`

#### Defined in

[services/survey-service/src/models/survey-question.model.ts:79](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/survey-service/src/models/survey-question.model.ts#L79)

___

### weight

• `Optional` **weight**: `number`

#### Defined in

[services/survey-service/src/models/survey-question.model.ts:62](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/d35fdb3f0/services/survey-service/src/models/survey-question.model.ts#L62)
