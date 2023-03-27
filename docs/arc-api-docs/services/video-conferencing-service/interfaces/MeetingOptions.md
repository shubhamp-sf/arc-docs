[@sourceloop/video-conferencing-service](../README.md) / [Exports](../modules.md) / MeetingOptions

# Interface: MeetingOptions

**`Interface`**

MeetingOptions

**`Param`**

optional parameter to enable/disable recordings. Default will be false

**`Param`**

parameter to check whether a meeting is booked now if

**`Param`**

or scheduled at a later time if

**`Param`**

**`Param`**

not required if

**`Param`**

is false,
 else set a later time for scheduling meeting

## Hierarchy

- **`MeetingOptions`**

  ↳ [`VonageMeetingOptions`](VonageMeetingOptions.md)

  ↳ [`TwilioMeetingOptions`](TwilioMeetingOptions.md)

## Table of contents

### Properties

- [isScheduled](MeetingOptions.md#isscheduled)
- [scheduleTime](MeetingOptions.md#scheduletime)

## Properties

### isScheduled

• **isScheduled**: `boolean`

#### Defined in

[services/video-conferencing-service/src/types.ts:149](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/a84fe677/services/video-conferencing-service/src/types.ts#L149)

___

### scheduleTime

• `Optional` **scheduleTime**: `Date`

#### Defined in

[services/video-conferencing-service/src/types.ts:150](https://github.com/sourcefuse/loopback4-microservice-catalog/blob/a84fe677/services/video-conferencing-service/src/types.ts#L150)
