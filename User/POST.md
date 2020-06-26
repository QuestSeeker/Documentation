# Create User

**URL** : `/api/user/`

**Method** : `POST`

**Auth required** : NO

**Permissions required** : None

**Data constraints**

```json
{
    "username": "[1 to 30 chars]",
    "email": "[valid email address]",
    "password": "[password in plain text]"
}
```

## Success Responses

**Condition** : Data provided is valid and User is created.

**Code** : `200 OK`

```json
{
    "id": 1234,
    "username" "JohnDoe"
    "email": "joe25@example.com"
}
```

## Error Response

**Condition** : If provided data is invalid, e.g. a name field is too long.

**Code** : `400 BAD REQUEST`

**Content example** :

```json
{
    "username": [
        "Please provide maximum 30 character",
    ],
    "email": [
        "Please provide valid email",
    ],
    "password": [
        "Please provide maximum 30 character",
    ]
}
```
