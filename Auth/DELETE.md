# Logout

Used to delete an auth.

**URL** : `/api/auth/`

**Method** : `DELETE`

**Auth required** : YES

## Success Response

**Code** : `204 No Content`

**Content example**

```json
{
    "token": "93144b288eb1fdccbe46d6fc0f241a51766ecd3d"
}
```

## Error Response

**Condition** : If 'username' and 'password' combination is wrong.

**Code** : `400 BAD REQUEST`

**Content** :

```json
{
    "non_field_errors": [
        "Unable to logout with provided token."
    ]
}
```
