# Friends

This API allows you to get information about your friends

## Request Method 
GET

## Endpoint
https://api.vrchat.cloud/api/1/auth/user/friends

## Requires Authentication
Yes

## Parameters

Field | Type | Optional | Description
------|------|----------|------------
offset | int | Yes | from where
n | int | Yes | How many
offline | boolean | Yes | Should return online friends

## Returns 
array of users

Field | Type | Description
------|------|------------
id | string | the user id
username | string | the login name
displayName | string | the display name
currentAvatarImageUrl | string | url to the avatar preview
currentAvatarThumbnailImageUrl | string | url to the avatar thumbnail
tags | array of `Permission` | The permissions the user has. 
developerType | `DeveloperType` | the user type
location | string | World Id With Instance Number and extra stuff at the end