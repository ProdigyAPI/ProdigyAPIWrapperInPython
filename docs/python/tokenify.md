# Tokenify

Tokenify is a tool for getting your jwt token and other info.

## Examples

Here is an example:
```py
from prodigy import tokenify

print(f"Your jwt token is {tokenify('username', 'password')['token']}!")
```

## Parameters

Tokenify requires two parameters.
Being username and password.

Each of these should be strings.

There are no keywords.

Tokenify does not accept log.

## Output

Tokenify output's a dictionary following this schema:
```json
{
    "$schema": "http://json-schema.org/schema#",
    "type": "object",
    "properties": {
        "objectID": {
            "type": "integer"
        },
        "curriculumOverride": {
            "type": "null"
        },
        "curriculumTreeID": {
            "type": "string"
        },
        "lastVisited": {
            "type": "string"
        },
        "registerDate": {
            "type": "string"
        },
        "classIDs": {
            "type": "array"
        },
        "ownerIDs": {
            "type": "array"
        },
        "primaryParentID": {
            "type": "null"
        },
        "isTowerTownEnabled": {
            "type": "boolean"
        },
        "placementTestID": {
            "type": "null"
        },
        "goalId": {
            "type": "null"
        },
        "gradeId": {
            "type": "string"
        },
        "grade": {
            "type": "integer"
        },
        "userID": {
            "type": "integer"
        },
        "usertype": {
            "type": "string"
        },
        "authToken": {
            "type": "string"
        },
        "name": {
            "type": "string"
        },
        "token": {
            "type": "string"
        }
    },
    "required": [
        "authToken",
        "classIDs",
        "curriculumOverride",
        "curriculumTreeID",
        "goalId",
        "grade",
        "gradeId",
        "isTowerTownEnabled",
        "lastVisited",
        "name",
        "objectID",
        "ownerIDs",
        "placementTestID",
        "primaryParentID",
        "registerDate",
        "token",
        "userID",
        "usertype"
    ]
}
```

