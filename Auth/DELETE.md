# Logout

Used to delete an auth.

**URL** : `/api/auth/`

**Method** : `DELETE`

**Auth required** : YES

## Success Response

**Code** : `204 No Content`

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
