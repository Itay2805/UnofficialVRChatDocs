# Search

This API allows you to list users and use some filters to filter them.

## Request Method
GET

## Endpoint
https://api.vrchat.cloud/api/1/users

## Requires Authentication
Yes (See [here](/GettingStarted/QuickStart?id=authorization) for details)

# Parameter

Field | Type | Optional | Description
------|------|----------|------------
search | string | no | Username to search for
developerType | `DeveloperType` | yes | Active user by developer type, `none` for normal users and `internal` for moderators
n | int | yes | How many users to return
offset | int | yes | How many users to skip

## Returns

Array of [`Limited User objects`](/Objects/User.md#limited-user-object)
