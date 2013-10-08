---
title: Cluestr frontend endpoint
subtitle: Search and retrieve.
layout: doc
---

### Home
* **Path**: `/`
* **HTTP-Verb** : `GET`

#### Description
This endpoint returns data about the currently logged in user's company.


#### Example
curl -H "Authorization: token ${TOKEN}" http://api.cluestr.com


#### Response
```json
{
    "_type": "Company",
    "id": "5252cebb03a470843f000002",
    "name": "matthieu@papiel.fr",
    "users_url": "/users",
    "user_url": "/user",
    "documents_url": "/documents",
    "document_types_url": "/document-types",
    "provider_status": {
        "9d6e862308f3377c8b5fac707c9dfff75ec3f640c4cd0e9c7688709ce69f3505": "2013-10-07T17:14:40.002Z"
    }
}
```

You will find here URLs to most services (all the `_url` keys).

`provider_status` contains information about all the providers connected on this account and the date they sent datas for the last time.

> We recommend sending a `/update` right after retrieving this URL, to ensure all datas are up to date.

Possible error codes: N/A.

### Home
* **Path**: `/`
* **HTTP-Verb** : `GET`

#### Description
This endpoint returns data about the currently logged in user's company.


#### Example
curl -H "Authorization: token ${TOKEN}" http://api.cluestr.com


#### Response
```json
{
    "_type": "Company",
    "id": "5252cebb03a470843f000002",
    "name": "matthieu@papiel.fr",
    "users_url": "/users",
    "user_url": "/user",
    "documents_url": "/documents",
    "document_types_url": "/document-types",
    "provider_status": {
        "9d6e862308f3377c8b5fac707c9dfff75ec3f640c4cd0e9c7688709ce69f3505": "2013-10-07T17:14:40.002Z"
    }
}
```

You will find here URLs to most services (all the `_url` keys).

`provider_status` contains information about all the providers connected on this account and the date they sent datas for the last time.

> We recommend sending a `/update` right after retrieving this URL, to ensure all datas are up to date.

Possible error codes: N/A.