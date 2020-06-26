# Change password

Send a link to change password in Email.

**URL** : `/api/auth/change-password`

**Method** : `POST`

**Auth required** : NO

**Data constraints**

```json
{
    "email": "[valid email address]"
}
```

**Data example**

```json
{
    "email": "iloveauth@example.com"
}
```

## Success Response

**Code** : `204 No Content`

## Error Response

**Condition** : If 'email' is wrong.

**Code** : `400 BAD REQUEST`

**Content** :

```json
{
    "non_field_errors": [
        "Unable to find email."
    ]
}
```
