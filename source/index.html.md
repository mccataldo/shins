---
title: ObservePoint API
language_tabs:
  - shell: Shell
  - http: HTTP
  - html: JavaScript
  - javascript: Node.JS
  - python: Python
  - ruby: Ruby
  - java: Java
toc_footers: []
includes: []
search: true
highlight_theme: darkula
---

# ObservePoint API



Base URL = https://app.observepoint.com/api/v2





# Account

## GET_account

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/account
````

````http
GET https://app.observepoint.com/api/v2/account HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/account',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/account', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/account', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/account', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/account");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /account`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
Total-Route-Time|header|integer|false|No description
Connect-Time|header|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "simulationsUsed": 0,
    "name": "string",
    "appsUsed": 0,
    "maxSimulations": 0,
    "maxUsers": 0,
    "strongPasswordPolicy": true,
    "urlsUsed": 0,
    "id": 0,
    "usersUsed": 0,
    "accountType": 0,
    "auditsUsed": 0,
    "maxAudits": 0,
    "maxApps": 0,
    "appTestsUsed": 0
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_locations

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/account/locations
````

````http
GET https://app.observepoint.com/api/v2/account/locations HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/account/locations',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/account/locations', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/account/locations', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/account/locations', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/account/locations");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /account/locations`

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {
      "name": "string",
      "label": "string"
    }
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_frequencies-audits

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/account/frequencies/audits
````

````http
GET https://app.observepoint.com/api/v2/account/frequencies/audits HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/account/frequencies/audits',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/account/frequencies/audits', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/account/frequencies/audits', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/account/frequencies/audits', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/account/frequencies/audits");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /account/frequencies/audits`

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    "string"
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_account-user-agents

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/account/user-agents
````

````http
GET https://app.observepoint.com/api/v2/account/user-agents HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/account/user-agents',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/account/user-agents', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/account/user-agents', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/account/user-agents', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/account/user-agents");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /account/user-agents`

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
[
  {
    "name": "string",
    "label": "string"
  }
]
````
<aside class="success">
This operation does not require authentication
</aside>

# Users

## GET_users

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/users
````

````http
GET https://app.observepoint.com/api/v2/users HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/users',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/users', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/users', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/users', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/users");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /users`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
Connect-Time|header|integer|false|No description
Total-Route-Time|header|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {
      "lastLogin": "string",
      "email": "string",
      "username": "string",
      "timezone": "string",
      "permissions": "string",
      "accountId": 0,
      "lastName": "string",
      "firstName": "string",
      "id": 0,
      "updated": "string",
      "created": "string"
    }
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_users

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/users
````

````http
POST https://app.observepoint.com/api/v2/users HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/users',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/users', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/users', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/users', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/users");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /users`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
body|body|object|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

> Body parameter

````json
{
  "timezone": "America/Denver",
  "firstName": "user",
  "lastName": "1",
  "username": "user1",
  "email": "mike.cataldo@observepoint.com",
  "permissions": "user"
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "email": {
          "type": "string"
        },
        "username": {
          "type": "string"
        },
        "timezone": {
          "type": "string"
        },
        "permissions": {
          "type": "string"
        },
        "accountId": {
          "type": "integer"
        },
        "lastName": {
          "type": "string"
        },
        "firstName": {
          "type": "string"
        },
        "id": {
          "type": "integer"
        },
        "updated": {
          "type": "string"
        },
        "created": {
          "type": "string"
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_users-param1

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/users/{param1}
````

````http
GET https://app.observepoint.com/api/v2/users/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/users/{param1}',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/users/{param1}', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/users/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/users/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/users/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /users/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
Total-Route-Time|header|integer|false|No description
Connect-Time|header|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "lastLogin": "string",
    "email": "string",
    "username": "string",
    "timezone": "string",
    "permissions": "string",
    "accountId": 0,
    "lastName": "string",
    "firstName": "string",
    "id": 0,
    "updated": "string",
    "created": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## PUT_users-param1

> Code samples

````shell
# You can also use wget
curl -X put https://app.observepoint.com/api/v2/users/{param1}
````

````http
PUT https://app.observepoint.com/api/v2/users/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/users/{param1}',
    method: 'put',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/users/{param1}', { method: 'PUT'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.put 'https://app.observepoint.com/api/v2/users/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.put('https://app.observepoint.com/api/v2/users/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/users/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("PUT");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`PUT /users/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
body|body|object|false|No description
Content-Type|header|string|false|No description
Authorization|header|string|false|No description

> Body parameter

````json
{
  "lastLogin": "2016-11-17T16:34:55.000-07:00",
  "email": "MIKE.CATALDO@OBSERVEPOINT.COM",
  "username": "starwoodadmin",
  "timezone": "America/Denver",
  "permissions": "admin",
  "accountId": 19,
  "lastName": "cataldo",
  "firstName": "mike",
  "id": 26,
  "updated": "2016-11-01T12:50:52.000-06:00",
  "created": "2016-11-01T12:50:52.000-06:00"
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "lastLogin": "string",
    "email": "string",
    "username": "string",
    "timezone": "string",
    "permissions": "string",
    "accountId": 0,
    "lastName": "string",
    "firstName": "string",
    "id": 0,
    "updated": "string",
    "created": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## DELETE_users-param1

> Code samples

````shell
# You can also use wget
curl -X delete https://app.observepoint.com/api/v2/users/{param1}
````

````http
DELETE https://app.observepoint.com/api/v2/users/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/users/{param1}',
    method: 'delete',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/users/{param1}', { method: 'DELETE'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.delete 'https://app.observepoint.com/api/v2/users/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.delete('https://app.observepoint.com/api/v2/users/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/users/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("DELETE");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`DELETE /users/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
Authorization|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_users-param1-folders

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/users/{param1}/folders
````

````http
GET https://app.observepoint.com/api/v2/users/{param1}/folders HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/users/{param1}/folders',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/users/{param1}/folders', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/users/{param1}/folders', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/users/{param1}/folders', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/users/{param1}/folders");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /users/{param1}/folders`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
Authorization|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {
      "id": 0,
      "name": "string",
      "accountId": 0
    }
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_users-param1-folders

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/users/{param1}/folders
````

````http
POST https://app.observepoint.com/api/v2/users/{param1}/folders HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/users/{param1}/folders',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/users/{param1}/folders', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/users/{param1}/folders', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/users/{param1}/folders', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/users/{param1}/folders");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /users/{param1}/folders`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
body|body|object|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

> Body parameter

````json
[
  83
]
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {
      "id": 0,
      "name": "string",
      "accountId": 0
    }
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

# Apps

## GET_apps-param1-appetize-key

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/apps/{param1}/appetize-key
````

````http
GET https://app.observepoint.com/api/v2/apps/{param1}/appetize-key HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/apps/{param1}/appetize-key',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/apps/{param1}/appetize-key', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/apps/{param1}/appetize-key', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/apps/{param1}/appetize-key', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/apps/{param1}/appetize-key");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /apps/{param1}/appetize-key`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
Authorization|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "key": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_apps-count

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/apps/count
````

````http
GET https://app.observepoint.com/api/v2/apps/count HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/apps/count',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/apps/count', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/apps/count', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/apps/count', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/apps/count");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /apps/count`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
Authorization|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "count": 0
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## DELETE_apps-param1

> Code samples

````shell
# You can also use wget
curl -X delete https://app.observepoint.com/api/v2/apps/{param1}
````

````http
DELETE https://app.observepoint.com/api/v2/apps/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/apps/{param1}',
    method: 'delete',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/apps/{param1}', { method: 'DELETE'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.delete 'https://app.observepoint.com/api/v2/apps/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.delete('https://app.observepoint.com/api/v2/apps/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/apps/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("DELETE");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`DELETE /apps/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|No description

> Example responses

````json
{}
````
<aside class="success">
This operation does not require authentication
</aside>

## PUT_apps-param1

> Code samples

````shell
# You can also use wget
curl -X put https://app.observepoint.com/api/v2/apps/{param1}
````

````http
PUT https://app.observepoint.com/api/v2/apps/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/apps/{param1}',
    method: 'put',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/apps/{param1}', { method: 'PUT'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.put 'https://app.observepoint.com/api/v2/apps/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.put('https://app.observepoint.com/api/v2/apps/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/apps/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("PUT");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`PUT /apps/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
body|body|object|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

> Body parameter

````json
{
  "id": 178,
  "name": "testing stoplight1",
  "folderId": 531,
  "platform": 1,
  "file": "SPGAndroid-develop-1716 (1).apk",
  "recipients": [
    "mike.cataldo@observepoint.com",
    "mike.cataldo@blaskjgjrigndnfkvgijrvf.com"
  ]
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "uploadId": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_apps

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/apps
````

````http
GET https://app.observepoint.com/api/v2/apps HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/apps',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/apps', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/apps', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/apps', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/apps");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /apps`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
folderId|query|integer|false|No description
Authorization|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {}
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_apps

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/apps
````

````http
POST https://app.observepoint.com/api/v2/apps HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/apps',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/apps', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/apps', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/apps', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/apps");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /apps`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
body|body|object|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

> Body parameter

````json
{
  "name": "testing stoplight",
  "file": "SPGAndroid-develop-1716 (1).apk",
  "platform": 1,
  "folderId": 531,
  "recipients": [
    "mike.cataldo@observepoint.com",
    "mike.cataldo@blaskjgjrigndnfkvgijrvf.com"
  ]
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "uploadId": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_apps-param1-suites

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/apps/{param1}/suites
````

````http
GET https://app.observepoint.com/api/v2/apps/{param1}/suites HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/apps/{param1}/suites',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/apps/{param1}/suites', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/apps/{param1}/suites', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/apps/{param1}/suites', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/apps/{param1}/suites");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /apps/{param1}/suites`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
Authorization|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {}
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

# Audits

## GET_audits

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/web-audits
````

````http
GET https://app.observepoint.com/api/v2/web-audits HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-audits',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-audits', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/web-audits', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/web-audits', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-audits");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /web-audits`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
Total-Route-Time|header|integer|false|No description
Connect-Time|header|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {}
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_audits

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/web-audits
````

````http
POST https://app.observepoint.com/api/v2/web-audits HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-audits',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-audits', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/web-audits', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/web-audits', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-audits");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /web-audits`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
body|body|object|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

> Body parameter

````json
{
  "domainId": 280,
  "name": "testing stoplight",
  "limit": 100,
  "startingUrls": [
    "http://stoplight.io",
    "http://stoplight.io/cart"
  ],
  "frequency": "weekly",
  "recipients": [
    "MIKE.CATALDO@OBSERVEPOINT.COM",
    "mightymouse@sdlkjdfrtdfesdf.com"
  ],
  "nextRun": "2016-11-18T06:46:23.126Z",
  "filters": {
    "include": [
      "^https?://([^/:\\?]*\\.)?stoplight.io"
    ],
    "exclude": [
      "^https?://([^/:\\?]*\\.)?stoplightt.io"
    ]
  },
  "options": {
    "location": "mountain",
    "userAgent": "Firefox(45.0.1) - Linux",
    "requestRate": 10,
    "fireTags": false,
    "clearCookies": false,
    "stripQueryString": false,
    "loadFlash": true,
    "browserWidth": 1366
  }
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "name": {
          "type": "string"
        },
        "startingUrls": {
          "type": "array",
          "items": {
            "type": "string"
          }
        },
        "lastUpdated": {
          "type": "string"
        },
        "nextRun": {
          "type": "string"
        },
        "recipients": {
          "type": "array",
          "items": {
            "type": "string"
          }
        },
        "folderId": {
          "type": "integer"
        },
        "options": {
          "type": "object",
          "properties": {
            "location": {
              "type": "string"
            },
            "stripQueryString": {
              "type": "boolean"
            },
            "browserWidth": {
              "type": "integer"
            },
            "userAgent": {
              "type": "string"
            },
            "fireTags": {
              "type": "boolean"
            },
            "loadFlash": {
              "type": "boolean"
            },
            "requestRate": {
              "type": "integer"
            },
            "clearCookies": {
              "type": "boolean"
            }
          }
        },
        "id": {
          "type": "integer"
        },
        "filters": {
          "type": "object",
          "properties": {
            "include": {
              "type": "array",
              "items": {
                "type": "string"
              }
            },
            "exclude": {
              "type": "array",
              "items": {
                "type": "string"
              }
            }
          }
        },
        "ownerId": {
          "type": "integer"
        },
        "domainId": {
          "type": "integer"
        },
        "frequency": {
          "type": "string"
        },
        "limit": {
          "type": "integer"
        },
        "created": {
          "type": "string"
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_audits-param1

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/web-audits/{param1}
````

````http
GET https://app.observepoint.com/api/v2/web-audits/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-audits/{param1}',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-audits/{param1}', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/web-audits/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/web-audits/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-audits/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /web-audits/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
Authorization|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "name": {
          "type": "string"
        },
        "startingUrls": {
          "type": "array",
          "items": {
            "type": "string"
          }
        },
        "lastUpdated": {
          "type": "string"
        },
        "nextRun": {
          "type": "string"
        },
        "recipients": {
          "type": "array",
          "items": {
            "type": "string"
          }
        },
        "folderId": {
          "type": "integer"
        },
        "ruleSets": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "name": {
                "type": "string"
              },
              "updatedAt": {
                "type": "string"
              },
              "recipients": {
                "type": "array",
                "items": {
                  "type": "object",
                  "properties": {}
                }
              },
              "accountId": {
                "type": "integer"
              },
              "id": {
                "type": "integer"
              },
              "createdAt": {
                "type": "string"
              }
            }
          }
        },
        "options": {
          "type": "object",
          "properties": {
            "location": {
              "type": "string"
            },
            "stripQueryString": {
              "type": "boolean"
            },
            "browserWidth": {
              "type": "integer"
            },
            "userAgent": {
              "type": "string"
            },
            "fireTags": {
              "type": "boolean"
            },
            "loadFlash": {
              "type": "boolean"
            },
            "requestRate": {
              "type": "integer"
            },
            "clearCookies": {
              "type": "boolean"
            }
          }
        },
        "id": {
          "type": "integer"
        },
        "filters": {
          "type": "object",
          "properties": {
            "include": {
              "type": "array",
              "items": {
                "type": "string"
              }
            },
            "exclude": {
              "type": "array",
              "items": {
                "type": "string"
              }
            }
          }
        },
        "ownerId": {
          "type": "integer"
        },
        "domainId": {
          "type": "integer"
        },
        "frequency": {
          "type": "string"
        },
        "limit": {
          "type": "integer"
        },
        "created": {
          "type": "string"
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## PUT_audits-param1

> Code samples

````shell
# You can also use wget
curl -X put https://app.observepoint.com/api/v2/web-audits/{param1}
````

````http
PUT https://app.observepoint.com/api/v2/web-audits/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-audits/{param1}',
    method: 'put',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-audits/{param1}', { method: 'PUT'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.put 'https://app.observepoint.com/api/v2/web-audits/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.put('https://app.observepoint.com/api/v2/web-audits/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-audits/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("PUT");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`PUT /web-audits/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
body|body|object|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

> Body parameter

````json
{
  "name": "testing stoplight copied 17 November 2016, 11:46:34pm",
  "startingUrls": [
    "http://stoplight.io",
    "http://stoplight.io/cart"
  ],
  "lastUpdated": "2016-11-18T06:46:13.000Z",
  "nextRun": "2016-11-18T06:46:37.522Z",
  "recipients": [
    "MIKE.CATALDO@OBSERVEPOINT.COM",
    "mightymouse@sdlkjdfrtdfesdf.com"
  ],
  "lastRun": null,
  "folderId": 531,
  "ruleSets": [
    {
      "name": "Bing (with Tag Matching)",
      "updatedAt": "2016-11-02T19:41:34.000Z",
      "recipients": [],
      "accountId": 19,
      "id": 13,
      "createdAt": "2016-11-02T19:41:34.000Z",
      "rules": null
    }
  ],
  "options": {
    "location": "mountain",
    "stripQueryString": false,
    "browserWidth": 1366,
    "userAgent": "Firefox(45.0.1) - Linux",
    "fireTags": true,
    "loadFlash": true,
    "requestRate": 10,
    "clearCookies": false
  },
  "id": 120,
  "filters": {
    "include": [
      "^https?://([^/:\\?]*\\.)?stoplight.io"
    ],
    "exclude": [
      "^https?://([^/:\\?]*\\.)?stoplightt.io"
    ]
  },
  "screenshot": null,
  "ownerId": 26,
  "domainId": 280,
  "frequency": "weekly",
  "auditRunning": null,
  "limit": 100,
  "created": "2016-11-18T06:46:13.000Z",
  "actions": []
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "name": {
          "type": "string"
        },
        "startingUrls": {
          "type": "array",
          "items": {
            "type": "string"
          }
        },
        "lastUpdated": {
          "type": "string"
        },
        "nextRun": {
          "type": "string"
        },
        "recipients": {
          "type": "array",
          "items": {
            "type": "string"
          }
        },
        "folderId": {
          "type": "integer"
        },
        "ruleSets": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "name": {
                "type": "string"
              },
              "updatedAt": {
                "type": "string"
              },
              "recipients": {
                "type": "array",
                "items": {
                  "type": "object",
                  "properties": {}
                }
              },
              "accountId": {
                "type": "integer"
              },
              "id": {
                "type": "integer"
              },
              "createdAt": {
                "type": "string"
              }
            }
          }
        },
        "options": {
          "type": "object",
          "properties": {
            "location": {
              "type": "string"
            },
            "stripQueryString": {
              "type": "boolean"
            },
            "browserWidth": {
              "type": "integer"
            },
            "userAgent": {
              "type": "string"
            },
            "fireTags": {
              "type": "boolean"
            },
            "loadFlash": {
              "type": "boolean"
            },
            "requestRate": {
              "type": "integer"
            },
            "clearCookies": {
              "type": "boolean"
            }
          }
        },
        "id": {
          "type": "integer"
        },
        "filters": {
          "type": "object",
          "properties": {
            "include": {
              "type": "array",
              "items": {
                "type": "string"
              }
            },
            "exclude": {
              "type": "array",
              "items": {
                "type": "string"
              }
            }
          }
        },
        "ownerId": {
          "type": "integer"
        },
        "domainId": {
          "type": "integer"
        },
        "frequency": {
          "type": "string"
        },
        "limit": {
          "type": "integer"
        },
        "created": {
          "type": "string"
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_audits-NaN-runs

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/audits/NaN/runs
````

````http
GET https://app.observepoint.com/api/v2/audits/NaN/runs HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/audits/NaN/runs',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/audits/NaN/runs', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/audits/NaN/runs', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/audits/NaN/runs', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/audits/NaN/runs");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /audits/NaN/runs`

### Responses

Status|Meaning|Description
---|---|---|
404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|No description

> Example responses

````json
{}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_audits-param1-runs

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/web-audits/{param1}/runs
````

````http
GET https://app.observepoint.com/api/v2/web-audits/{param1}/runs HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-audits/{param1}/runs',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-audits/{param1}/runs', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/web-audits/{param1}/runs', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/web-audits/{param1}/runs', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-audits/{param1}/runs");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /web-audits/{param1}/runs`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
Authorization|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "array",
      "items": {
        "type": "object",
        "properties": {
          "auditId": {
            "type": "integer"
          },
          "score": {
            "type": "integer"
          },
          "totalUrl": {
            "type": "integer"
          },
          "silentMode": {
            "type": "boolean"
          },
          "id": {
            "type": "integer"
          },
          "taggedUrl": {
            "type": "integer"
          },
          "userId": {
            "type": "integer"
          },
          "started": {
            "type": "string"
          },
          "limit": {
            "type": "integer"
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_audits-param1-login-actions

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/web-audits/{param1}/login-actions
````

````http
GET https://app.observepoint.com/api/v2/web-audits/{param1}/login-actions HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-audits/{param1}/login-actions',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-audits/{param1}/login-actions', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/web-audits/{param1}/login-actions', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/web-audits/{param1}/login-actions', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-audits/{param1}/login-actions");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /web-audits/{param1}/login-actions`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
Authorization|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|No description
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{}
````
````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## PUT_audits-param1-filters

> Code samples

````shell
# You can also use wget
curl -X put https://app.observepoint.com/api/v2/web-audits/{param1}/filters
````

````http
PUT https://app.observepoint.com/api/v2/web-audits/{param1}/filters HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-audits/{param1}/filters',
    method: 'put',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-audits/{param1}/filters', { method: 'PUT'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.put 'https://app.observepoint.com/api/v2/web-audits/{param1}/filters', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.put('https://app.observepoint.com/api/v2/web-audits/{param1}/filters', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-audits/{param1}/filters");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("PUT");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`PUT /web-audits/{param1}/filters`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
body|body|object|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

> Body parameter

````json
{
  "include": [
    "^https?://([^/:\\?]*\\.)?stoplight.io"
  ],
  "exclude": [
    "^https?://([^/:\\?]*\\.)?stoplightt.io"
  ]
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "include": [
      "string"
    ],
    "exclude": [
      "string"
    ]
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## PUT_audits-param1-login-actions

> Code samples

````shell
# You can also use wget
curl -X put https://app.observepoint.com/api/v2/audits/{param1}/login-actions
````

````http
PUT https://app.observepoint.com/api/v2/audits/{param1}/login-actions HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/audits/{param1}/login-actions',
    method: 'put',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/audits/{param1}/login-actions', { method: 'PUT'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.put 'https://app.observepoint.com/api/v2/audits/{param1}/login-actions', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.put('https://app.observepoint.com/api/v2/audits/{param1}/login-actions', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/audits/{param1}/login-actions");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("PUT");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`PUT /audits/{param1}/login-actions`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
body|body|object|false|No description
Content-Type|header|string|false|No description
Authorization|header|string|false|No description

> Body parameter

````json
{
  "url": "http://stoplight.io",
  "actions": [
    {
      "type": "click",
      "preventNavigation": true,
      "sequence": 0,
      "identifier": "id",
      "action": "click",
      "rules": []
    },
    {
      "type": "input",
      "preventNavigation": true,
      "sequence": 1,
      "value": "dsf",
      "identifier": "dsf",
      "action": "input",
      "rules": []
    },
    {
      "type": "maskedInput",
      "preventNavigation": false,
      "sequence": 2,
      "maskedValue": "34",
      "maskedInputType": "text",
      "viewedValue": "34",
      "isChangedValue": true,
      "identifier": "dsf",
      "action": "maskedInput",
      "rules": []
    },
    {
      "type": "select",
      "preventNavigation": false,
      "sequence": 3,
      "value": "sdfg",
      "identifier": "adf",
      "action": "select",
      "rules": []
    },
    {
      "type": "check",
      "preventNavigation": false,
      "sequence": 4,
      "identifier": "sdf",
      "action": "check",
      "rules": []
    },
    {
      "type": "uncheck",
      "preventNavigation": false,
      "sequence": 5,
      "identifier": "grh",
      "action": "uncheck",
      "rules": []
    },
    {
      "type": "execute",
      "preventNavigation": false,
      "sequence": 6,
      "js": "sdfgsfhnhtbt",
      "action": "execute",
      "rules": []
    },
    {
      "type": "watch",
      "preventNavigation": false,
      "sequence": 7,
      "seconds": 12,
      "action": "watch",
      "rules": []
    }
  ]
}
````
### Responses

Status|Meaning|Description
---|---|---|
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_audits-param1-actions

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/audits/{param1}/actions
````

````http
GET https://app.observepoint.com/api/v2/audits/{param1}/actions HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/audits/{param1}/actions',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/audits/{param1}/actions', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/audits/{param1}/actions', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/audits/{param1}/actions', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/audits/{param1}/actions");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /audits/{param1}/actions`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
Authorization|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {}
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## PUT_audits-param1-actions

> Code samples

````shell
# You can also use wget
curl -X put https://app.observepoint.com/api/v2/audits/{param1}/actions
````

````http
PUT https://app.observepoint.com/api/v2/audits/{param1}/actions HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/audits/{param1}/actions',
    method: 'put',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/audits/{param1}/actions', { method: 'PUT'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.put 'https://app.observepoint.com/api/v2/audits/{param1}/actions', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.put('https://app.observepoint.com/api/v2/audits/{param1}/actions', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/audits/{param1}/actions");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("PUT");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`PUT /audits/{param1}/actions`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
body|body|object|false|No description
Content-Type|header|string|false|No description
Authorization|header|string|false|No description

> Body parameter

````json
[
  {}
]
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {}
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_audits-param1-tag-summaries

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/audits/{param1}/tag-summaries
````

````http
GET https://app.observepoint.com/api/v2/audits/{param1}/tag-summaries HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/audits/{param1}/tag-summaries',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/audits/{param1}/tag-summaries', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/audits/{param1}/tag-summaries', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/audits/{param1}/tag-summaries', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/audits/{param1}/tag-summaries");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /audits/{param1}/tag-summaries`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
run_id|query|integer|false|No description
Authorization|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {}
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_audits-default-filters

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/audits/default-filters
````

````http
POST https://app.observepoint.com/api/v2/audits/default-filters HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/audits/default-filters',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/audits/default-filters', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/audits/default-filters', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/audits/default-filters', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/audits/default-filters");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /audits/default-filters`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
body|body|object|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

> Body parameter

````json
[
  "http://stoplight.io",
  "http://stoplight.io/cart"
]
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "include": [
      "string"
    ],
    "exclude": [
      {}
    ]
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## PUT_audits-param1-rule-sets

> Code samples

````shell
# You can also use wget
curl -X put https://app.observepoint.com/api/v2/audits/{param1}/rule-sets
````

````http
PUT https://app.observepoint.com/api/v2/audits/{param1}/rule-sets HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/audits/{param1}/rule-sets',
    method: 'put',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/audits/{param1}/rule-sets', { method: 'PUT'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.put 'https://app.observepoint.com/api/v2/audits/{param1}/rule-sets', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.put('https://app.observepoint.com/api/v2/audits/{param1}/rule-sets', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/audits/{param1}/rule-sets");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("PUT");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`PUT /audits/{param1}/rule-sets`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
body|body|object|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

> Body parameter

````json
[
  13
]
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "array",
      "items": {
        "type": "object",
        "properties": {
          "name": {
            "type": "string"
          },
          "updatedAt": {
            "type": "string"
          },
          "recipients": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {}
            }
          },
          "accountId": {
            "type": "integer"
          },
          "id": {
            "type": "integer"
          },
          "createdAt": {
            "type": "string"
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_audit-param1-reports-summary-run-param2

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/audits/{param1}/reports/summary/run/{param2}
````

````http
GET https://app.observepoint.com/api/v2/audits/{param1}/reports/summary/run/{param2} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: text/html
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/audits/{param1}/reports/summary/run/{param2}',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/audits/{param1}/reports/summary/run/{param2}', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/audits/{param1}/reports/summary/run/{param2}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/audits/{param1}/reports/summary/run/{param2}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/audits/{param1}/reports/summary/run/{param2}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /audits/{param1}/reports/summary/run/{param2}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|string|true|No description
param2|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{}
````
<aside class="success">
This operation does not require authentication
</aside>

# Domains

## GET_domains

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/domains
````

````http
GET https://app.observepoint.com/api/v2/domains HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/domains',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/domains', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/domains', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/domains', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/domains");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /domains`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
withTotals|query|boolean|false|No description
folderId|query|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {
      "name": "string",
      "guidedJourneys": 0,
      "domain": "string",
      "pages": 0,
      "folderId": 0,
      "errors": 0,
      "id": 0,
      "automatedJourneys": 0,
      "auditsRunning": 0,
      "averageScore": 0,
      "createdAt": "string",
      "userId": 0,
      "dataLayer": "string",
      "simulationsRunning": 0
    }
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_domains

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/domains
````

````http
POST https://app.observepoint.com/api/v2/domains HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/domains',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/domains', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/domains', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/domains', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/domains");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /domains`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
body|body|object|false|No description

> Body parameter

````json
{
  "folderId": 531,
  "name": "testingstoplightdomain",
  "domain": "http://stoplight.io",
  "dataLayer": "datalayrrrrr"
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "name": "string",
    "domain": "string",
    "folderId": 0,
    "id": 0,
    "createdAt": "string",
    "userId": 0,
    "dataLayer": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_domains-count

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/domains/count
````

````http
GET https://app.observepoint.com/api/v2/domains/count HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/domains/count',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/domains/count', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/domains/count', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/domains/count', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/domains/count");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /domains/count`

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "count": 0
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_domains-param1

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/domains/{param1}
````

````http
GET https://app.observepoint.com/api/v2/domains/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/domains/{param1}',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/domains/{param1}', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/domains/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/domains/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/domains/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /domains/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
withTotals|query|boolean|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "name": "string",
    "domain": "string",
    "folderId": 0,
    "id": 0,
    "createdAt": "string",
    "userId": 0,
    "dataLayer": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## PUT_domains-param1

> Code samples

````shell
# You can also use wget
curl -X put https://app.observepoint.com/api/v2/domains/{param1}
````

````http
PUT https://app.observepoint.com/api/v2/domains/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/domains/{param1}',
    method: 'put',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/domains/{param1}', { method: 'PUT'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.put 'https://app.observepoint.com/api/v2/domains/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.put('https://app.observepoint.com/api/v2/domains/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/domains/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("PUT");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`PUT /domains/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
body|body|object|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

> Body parameter

````json
{
  "name": "testingstoplightdomain1",
  "guidedJourneys": 0,
  "domain": "http://stoplight.io",
  "pages": 0,
  "folderId": 531,
  "errors": 0,
  "id": 280,
  "automatedJourneys": 0,
  "auditsRunning": 0,
  "averageScore": 0,
  "createdAt": "2016-11-17T23:36:30.000-07:00",
  "userId": 26,
  "dataLayer": "datalayrrrrr",
  "simulationsRunning": 0,
  "hover": false,
  "hoverMenu": false
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "name": "string",
    "domain": "string",
    "folderId": 0,
    "id": 0,
    "createdAt": "string",
    "userId": 0,
    "dataLayer": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## DELETE_domains-param1

> Code samples

````shell
# You can also use wget
curl -X delete https://app.observepoint.com/api/v2/domains/{param1}
````

````http
DELETE https://app.observepoint.com/api/v2/domains/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/domains/{param1}',
    method: 'delete',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/domains/{param1}', { method: 'DELETE'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.delete 'https://app.observepoint.com/api/v2/domains/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.delete('https://app.observepoint.com/api/v2/domains/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/domains/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("DELETE");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`DELETE /domains/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|No description

> Example responses

````json
{}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_domains-param1-automated

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/domains/{param1}/web-audits
````

````http
GET https://app.observepoint.com/api/v2/domains/{param1}/web-audits HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/domains/{param1}/web-audits',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/domains/{param1}/web-audits', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/domains/{param1}/web-audits', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/domains/{param1}/web-audits', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/domains/{param1}/web-audits");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /domains/{param1}/web-audits`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {}
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_domains-param1-guided

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/domains/{param1}/web-journeys
````

````http
GET https://app.observepoint.com/api/v2/domains/{param1}/web-journeys HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/domains/{param1}/web-journeys',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/domains/{param1}/web-journeys', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/domains/{param1}/web-journeys', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/domains/{param1}/web-journeys', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/domains/{param1}/web-journeys");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /domains/{param1}/web-journeys`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {}
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

# Events

## GET_events

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/events
````

````http
GET https://app.observepoint.com/api/v2/events HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/events',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/events', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/events', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/events', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/events");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /events`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
Connect-Time|header|integer|false|No description
Total-Route-Time|header|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {}
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

# Folders

## GET_folders

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/folders
````

````http
GET https://app.observepoint.com/api/v2/folders HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/folders',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/folders', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/folders', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/folders', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/folders");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /folders`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
Connect-Time|header|integer|false|No description
Total-Route-Time|header|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "data": [
    {
      "appsRunning": 0,
      "appsInQueue": 0,
      "name": "string",
      "appRuleFailures": 0,
      "createdByUserName": "string",
      "appsCount": 0,
      "accountId": 0,
      "createdByUserId": 0,
      "id": 0,
      "auditsRunning": 0,
      "createdAt": "string",
      "appFailures": 0,
      "simulationErrors": 0,
      "simulationsRunning": 0,
      "domainsCount": 0
    }
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_folders

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/folders
````

````http
POST https://app.observepoint.com/api/v2/folders HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/folders',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/folders', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/folders', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/folders', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/folders");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /folders`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
body|body|object|false|No description

> Body parameter

````json
{
  "accountId": 19,
  "name": "testingstoplight"
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "appsRunning": 0,
    "appsInQueue": 0,
    "name": "string",
    "appRuleFailures": 0,
    "createdByUserName": "string",
    "appsCount": 0,
    "accountId": 0,
    "createdByUserId": 0,
    "id": 0,
    "auditsRunning": 0,
    "createdAt": "string",
    "appFailures": 0,
    "simulationErrors": 0,
    "simulationsRunning": 0,
    "domainsCount": 0
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_folders-count

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/folders/count
````

````http
GET https://app.observepoint.com/api/v2/folders/count HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/folders/count',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/folders/count', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/folders/count', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/folders/count', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/folders/count");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /folders/count`

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "count": 0
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_folders-param1

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/folders/{param1}
````

````http
GET https://app.observepoint.com/api/v2/folders/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/folders/{param1}',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/folders/{param1}', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/folders/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/folders/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/folders/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /folders/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "appsRunning": 0,
    "appsInQueue": 0,
    "name": "string",
    "appRuleFailures": 0,
    "createdByUserName": "string",
    "appsCount": 0,
    "accountId": 0,
    "createdByUserId": 0,
    "id": 0,
    "auditsRunning": 0,
    "createdAt": "string",
    "appFailures": 0,
    "simulationErrors": 0,
    "simulationsRunning": 0,
    "domainsCount": 0
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## PUT_folders-param1

> Code samples

````shell
# You can also use wget
curl -X put https://app.observepoint.com/api/v2/folders/{param1}
````

````http
PUT https://app.observepoint.com/api/v2/folders/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/folders/{param1}',
    method: 'put',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/folders/{param1}', { method: 'PUT'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.put 'https://app.observepoint.com/api/v2/folders/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.put('https://app.observepoint.com/api/v2/folders/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/folders/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("PUT");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`PUT /folders/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
body|body|object|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

> Body parameter

````json
{
  "id": 531,
  "accountId": 19,
  "name": "testingstoplight1",
  "domainsCount": 0,
  "appsCount": 0
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "appsRunning": 0,
    "appsInQueue": 0,
    "name": "string",
    "appRuleFailures": 0,
    "createdByUserName": "string",
    "appsCount": 0,
    "accountId": 0,
    "createdByUserId": 0,
    "id": 0,
    "auditsRunning": 0,
    "createdAt": "string",
    "appFailures": 0,
    "simulationErrors": 0,
    "simulationsRunning": 0,
    "domainsCount": 0
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## DELETE_folders-param1

> Code samples

````shell
# You can also use wget
curl -X delete https://app.observepoint.com/api/v2/folders/{param1}
````

````http
DELETE https://app.observepoint.com/api/v2/folders/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/folders/{param1}',
    method: 'delete',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/folders/{param1}', { method: 'DELETE'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.delete 'https://app.observepoint.com/api/v2/folders/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.delete('https://app.observepoint.com/api/v2/folders/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/folders/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("DELETE");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`DELETE /folders/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|No description

> Example responses

````json
{}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_folders-param1-users

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/folders/{param1}/users
````

````http
GET https://app.observepoint.com/api/v2/folders/{param1}/users HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/folders/{param1}/users',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/folders/{param1}/users', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/folders/{param1}/users', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/folders/{param1}/users', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/folders/{param1}/users");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /folders/{param1}/users`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
Authorization|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "array",
      "items": {
        "type": "object",
        "properties": {
          "email": {
            "type": "string"
          },
          "username": {
            "type": "string"
          },
          "timezone": {
            "type": "string"
          },
          "permissions": {
            "type": "string"
          },
          "accountId": {
            "type": "integer"
          },
          "lastName": {
            "type": "string"
          },
          "firstName": {
            "type": "string"
          },
          "id": {
            "type": "integer"
          },
          "updated": {
            "type": "string"
          },
          "created": {
            "type": "string"
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_folders-param1-users

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/folders/{param1}/users
````

````http
POST https://app.observepoint.com/api/v2/folders/{param1}/users HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/folders/{param1}/users',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/folders/{param1}/users', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/folders/{param1}/users', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/folders/{param1}/users', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/folders/{param1}/users");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /folders/{param1}/users`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
body|body|object|false|No description
Content-Type|header|string|false|No description
Authorization|header|string|false|No description

> Body parameter

````json
[
  72
]
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "array",
      "items": {
        "type": "object",
        "properties": {
          "email": {
            "type": "string"
          },
          "username": {
            "type": "string"
          },
          "timezone": {
            "type": "string"
          },
          "permissions": {
            "type": "string"
          },
          "accountId": {
            "type": "integer"
          },
          "lastName": {
            "type": "string"
          },
          "firstName": {
            "type": "string"
          },
          "id": {
            "type": "integer"
          },
          "updated": {
            "type": "string"
          },
          "created": {
            "type": "string"
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

# Report

## GET_report-compliance-business

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/web-audits/report/compliance/business
````

````http
GET https://app.observepoint.com/api/v2/web-audits/report/compliance/business HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-audits/report/compliance/business',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-audits/report/compliance/business', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/web-audits/report/compliance/business', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/web-audits/report/compliance/business', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-audits/report/compliance/business");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /web-audits/report/compliance/business`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "request": {
          "type": "object",
          "properties": {
            "runIds": {
              "type": "array",
              "items": {
                "type": "integer"
              }
            }
          }
        },
        "producedSelection": {
          "type": "object",
          "properties": {
            "runs": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "id": {
                    "type": "integer"
                  },
                  "completed": {
                    "type": "string"
                  }
                }
              }
            }
          }
        },
        "overviews": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "runId": {
                "type": "integer"
              },
              "pagesFailing": {
                "type": "integer"
              },
              "ruleSetFailing": {
                "type": "integer"
              }
            }
          }
        }
      }
    }
  }
}
````
````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_report-summary-audit

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/report/summary/audit
````

````http
GET https://app.observepoint.com/api/v2/report/summary/audit HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/summary/audit',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/summary/audit', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/report/summary/audit', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/report/summary/audit', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/summary/audit");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /report/summary/audit`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
audit_id|query|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "request": {
          "type": "object",
          "properties": {
            "auditId": {
              "type": "integer"
            }
          }
        },
        "producedSelection": {
          "type": "object",
          "properties": {
            "runs": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {}
              }
            },
            "auditId": {
              "type": "integer"
            }
          }
        }
      }
    }
  }
}
````
````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_report-page-load-time

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/report/page/load-time
````

````http
GET https://app.observepoint.com/api/v2/report/page/load-time HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/page/load-time',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/page/load-time', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/report/page/load-time', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/report/page/load-time', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/page/load-time");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /report/page/load-time`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description
account|query|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_report-summary-variable

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/report/summary/variable
````

````http
GET https://app.observepoint.com/api/v2/report/summary/variable HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/summary/variable',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/summary/variable', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/report/summary/variable', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/report/summary/variable', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/summary/variable");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /report/summary/variable`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "request": {
          "type": "object",
          "properties": {
            "runIds": {
              "type": "array",
              "items": {
                "type": "integer"
              }
            }
          }
        },
        "producedSelection": {
          "type": "object",
          "properties": {
            "runs": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "id": {
                    "type": "integer"
                  },
                  "completed": {
                    "type": "string"
                  }
                }
              }
            }
          }
        },
        "variableSummaries": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "runId": {
                "type": "integer"
              },
              "summaries": {
                "type": "array",
                "items": {
                  "type": "object",
                  "properties": {}
                }
              }
            }
          }
        }
      }
    }
  }
}
````
````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_report-tag-missing

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/report/tag/missing
````

````http
GET https://app.observepoint.com/api/v2/report/tag/missing HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/tag/missing',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/tag/missing', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/report/tag/missing', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/report/tag/missing', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/tag/missing");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /report/tag/missing`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "request": {
          "type": "object",
          "properties": {
            "runIds": {
              "type": "array",
              "items": {
                "type": "integer"
              }
            }
          }
        },
        "producedSelection": {
          "type": "object",
          "properties": {
            "runs": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "id": {
                    "type": "integer"
                  },
                  "completed": {
                    "type": "string"
                  }
                }
              }
            }
          }
        },
        "totalPages": {
          "type": "integer"
        },
        "runTags": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {}
          }
        }
      }
    }
  }
}
````
````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_report-tag-duplicate-requests

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/report/tag/duplicate-requests
````

````http
GET https://app.observepoint.com/api/v2/report/tag/duplicate-requests HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/tag/duplicate-requests',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/tag/duplicate-requests', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/report/tag/duplicate-requests', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/report/tag/duplicate-requests', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/tag/duplicate-requests");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /report/tag/duplicate-requests`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "request": {
          "type": "object",
          "properties": {
            "runIds": {
              "type": "array",
              "items": {
                "type": "integer"
              }
            }
          }
        },
        "producedSelection": {
          "type": "object",
          "properties": {
            "runs": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "id": {
                    "type": "integer"
                  },
                  "completed": {
                    "type": "string"
                  }
                }
              }
            }
          }
        },
        "totalPages": {
          "type": "integer"
        },
        "runTags": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {}
          }
        }
      }
    }
  }
}
````
````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_report-tag-status-codes

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/report/tag/status-codes
````

````http
GET https://app.observepoint.com/api/v2/report/tag/status-codes HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/tag/status-codes',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/tag/status-codes', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/report/tag/status-codes', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/report/tag/status-codes', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/tag/status-codes");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /report/tag/status-codes`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "request": {
          "type": "object",
          "properties": {
            "runIds": {
              "type": "array",
              "items": {
                "type": "integer"
              }
            }
          }
        },
        "producedSelection": {
          "type": "object",
          "properties": {
            "runs": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "id": {
                    "type": "integer"
                  },
                  "completed": {
                    "type": "string"
                  }
                }
              }
            }
          }
        },
        "totalPages": {
          "type": "integer"
        },
        "runTags": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {}
          }
        }
      }
    }
  }
}
````
````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_report-compliance-vendor

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/report/compliance/vendor
````

````http
GET https://app.observepoint.com/api/v2/report/compliance/vendor HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/compliance/vendor',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/compliance/vendor', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/report/compliance/vendor', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/report/compliance/vendor', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/compliance/vendor");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /report/compliance/vendor`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "request": {
          "type": "object",
          "properties": {
            "runIds": {
              "type": "array",
              "items": {
                "type": "integer"
              }
            }
          }
        },
        "producedSelection": {
          "type": "object",
          "properties": {
            "runs": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "id": {
                    "type": "integer"
                  },
                  "completed": {
                    "type": "string"
                  }
                }
              }
            }
          }
        },
        "overviews": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "runId": {
                "type": "integer"
              },
              "tagsFailing": {
                "type": "integer"
              },
              "tagsCompliant": {
                "type": "integer"
              }
            }
          }
        }
      }
    }
  }
}
````
````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_report-page-javascript-errors

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/report/page/javascript-errors
````

````http
GET https://app.observepoint.com/api/v2/report/page/javascript-errors HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/page/javascript-errors',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/page/javascript-errors', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/report/page/javascript-errors', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/report/page/javascript-errors', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/page/javascript-errors");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /report/page/javascript-errors`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description
account|query|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_report-summary-tags

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/report/summary/tags
````

````http
GET https://app.observepoint.com/api/v2/report/summary/tags HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/summary/tags',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/summary/tags', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/report/summary/tags', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/report/summary/tags', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/summary/tags");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /report/summary/tags`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "request": {
          "type": "object",
          "properties": {
            "runIds": {
              "type": "array",
              "items": {
                "type": "integer"
              }
            }
          }
        },
        "producedSelection": {
          "type": "object",
          "properties": {
            "runs": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "id": {
                    "type": "integer"
                  },
                  "completed": {
                    "type": "string"
                  }
                }
              }
            }
          }
        },
        "tagSummaries": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "runId": {
                "type": "integer"
              }
            }
          }
        }
      }
    }
  }
}
````
````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_report-tag-versions-page-overview

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/report/tag/versions/page-overview
````

````http
POST https://app.observepoint.com/api/v2/report/tag/versions/page-overview HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/tag/versions/page-overview',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/tag/versions/page-overview', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/report/tag/versions/page-overview', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/report/tag/versions/page-overview', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/tag/versions/page-overview");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /report/tag/versions/page-overview`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description
account|query|integer|false|No description
body|body|object|false|No description

> Body parameter

````json
{
  "identifiers": []
}
````
### Responses

Status|Meaning|Description
---|---|---|
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_report-tag-multiple-requests-page-overview

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/report/tag/multiple-requests/page-overview
````

````http
POST https://app.observepoint.com/api/v2/report/tag/multiple-requests/page-overview HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/tag/multiple-requests/page-overview',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/tag/multiple-requests/page-overview', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/report/tag/multiple-requests/page-overview', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/report/tag/multiple-requests/page-overview', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/tag/multiple-requests/page-overview");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /report/tag/multiple-requests/page-overview`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description
account|query|integer|false|No description
body|body|object|false|No description

> Body parameter

````json
{
  "identifiers": []
}
````
### Responses

Status|Meaning|Description
---|---|---|
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_report-tag-presence-page-overview

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/report/tag/presence/page-overview
````

````http
POST https://app.observepoint.com/api/v2/report/tag/presence/page-overview HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/tag/presence/page-overview',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/tag/presence/page-overview', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/report/tag/presence/page-overview', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/report/tag/presence/page-overview', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/tag/presence/page-overview");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /report/tag/presence/page-overview`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description
account|query|integer|false|No description
body|body|object|false|No description

> Body parameter

````json
{
  "identifiers": []
}
````
### Responses

Status|Meaning|Description
---|---|---|
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_report-mobile-journey-export

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/report/mobile-journey/export
````

````http
POST https://app.observepoint.com/api/v2/report/mobile-journey/export HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/mobile-journey/export',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/mobile-journey/export', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/report/mobile-journey/export', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/report/mobile-journey/export', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/mobile-journey/export");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /report/mobile-journey/export`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "request": {
          "type": "object",
          "properties": {
            "runIds": {
              "type": "array",
              "items": {
                "type": "integer"
              }
            },
            "filename": {
              "type": "string"
            }
          }
        },
        "producedSelection": {
          "type": "object",
          "properties": {
            "runs": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "id": {
                    "type": "integer"
                  },
                  "completed": {
                    "type": "string"
                  }
                }
              }
            }
          }
        },
        "fileInfo": {
          "type": "object",
          "properties": {
            "file": {
              "type": "string"
            },
            "metadata": {
              "type": "string"
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_report-tag-versions

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/report/tag/versions
````

````http
GET https://app.observepoint.com/api/v2/report/tag/versions HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/tag/versions',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/tag/versions', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/report/tag/versions', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/report/tag/versions', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/tag/versions");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /report/tag/versions`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "request": {
          "type": "object",
          "properties": {
            "runIds": {
              "type": "array",
              "items": {
                "type": "integer"
              }
            }
          }
        },
        "producedSelection": {
          "type": "object",
          "properties": {
            "runs": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "id": {
                    "type": "integer"
                  },
                  "completed": {
                    "type": "string"
                  }
                }
              }
            }
          }
        },
        "totalPages": {
          "type": "integer"
        },
        "runTags": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {}
          }
        }
      }
    }
  }
}
````
````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_report-tag-multiple-requests

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/report/tag/multiple-requests
````

````http
GET https://app.observepoint.com/api/v2/report/tag/multiple-requests HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/tag/multiple-requests',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/tag/multiple-requests', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/report/tag/multiple-requests', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/report/tag/multiple-requests', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/tag/multiple-requests");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /report/tag/multiple-requests`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "request": {
          "type": "object",
          "properties": {
            "runIds": {
              "type": "array",
              "items": {
                "type": "integer"
              }
            }
          }
        },
        "producedSelection": {
          "type": "object",
          "properties": {
            "runs": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "id": {
                    "type": "integer"
                  },
                  "completed": {
                    "type": "string"
                  }
                }
              }
            }
          }
        },
        "totalPages": {
          "type": "integer"
        },
        "runTags": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {}
          }
        }
      }
    }
  }
}
````
````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_report-tag-presence

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/report/tag/presence
````

````http
GET https://app.observepoint.com/api/v2/report/tag/presence HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/tag/presence',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/tag/presence', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/report/tag/presence', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/report/tag/presence', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/tag/presence");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /report/tag/presence`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description
audit_id|query|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "request": {
          "type": "object",
          "properties": {
            "runIds": {
              "type": "array",
              "items": {
                "type": "integer"
              }
            }
          }
        },
        "producedSelection": {
          "type": "object",
          "properties": {
            "runs": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "id": {
                    "type": "integer"
                  },
                  "completed": {
                    "type": "string"
                  }
                }
              }
            }
          }
        },
        "totalPages": {
          "type": "integer"
        },
        "runTags": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {}
          }
        }
      }
    }
  }
}
````
````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_report-page-status-codes

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/report/page/status-codes
````

````http
GET https://app.observepoint.com/api/v2/report/page/status-codes HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/page/status-codes',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/page/status-codes', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/report/page/status-codes', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/report/page/status-codes', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/page/status-codes");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /report/page/status-codes`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description
account|query|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_report-summary-scoring

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/report/summary/scoring
````

````http
GET https://app.observepoint.com/api/v2/report/summary/scoring HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/summary/scoring',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/summary/scoring', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/report/summary/scoring', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/report/summary/scoring', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/summary/scoring");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /report/summary/scoring`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
audit_id|query|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "request": {
          "type": "object",
          "properties": {
            "auditId": {
              "type": "integer"
            },
            "dateRange": {
              "type": "object",
              "properties": {
                "start": {
                  "type": "string"
                }
              }
            }
          }
        },
        "producedSelection": {
          "type": "object",
          "properties": {
            "runs": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {}
              }
            },
            "auditId": {
              "type": "integer"
            },
            "dateRange": {
              "type": "object",
              "properties": {
                "start": {
                  "type": "string"
                }
              }
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_report-tag-missing-page-overview

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/report/tag/missing/page-overview
````

````http
POST https://app.observepoint.com/api/v2/report/tag/missing/page-overview HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/tag/missing/page-overview',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/tag/missing/page-overview', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/report/tag/missing/page-overview', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/report/tag/missing/page-overview', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/tag/missing/page-overview");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /report/tag/missing/page-overview`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description
account|query|integer|false|No description
body|body|object|false|No description

> Body parameter

````json
{
  "identifiers": []
}
````
### Responses

Status|Meaning|Description
---|---|---|
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_report-tag-duplicate-requests-page-overview

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/report/tag/duplicate-requests/page-overview
````

````http
POST https://app.observepoint.com/api/v2/report/tag/duplicate-requests/page-overview HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/tag/duplicate-requests/page-overview',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/tag/duplicate-requests/page-overview', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/report/tag/duplicate-requests/page-overview', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/report/tag/duplicate-requests/page-overview', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/tag/duplicate-requests/page-overview");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /report/tag/duplicate-requests/page-overview`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description
account|query|integer|false|No description
body|body|object|false|No description

> Body parameter

````json
{
  "identifiers": []
}
````
### Responses

Status|Meaning|Description
---|---|---|
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_report-tag-status-codes-page-overview

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/report/tag/status-codes/page-overview
````

````http
POST https://app.observepoint.com/api/v2/report/tag/status-codes/page-overview HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/tag/status-codes/page-overview',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/tag/status-codes/page-overview', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/report/tag/status-codes/page-overview', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/report/tag/status-codes/page-overview', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/tag/status-codes/page-overview");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /report/tag/status-codes/page-overview`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description
account|query|integer|false|No description
body|body|object|false|No description

> Body parameter

````json
{
  "identifiers": []
}
````
### Responses

Status|Meaning|Description
---|---|---|
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_report-advanced-full-vendor

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/report/advanced/full-vendor
````

````http
POST https://app.observepoint.com/api/v2/report/advanced/full-vendor HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/advanced/full-vendor',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/advanced/full-vendor', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/report/advanced/full-vendor', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/report/advanced/full-vendor', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/advanced/full-vendor");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /report/advanced/full-vendor`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
account|query|integer|false|No description
audit_id|query|integer|false|No description
body|body|object|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

> Body parameter

````json
{
  "identifiers": []
}
````
### Responses

Status|Meaning|Description
---|---|---|
500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|No description

> Example responses

````json
{
  "success": true,
  "error": {
    "code": 0,
    "message": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_report-web-journey-export

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/report/web-journey/export
````

````http
POST https://app.observepoint.com/api/v2/report/web-journey/export HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/report/web-journey/export',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/report/web-journey/export', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/report/web-journey/export', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/report/web-journey/export', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/report/web-journey/export");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /report/web-journey/export`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
run_id|query|integer|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "request": {
          "type": "object",
          "properties": {
            "runIds": {
              "type": "array",
              "items": {
                "type": "integer"
              }
            },
            "filename": {
              "type": "string"
            }
          }
        },
        "producedSelection": {
          "type": "object",
          "properties": {
            "runs": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "id": {
                    "type": "integer"
                  },
                  "completed": {
                    "type": "string"
                  }
                }
              }
            }
          }
        },
        "fileInfo": {
          "type": "object",
          "properties": {
            "file": {
              "type": "string"
            },
            "metadata": {
              "type": "string"
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

# Rule-sets

## GET_rule-sets-param1-audits

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/rule-sets/{param1}/audits
````

````http
GET https://app.observepoint.com/api/v2/rule-sets/{param1}/audits HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/rule-sets/{param1}/audits',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/rule-sets/{param1}/audits', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/rule-sets/{param1}/audits', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/rule-sets/{param1}/audits', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/rule-sets/{param1}/audits");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /rule-sets/{param1}/audits`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {}
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_rule-sets-param1-web-sims

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/rule-sets/{param1}/web-sims
````

````http
GET https://app.observepoint.com/api/v2/rule-sets/{param1}/web-sims HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/rule-sets/{param1}/web-sims',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/rule-sets/{param1}/web-sims', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/rule-sets/{param1}/web-sims', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/rule-sets/{param1}/web-sims', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/rule-sets/{param1}/web-sims");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /rule-sets/{param1}/web-sims`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "array",
      "items": {
        "type": "object",
        "properties": {
          "name": {
            "type": "string"
          },
          "lastCheck": {
            "type": "string"
          },
          "state": {
            "type": "string"
          },
          "simulationRunning": {
            "type": "boolean"
          },
          "folderId": {
            "type": "integer"
          },
          "options": {
            "type": "object",
            "properties": {
              "location": {
                "type": "string"
              },
              "browserWidth": {
                "type": "integer"
              },
              "reminders": {
                "type": "boolean"
              },
              "userAgent": {
                "type": "string"
              },
              "loadFlash": {
                "type": "boolean"
              },
              "frequency": {
                "type": "string"
              },
              "alerts": {
                "type": "boolean"
              }
            }
          },
          "id": {
            "type": "integer"
          },
          "createdAt": {
            "type": "string"
          },
          "domainId": {
            "type": "integer"
          },
          "actions": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {}
            }
          },
          "nextCheck": {
            "type": "string"
          },
          "userId": {
            "type": "integer"
          },
          "emails": {
            "type": "array",
            "items": {
              "type": "string"
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_rule-sets-param1-apps

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/rule-sets/{param1}/apps
````

````http
GET https://app.observepoint.com/api/v2/rule-sets/{param1}/apps HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/rule-sets/{param1}/apps',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/rule-sets/{param1}/apps', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/rule-sets/{param1}/apps', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/rule-sets/{param1}/apps', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/rule-sets/{param1}/apps");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /rule-sets/{param1}/apps`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "array",
      "items": {
        "type": "object",
        "properties": {
          "name": {
            "type": "string"
          },
          "updatedAt": {
            "type": "string"
          },
          "running": {
            "type": "integer"
          },
          "tests": {
            "type": "integer"
          },
          "folderId": {
            "type": "integer"
          },
          "id": {
            "type": "integer"
          },
          "inQueue": {
            "type": "integer"
          },
          "ruleFailures": {
            "type": "integer"
          },
          "failures": {
            "type": "integer"
          },
          "createdAt": {
            "type": "string"
          },
          "file": {
            "type": "string"
          },
          "screenshotFilename": {
            "type": "string"
          },
          "userId": {
            "type": "integer"
          },
          "platform": {
            "type": "integer"
          },
          "testSuites": {
            "type": "array",
            "items": {
              "type": "integer"
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_rule-sets

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/rule-sets
````

````http
GET https://app.observepoint.com/api/v2/rule-sets HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/rule-sets',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/rule-sets', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/rule-sets', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/rule-sets', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/rule-sets");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /rule-sets`

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "array",
      "items": {
        "type": "object",
        "properties": {
          "name": {
            "type": "string"
          },
          "updatedAt": {
            "type": "string"
          },
          "recipients": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {}
            }
          },
          "accountId": {
            "type": "integer"
          },
          "id": {
            "type": "integer"
          },
          "createdAt": {
            "type": "string"
          },
          "rules": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {
                "name": {
                  "type": "string"
                },
                "updatedAt": {
                  "type": "string"
                },
                "tags": {
                  "type": "array",
                  "items": {
                    "type": "object",
                    "properties": {
                      "id": {
                        "type": "integer"
                      },
                      "condition": {
                        "type": "boolean"
                      },
                      "tagId": {
                        "type": "integer"
                      },
                      "ruleId": {
                        "type": "integer"
                      }
                    }
                  }
                },
                "id": {
                  "type": "integer"
                },
                "createdAt": {
                  "type": "string"
                },
                "ruleSetId": {
                  "type": "integer"
                }
              }
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_rule-sets

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/rule-sets
````

````http
POST https://app.observepoint.com/api/v2/rule-sets HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/rule-sets',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/rule-sets', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/rule-sets', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/rule-sets', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/rule-sets");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /rule-sets`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
body|body|object|false|No description

> Body parameter

````json
{
  "name": "garbage",
  "rules": [
    {
      "id": null,
      "name": "garbage",
      "ruleSetId": null,
      "pageFilters": [],
      "tags": [
        {
          "id": null,
          "ruleId": null,
          "tagId": 240,
          "matchType": "Equals",
          "account": "u5wROFQLQrgirhiXnEjdatXN7dbE9vNP",
          "condition": false
        },
        {
          "id": null,
          "ruleId": null,
          "tagId": 240,
          "matchType": null,
          "account": null,
          "condition": true,
          "variables": []
        }
      ],
      "expectations": [
        {
          "id": null,
          "ruleId": null,
          "tagId": 240,
          "matchType": null,
          "account": null,
          "condition": true,
          "variables": []
        }
      ]
    }
  ],
  "recipients": []
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "name": {
          "type": "string"
        },
        "updatedAt": {
          "type": "string"
        },
        "recipients": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {}
          }
        },
        "accountId": {
          "type": "integer"
        },
        "id": {
          "type": "integer"
        },
        "createdAt": {
          "type": "string"
        },
        "rules": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "name": {
                "type": "string"
              },
              "updatedAt": {
                "type": "string"
              },
              "tags": {
                "type": "array",
                "items": {
                  "type": "object",
                  "properties": {
                    "matchType": {
                      "type": "string"
                    },
                    "id": {
                      "type": "integer"
                    },
                    "condition": {
                      "type": "boolean"
                    },
                    "tagId": {
                      "type": "integer"
                    },
                    "account": {
                      "type": "string"
                    },
                    "ruleId": {
                      "type": "integer"
                    }
                  }
                }
              },
              "id": {
                "type": "integer"
              },
              "createdAt": {
                "type": "string"
              },
              "ruleSetId": {
                "type": "integer"
              }
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## PUT_rule-sets-param1

> Code samples

````shell
# You can also use wget
curl -X put https://app.observepoint.com/api/v2/rule-sets/{param1}
````

````http
PUT https://app.observepoint.com/api/v2/rule-sets/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/rule-sets/{param1}',
    method: 'put',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/rule-sets/{param1}', { method: 'PUT'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.put 'https://app.observepoint.com/api/v2/rule-sets/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.put('https://app.observepoint.com/api/v2/rule-sets/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/rule-sets/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("PUT");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`PUT /rule-sets/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
body|body|object|false|No description

> Body parameter

````json
{
  "name": "garbage rule set",
  "updatedAt": "2016-11-17T23:58:08.000-07:00",
  "recipients": [
    "mike.cataldo@observepoint.com"
  ],
  "accountId": 19,
  "id": 122,
  "createdAt": "2016-11-17T23:58:08.000-07:00",
  "rules": [
    {
      "name": "Unthistitled Rule 1",
      "updatedAt": "2016-11-17T23:58:08.000-07:00",
      "tags": [],
      "pageFilters": [],
      "id": 166,
      "createdAt": "2016-11-17T23:58:08.000-07:00",
      "ruleSetId": 122,
      "expectations": []
    }
  ],
  "show": false,
  "automatedJourneys": [],
  "apps": [],
  "guidedJourneys": []
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "name": {
          "type": "string"
        },
        "updatedAt": {
          "type": "string"
        },
        "recipients": {
          "type": "array",
          "items": {
            "type": "string"
          }
        },
        "accountId": {
          "type": "integer"
        },
        "id": {
          "type": "integer"
        },
        "createdAt": {
          "type": "string"
        },
        "rules": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "name": {
                "type": "string"
              },
              "updatedAt": {
                "type": "string"
              },
              "id": {
                "type": "integer"
              },
              "createdAt": {
                "type": "string"
              },
              "ruleSetId": {
                "type": "integer"
              }
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

# Search

## GET_search

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/search
````

````http
GET https://app.observepoint.com/api/v2/search HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/search',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/search', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/search', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/search', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/search");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /search`

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "mobileJourneys": [
      {}
    ],
    "domains": [
      {}
    ],
    "folders": [
      {}
    ],
    "webJourneys": [
      {}
    ],
    "audits": [
      {}
    ],
    "apps": [
      {}
    ]
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

# Suites

## DELETE_suites-param1

> Code samples

````shell
# You can also use wget
curl -X delete https://app.observepoint.com/api/v2/suites/{param1}
````

````http
DELETE https://app.observepoint.com/api/v2/suites/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/suites/{param1}',
    method: 'delete',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/suites/{param1}', { method: 'DELETE'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.delete 'https://app.observepoint.com/api/v2/suites/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.delete('https://app.observepoint.com/api/v2/suites/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/suites/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("DELETE");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`DELETE /suites/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|No description

> Example responses

````json
{}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_suites-param1

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/suites/{param1}
````

````http
GET https://app.observepoint.com/api/v2/suites/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/suites/{param1}',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/suites/{param1}', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/suites/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/suites/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/suites/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /suites/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "name": "string",
    "updatedAt": "string",
    "mobileApps": [
      0
    ],
    "accountId": 0,
    "nextTest": "string",
    "id": 0,
    "createdAt": "string",
    "frequency": 0,
    "userId": 0,
    "_links": {
      "self": {
        "href": "string"
      },
      "op:tests": {
        "href": "string"
      },
      "curies": [
        {
          "name": "string",
          "href": "string",
          "templated": true
        }
      ]
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## PUT_suites-param1

> Code samples

````shell
# You can also use wget
curl -X put https://app.observepoint.com/api/v2/suites/{param1}
````

````http
PUT https://app.observepoint.com/api/v2/suites/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/suites/{param1}',
    method: 'put',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/suites/{param1}', { method: 'PUT'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.put 'https://app.observepoint.com/api/v2/suites/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.put('https://app.observepoint.com/api/v2/suites/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/suites/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("PUT");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`PUT /suites/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
body|body|object|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

> Body parameter

````json
{
  "id": 138,
  "name": "testing stoplight22",
  "frequency": 7,
  "mobileApps": [
    178
  ]
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "name": {
          "type": "string"
        },
        "updatedAt": {
          "type": "string"
        },
        "mobileApps": {
          "type": "array",
          "items": {
            "type": "integer"
          }
        },
        "accountId": {
          "type": "integer"
        },
        "id": {
          "type": "integer"
        },
        "createdAt": {
          "type": "string"
        },
        "frequency": {
          "type": "integer"
        },
        "userId": {
          "type": "integer"
        },
        "_links": {
          "type": "object",
          "properties": {
            "self": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            },
            "op:tests": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            },
            "curies": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "name": {
                    "type": "string"
                  },
                  "href": {
                    "type": "string"
                  },
                  "templated": {
                    "type": "boolean"
                  }
                }
              }
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_suites-param1-tests

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/suites/{param1}/tests
````

````http
GET https://app.observepoint.com/api/v2/suites/{param1}/tests HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/suites/{param1}/tests',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/suites/{param1}/tests', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/suites/{param1}/tests', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/suites/{param1}/tests', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/suites/{param1}/tests");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /suites/{param1}/tests`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "_links": {
          "type": "object",
          "properties": {
            "self": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            },
            "curies": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "name": {
                    "type": "string"
                  },
                  "href": {
                    "type": "string"
                  },
                  "templated": {
                    "type": "boolean"
                  }
                }
              }
            }
          }
        },
        "_embedded": {
          "type": "object",
          "properties": {
            "op:tests": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "lastRunId": {
                    "type": "integer"
                  },
                  "name": {
                    "type": "string"
                  },
                  "updatedAt": {
                    "type": "string"
                  },
                  "id": {
                    "type": "integer"
                  },
                  "countryCode": {
                    "type": "string"
                  },
                  "status": {
                    "type": "integer"
                  },
                  "createdAt": {
                    "type": "string"
                  },
                  "userId": {
                    "type": "integer"
                  },
                  "osVersion": {
                    "type": "string"
                  },
                  "device": {
                    "type": "integer"
                  },
                  "suiteId": {
                    "type": "integer"
                  },
                  "_links": {
                    "type": "object",
                    "properties": {
                      "op:runs": {
                        "type": "object",
                        "properties": {
                          "href": {
                            "type": "string"
                          }
                        }
                      },
                      "self": {
                        "type": "object",
                        "properties": {
                          "href": {
                            "type": "string"
                          }
                        }
                      },
                      "op:actions": {
                        "type": "object",
                        "properties": {
                          "href": {
                            "type": "string"
                          }
                        }
                      },
                      "op:results": {
                        "type": "object",
                        "properties": {
                          "href": {
                            "type": "string"
                          }
                        }
                      },
                      "op:suite": {
                        "type": "object",
                        "properties": {
                          "href": {
                            "type": "string"
                          }
                        }
                      }
                    }
                  }
                }
              }
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_suites-param1-run

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/suites/{param1}/run
````

````http
POST https://app.observepoint.com/api/v2/suites/{param1}/run HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/suites/{param1}/run',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/suites/{param1}/run', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/suites/{param1}/run', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/suites/{param1}/run', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/suites/{param1}/run");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /suites/{param1}/run`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "name": "string",
    "updatedAt": "string",
    "mobileApps": [
      0
    ],
    "accountId": 0,
    "nextTest": "string",
    "id": 0,
    "createdAt": "string",
    "frequency": 0,
    "userId": 0,
    "_links": {
      "self": {
        "href": "string"
      },
      "op:tests": {
        "href": "string"
      },
      "curies": [
        {
          "name": "string",
          "href": "string",
          "templated": true
        }
      ]
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_suites

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/suites
````

````http
POST https://app.observepoint.com/api/v2/suites HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/suites',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/suites', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/suites', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/suites', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/suites");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /suites`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
body|body|object|false|No description
Content-Type|header|string|false|No description
Authorization|header|string|false|No description

> Body parameter

````json
{
  "name": "testing stoplight",
  "frequency": 7,
  "mobileApps": [
    178
  ]
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "name": {
          "type": "string"
        },
        "updatedAt": {
          "type": "string"
        },
        "mobileApps": {
          "type": "array",
          "items": {
            "type": "integer"
          }
        },
        "accountId": {
          "type": "integer"
        },
        "id": {
          "type": "integer"
        },
        "createdAt": {
          "type": "string"
        },
        "frequency": {
          "type": "integer"
        },
        "userId": {
          "type": "integer"
        },
        "_links": {
          "type": "object",
          "properties": {
            "self": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            },
            "op:tests": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            },
            "curies": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "name": {
                    "type": "string"
                  },
                  "href": {
                    "type": "string"
                  },
                  "templated": {
                    "type": "boolean"
                  }
                }
              }
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

# Tags

## GET_tags

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/tags
````

````http
GET https://app.observepoint.com/api/v2/tags HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/tags',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/tags', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/tags', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/tags', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/tags");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /tags`

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
[
  {
    "id": 0,
    "name": "string",
    "icon": "string",
    "category": {
      "id": 0,
      "name": "string"
    }
  }
]
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_tags-param1

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/tags/{param1}
````

````http
GET https://app.observepoint.com/api/v2/tags/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/tags/{param1}',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/tags/{param1}', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/tags/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/tags/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/tags/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /tags/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "id": 0,
  "name": "string",
  "icon": "string",
  "category": {
    "id": 0,
    "name": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

# Tests

## DELETE_tests-param1

> Code samples

````shell
# You can also use wget
curl -X delete https://app.observepoint.com/api/v2/tests/{param1}
````

````http
DELETE https://app.observepoint.com/api/v2/tests/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/tests/{param1}',
    method: 'delete',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/tests/{param1}', { method: 'DELETE'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.delete 'https://app.observepoint.com/api/v2/tests/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.delete('https://app.observepoint.com/api/v2/tests/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/tests/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("DELETE");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`DELETE /tests/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|No description

> Example responses

````json
{}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_tests-param1

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/tests/{param1}
````

````http
GET https://app.observepoint.com/api/v2/tests/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/tests/{param1}',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/tests/{param1}', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/tests/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/tests/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/tests/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /tests/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "lastRunId": {
          "type": "integer"
        },
        "name": {
          "type": "string"
        },
        "updatedAt": {
          "type": "string"
        },
        "id": {
          "type": "integer"
        },
        "countryCode": {
          "type": "string"
        },
        "status": {
          "type": "integer"
        },
        "createdAt": {
          "type": "string"
        },
        "userId": {
          "type": "integer"
        },
        "osVersion": {
          "type": "string"
        },
        "device": {
          "type": "integer"
        },
        "suiteId": {
          "type": "integer"
        },
        "_links": {
          "type": "object",
          "properties": {
            "op:runs": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            },
            "curies": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "name": {
                    "type": "string"
                  },
                  "href": {
                    "type": "string"
                  },
                  "templated": {
                    "type": "boolean"
                  }
                }
              }
            },
            "self": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            },
            "op:actions": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            },
            "op:results": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            },
            "op:suite": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## PUT_tests-param1

> Code samples

````shell
# You can also use wget
curl -X put https://app.observepoint.com/api/v2/tests/{param1}
````

````http
PUT https://app.observepoint.com/api/v2/tests/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/tests/{param1}',
    method: 'put',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/tests/{param1}', { method: 'PUT'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.put 'https://app.observepoint.com/api/v2/tests/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.put('https://app.observepoint.com/api/v2/tests/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/tests/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("PUT");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`PUT /tests/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
body|body|object|false|No description

> Body parameter

````json
{
  "id": 190,
  "name": "testing stoplight",
  "suiteId": 137,
  "device": 6,
  "osVersion": "4.4",
  "countryCode": "US"
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "name": {
          "type": "string"
        },
        "updatedAt": {
          "type": "string"
        },
        "id": {
          "type": "integer"
        },
        "countryCode": {
          "type": "string"
        },
        "createdAt": {
          "type": "string"
        },
        "userId": {
          "type": "integer"
        },
        "osVersion": {
          "type": "string"
        },
        "device": {
          "type": "integer"
        },
        "suiteId": {
          "type": "integer"
        },
        "_links": {
          "type": "object",
          "properties": {
            "op:runs": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            },
            "curies": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "name": {
                    "type": "string"
                  },
                  "href": {
                    "type": "string"
                  },
                  "templated": {
                    "type": "boolean"
                  }
                }
              }
            },
            "self": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            },
            "op:actions": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            },
            "op:suite": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_tests-param1-runs

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/tests/{param1}/runs
````

````http
GET https://app.observepoint.com/api/v2/tests/{param1}/runs HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/tests/{param1}/runs',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/tests/{param1}/runs', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/tests/{param1}/runs', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/tests/{param1}/runs', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/tests/{param1}/runs");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /tests/{param1}/runs`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
Authorization|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "_links": {
          "type": "object",
          "properties": {
            "self": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            },
            "curies": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "name": {
                    "type": "string"
                  },
                  "href": {
                    "type": "string"
                  },
                  "templated": {
                    "type": "boolean"
                  }
                }
              }
            }
          }
        },
        "_embedded": {
          "type": "object",
          "properties": {
            "op:runs": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "requestedAt": {
                    "type": "string"
                  },
                  "id": {
                    "type": "integer"
                  },
                  "testId": {
                    "type": "integer"
                  },
                  "appId": {
                    "type": "integer"
                  },
                  "_links": {
                    "type": "object",
                    "properties": {
                      "self": {
                        "type": "object",
                        "properties": {
                          "href": {
                            "type": "string"
                          }
                        }
                      },
                      "op:app": {
                        "type": "object",
                        "properties": {
                          "href": {
                            "type": "string"
                          }
                        }
                      },
                      "op:results": {
                        "type": "object",
                        "properties": {
                          "href": {
                            "type": "string"
                          }
                        }
                      }
                    }
                  }
                }
              }
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_tests-param1-actions-param2-rules

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}/rules
````

````http
GET https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}/rules HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}/rules',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}/rules', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}/rules', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}/rules', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}/rules");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /tests/{param1}/actions/{param2}/rules`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
param2|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {}
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_tests-param1-actions-param2-rules

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}/rules
````

````http
POST https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}/rules HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}/rules',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}/rules', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}/rules', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}/rules', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}/rules");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /tests/{param1}/actions/{param2}/rules`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
param2|path|integer|true|No description
body|body|object|false|No description
Content-Type|header|string|false|No description
Authorization|header|string|false|No description

> Body parameter

````json
{
  "add": [
    18
  ],
  "remove": []
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    0
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_tests-param1-runs-param2-failures

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/tests/{param1}/runs/{param2}/failures
````

````http
GET https://app.observepoint.com/api/v2/tests/{param1}/runs/{param2}/failures HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/tests/{param1}/runs/{param2}/failures',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/tests/{param1}/runs/{param2}/failures', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/tests/{param1}/runs/{param2}/failures', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/tests/{param1}/runs/{param2}/failures', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/tests/{param1}/runs/{param2}/failures");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /tests/{param1}/runs/{param2}/failures`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
param2|path|string|true|No description
action_id|query|integer|false|No description
Authorization|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {}
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_tests-param1-actions

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/tests/{param1}/actions
````

````http
GET https://app.observepoint.com/api/v2/tests/{param1}/actions HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/tests/{param1}/actions',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/tests/{param1}/actions', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/tests/{param1}/actions', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/tests/{param1}/actions', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/tests/{param1}/actions");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /tests/{param1}/actions`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "array",
      "items": {
        "type": "object",
        "properties": {
          "id": {
            "type": "integer"
          },
          "actionType": {
            "type": "integer"
          },
          "sequence": {
            "type": "integer"
          },
          "testId": {
            "type": "integer"
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_tests-param1-actions

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/tests/{param1}/actions
````

````http
POST https://app.observepoint.com/api/v2/tests/{param1}/actions HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/tests/{param1}/actions',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/tests/{param1}/actions', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/tests/{param1}/actions', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/tests/{param1}/actions', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/tests/{param1}/actions");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /tests/{param1}/actions`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
vujb|query|boolean|false|No description
body|body|object|false|No description

> Body parameter

````json
{
  "testId": 190,
  "actionType": 14,
  "sequence": 0
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "action": {
          "type": "object",
          "properties": {
            "id": {
              "type": "integer"
            },
            "actionType": {
              "type": "integer"
            },
            "sequence": {
              "type": "integer"
            },
            "testId": {
              "type": "integer"
            }
          }
        },
        "success": {
          "type": "boolean"
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_tests-countries

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/tests/countries
````

````http
GET https://app.observepoint.com/api/v2/tests/countries HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/tests/countries',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/tests/countries', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/tests/countries', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/tests/countries', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/tests/countries");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /tests/countries`

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {
      "code": "string",
      "name": "string"
    }
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## PUT_tests-param1-actions-param2

> Code samples

````shell
# You can also use wget
curl -X put https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}
````

````http
PUT https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}',
    method: 'put',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}', { method: 'PUT'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.put 'https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.put('https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/tests/{param1}/actions/{param2}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("PUT");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`PUT /tests/{param1}/actions/{param2}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
param2|path|integer|true|No description
body|body|object|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

> Body parameter

````json
{
  "testId": 190,
  "actionType": 0,
  "sequence": 2,
  "elementType": 0,
  "value": 10000,
  "id": 1669
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "action": {
          "type": "object",
          "properties": {
            "id": {
              "type": "integer"
            },
            "actionType": {
              "type": "integer"
            },
            "sequence": {
              "type": "integer"
            },
            "testId": {
              "type": "integer"
            },
            "value": {
              "type": "integer"
            }
          }
        },
        "success": {
          "type": "boolean"
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_tests-param1-runs-param2-results

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/tests/{param1}/runs/{param2}/results
````

````http
GET https://app.observepoint.com/api/v2/tests/{param1}/runs/{param2}/results HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/tests/{param1}/runs/{param2}/results',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/tests/{param1}/runs/{param2}/results', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/tests/{param1}/runs/{param2}/results', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/tests/{param1}/runs/{param2}/results', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/tests/{param1}/runs/{param2}/results");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /tests/{param1}/runs/{param2}/results`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
param2|path|string|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "_links": {
      "self": {
        "href": "string"
      },
      "curies": [
        {
          "name": "string",
          "href": "string",
          "templated": true
        }
      ]
    },
    "_embedded": {
      "op:results": [
        {}
      ]
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_tests

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/tests
````

````http
POST https://app.observepoint.com/api/v2/tests HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/tests',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/tests', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/tests', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/tests', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/tests");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /tests`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
body|body|object|false|No description

> Body parameter

````json
{
  "name": "testing stoplight",
  "suiteId": 137,
  "device": 6,
  "osVersion": "4.4",
  "countryCode": "US"
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "name": {
          "type": "string"
        },
        "updatedAt": {
          "type": "string"
        },
        "id": {
          "type": "integer"
        },
        "countryCode": {
          "type": "string"
        },
        "createdAt": {
          "type": "string"
        },
        "userId": {
          "type": "integer"
        },
        "osVersion": {
          "type": "string"
        },
        "device": {
          "type": "integer"
        },
        "suiteId": {
          "type": "integer"
        },
        "_links": {
          "type": "object",
          "properties": {
            "op:runs": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            },
            "curies": {
              "type": "array",
              "items": {
                "type": "object",
                "properties": {
                  "name": {
                    "type": "string"
                  },
                  "href": {
                    "type": "string"
                  },
                  "templated": {
                    "type": "boolean"
                  }
                }
              }
            },
            "self": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            },
            "op:actions": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            },
            "op:suite": {
              "type": "object",
              "properties": {
                "href": {
                  "type": "string"
                }
              }
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

# Web-sims

## GET_web-sims-param1

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/web-sims/{param1}
````

````http
GET https://app.observepoint.com/api/v2/web-sims/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-sims/{param1}',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-sims/{param1}', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/web-sims/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/web-sims/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-sims/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /web-sims/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "name": {
          "type": "string"
        },
        "lastCheck": {
          "type": "string"
        },
        "state": {
          "type": "string"
        },
        "simulationRunning": {
          "type": "boolean"
        },
        "folderId": {
          "type": "integer"
        },
        "options": {
          "type": "object",
          "properties": {
            "location": {
              "type": "string"
            },
            "browserWidth": {
              "type": "integer"
            },
            "reminders": {
              "type": "boolean"
            },
            "userAgent": {
              "type": "string"
            },
            "loadFlash": {
              "type": "boolean"
            },
            "frequency": {
              "type": "string"
            },
            "alerts": {
              "type": "boolean"
            }
          }
        },
        "id": {
          "type": "integer"
        },
        "createdAt": {
          "type": "string"
        },
        "domainId": {
          "type": "integer"
        },
        "actions": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {}
          }
        },
        "nextCheck": {
          "type": "string"
        },
        "userId": {
          "type": "integer"
        },
        "emails": {
          "type": "array",
          "items": {
            "type": "string"
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## DELETE_web-sims-param1

> Code samples

````shell
# You can also use wget
curl -X delete https://app.observepoint.com/api/v2/web-sims/{param1}
````

````http
DELETE https://app.observepoint.com/api/v2/web-sims/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-sims/{param1}',
    method: 'delete',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-sims/{param1}', { method: 'DELETE'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.delete 'https://app.observepoint.com/api/v2/web-sims/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.delete('https://app.observepoint.com/api/v2/web-sims/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-sims/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("DELETE");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`DELETE /web-sims/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
204|[No Content](https://tools.ietf.org/html/rfc7231#section-6.3.5)|No description

> Example responses

````json
{}
````
<aside class="success">
This operation does not require authentication
</aside>

## PUT_web-sims-param1

> Code samples

````shell
# You can also use wget
curl -X put https://app.observepoint.com/api/v2/web-sims/{param1}
````

````http
PUT https://app.observepoint.com/api/v2/web-sims/{param1} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-sims/{param1}',
    method: 'put',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-sims/{param1}', { method: 'PUT'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.put 'https://app.observepoint.com/api/v2/web-sims/{param1}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.put('https://app.observepoint.com/api/v2/web-sims/{param1}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-sims/{param1}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("PUT");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`PUT /web-sims/{param1}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
body|body|object|false|No description

> Body parameter

````json
{
  "id": 169,
  "name": "stoplight.io1",
  "domainId": 280,
  "emails": [
    "MIKE.CATALDO@OBSERVEPOINT.COM"
  ],
  "options": {
    "frequency": "weekly",
    "location": "mountain",
    "userAgent": "Firefox(45.0.1) - Linux",
    "browserWidth": 1367,
    "alerts": true,
    "reminders": false,
    "loadFlash": false
  },
  "actions": [
    {
      "url": "http://stoplight.io",
      "label": "bael",
      "sequence": 0,
      "rules": [
        18
      ],
      "action": "navto"
    },
    {
      "identifier": "ytj",
      "preventNavigation": false,
      "label": "rjyy",
      "sequence": 1,
      "rules": [
        46
      ],
      "action": "click"
    },
    {
      "identifier": "sdg",
      "preventNavigation": false,
      "label": "arg",
      "sequence": 2,
      "rules": [
        20,
        45
      ],
      "value": "sdfg",
      "action": "input"
    },
    {
      "identifier": "sdfg",
      "preventNavigation": false,
      "label": "",
      "sequence": 3,
      "maskedValue": "ZFpoNLNohWDBmLHhRcN5qA==___!!!_!T7ochA2LbG1KY/R1MZkFnw==",
      "rules": [
        45,
        46
      ],
      "action": "maskedInput",
      "maskedInputType": "password",
      "viewedValue": "**********"
    },
    {
      "identifier": "dfgh",
      "preventNavigation": false,
      "label": "sdfg",
      "sequence": 4,
      "rules": [
        18,
        20
      ],
      "value": "dfgh",
      "action": "select"
    },
    {
      "identifier": "dfgh",
      "preventNavigation": false,
      "label": "dfgh",
      "sequence": 5,
      "rules": [
        18
      ],
      "action": "check"
    },
    {
      "identifier": "dfgh",
      "preventNavigation": false,
      "label": "dfgh",
      "sequence": 6,
      "rules": [
        18
      ],
      "action": "uncheck"
    },
    {
      "preventNavigation": true,
      "label": "dfgh",
      "sequence": 7,
      "js": "dfgh",
      "rules": [
        18
      ],
      "action": "execute"
    },
    {
      "preventNavigation": true,
      "seconds": 5,
      "label": "dfgh",
      "sequence": 8,
      "rules": [
        19
      ],
      "action": "watch"
    }
  ]
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "name": {
          "type": "string"
        },
        "state": {
          "type": "string"
        },
        "simulationRunning": {
          "type": "boolean"
        },
        "folderId": {
          "type": "integer"
        },
        "options": {
          "type": "object",
          "properties": {
            "location": {
              "type": "string"
            },
            "browserWidth": {
              "type": "integer"
            },
            "reminders": {
              "type": "boolean"
            },
            "userAgent": {
              "type": "string"
            },
            "loadFlash": {
              "type": "boolean"
            },
            "frequency": {
              "type": "string"
            },
            "alerts": {
              "type": "boolean"
            }
          }
        },
        "id": {
          "type": "integer"
        },
        "createdAt": {
          "type": "string"
        },
        "domainId": {
          "type": "integer"
        },
        "actions": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "url": {
                "type": "string"
              },
              "label": {
                "type": "string"
              },
              "sequence": {
                "type": "integer"
              },
              "rules": {
                "type": "array",
                "items": {
                  "type": "integer"
                }
              },
              "action": {
                "type": "string"
              }
            }
          }
        },
        "nextCheck": {
          "type": "string"
        },
        "userId": {
          "type": "integer"
        },
        "emails": {
          "type": "array",
          "items": {
            "type": "string"
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_web-sims

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/web-sims
````

````http
GET https://app.observepoint.com/api/v2/web-sims HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-sims',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-sims', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/web-sims', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/web-sims', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-sims");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /web-sims`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
Total-Route-Time|header|integer|false|No description
Connect-Time|header|integer|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "array",
      "items": {
        "type": "object",
        "properties": {
          "name": {
            "type": "string"
          },
          "lastCheck": {
            "type": "string"
          },
          "state": {
            "type": "string"
          },
          "simulationRunning": {
            "type": "boolean"
          },
          "folderId": {
            "type": "integer"
          },
          "options": {
            "type": "object",
            "properties": {
              "location": {
                "type": "string"
              },
              "browserWidth": {
                "type": "integer"
              },
              "reminders": {
                "type": "boolean"
              },
              "userAgent": {
                "type": "string"
              },
              "loadFlash": {
                "type": "boolean"
              },
              "frequency": {
                "type": "string"
              },
              "alerts": {
                "type": "boolean"
              }
            }
          },
          "id": {
            "type": "integer"
          },
          "createdAt": {
            "type": "string"
          },
          "domainId": {
            "type": "integer"
          },
          "actions": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {}
            }
          },
          "nextCheck": {
            "type": "string"
          },
          "userId": {
            "type": "integer"
          },
          "emails": {
            "type": "array",
            "items": {
              "type": "string"
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_web-sims

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/web-sims
````

````http
POST https://app.observepoint.com/api/v2/web-sims HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-sims',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-sims', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/web-sims', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/web-sims', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-sims");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /web-sims`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
body|body|object|false|No description

> Body parameter

````json
{
  "name": "stoplight.io",
  "domainId": 280,
  "emails": [
    "MIKE.CATALDO@OBSERVEPOINT.COM"
  ],
  "options": {
    "frequency": "weekly",
    "location": "mountain",
    "userAgent": "Firefox(45.0.1) - Linux",
    "browserWidth": 1367,
    "alerts": true,
    "reminders": false,
    "loadFlash": false
  },
  "actions": [
    {
      "action": "navto",
      "sequence": 0,
      "rules": [
        18
      ],
      "url": "http://stoplight.io",
      "label": "bael"
    },
    {
      "action": "click",
      "sequence": 1,
      "rules": [
        46
      ],
      "url": "http://stoplight.io",
      "label": "rjyy",
      "identifier": "ytj"
    },
    {
      "action": "input",
      "sequence": 2,
      "rules": [
        20,
        45
      ],
      "url": "http://stoplight.io",
      "label": "arg",
      "value": "sdfg",
      "identifier": "sdg"
    },
    {
      "action": "maskedInput",
      "sequence": 3,
      "rules": [
        45,
        46
      ],
      "url": "http://stoplight.io",
      "label": "sdfg",
      "maskedValue": "sdfg",
      "identifier": "sdfg",
      "maskedInputType": "text",
      "viewedValue": "sdfg",
      "isChangedValue": true
    },
    {
      "action": "select",
      "sequence": 4,
      "rules": [
        18,
        20
      ],
      "url": "http://stoplight.io",
      "label": "sdfg",
      "value": "dfgh",
      "identifier": "dfgh"
    },
    {
      "action": "check",
      "sequence": 5,
      "rules": [
        18
      ],
      "url": "http://stoplight.io",
      "label": "dfgh",
      "identifier": "dfgh"
    },
    {
      "action": "uncheck",
      "sequence": 6,
      "rules": [
        18
      ],
      "url": "http://stoplight.io",
      "label": "dfgh",
      "identifier": "dfgh"
    },
    {
      "action": "execute",
      "sequence": 7,
      "rules": [
        18
      ],
      "url": "http://stoplight.io",
      "label": "dfgh",
      "preventNavigation": true,
      "js": "dfgh"
    },
    {
      "action": "watch",
      "sequence": 8,
      "rules": [
        19
      ],
      "url": "http://stoplight.io",
      "label": "dfgh",
      "seconds": 5,
      "preventNavigation": true
    },
    {
      "action": "navto",
      "sequence": 9,
      "rules": [
        18
      ],
      "url": "http://stoplight.io",
      "label": "fdgh"
    }
  ]
}
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "name": {
          "type": "string"
        },
        "state": {
          "type": "string"
        },
        "simulationRunning": {
          "type": "boolean"
        },
        "folderId": {
          "type": "integer"
        },
        "options": {
          "type": "object",
          "properties": {
            "location": {
              "type": "string"
            },
            "browserWidth": {
              "type": "integer"
            },
            "reminders": {
              "type": "boolean"
            },
            "userAgent": {
              "type": "string"
            },
            "loadFlash": {
              "type": "boolean"
            },
            "frequency": {
              "type": "string"
            },
            "alerts": {
              "type": "boolean"
            }
          }
        },
        "id": {
          "type": "integer"
        },
        "createdAt": {
          "type": "string"
        },
        "domainId": {
          "type": "integer"
        },
        "actions": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "url": {
                "type": "string"
              },
              "label": {
                "type": "string"
              },
              "sequence": {
                "type": "integer"
              },
              "rules": {
                "type": "array",
                "items": {
                  "type": "integer"
                }
              },
              "action": {
                "type": "string"
              }
            }
          }
        },
        "nextCheck": {
          "type": "string"
        },
        "userId": {
          "type": "integer"
        },
        "emails": {
          "type": "array",
          "items": {
            "type": "string"
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_web-sims-param1-actions

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/web-sims/{param1}/actions
````

````http
GET https://app.observepoint.com/api/v2/web-sims/{param1}/actions HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-sims/{param1}/actions',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-sims/{param1}/actions', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/web-sims/{param1}/actions', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/web-sims/{param1}/actions', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-sims/{param1}/actions");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /web-sims/{param1}/actions`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {
      "url": "string",
      "label": "string",
      "sequence": 0,
      "rules": [
        0
      ],
      "action": "string"
    }
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_web-sims-param1-runs-param2

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/web-sims/{param1}/runs/{param2}
````

````http
GET https://app.observepoint.com/api/v2/web-sims/{param1}/runs/{param2} HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-sims/{param1}/runs/{param2}',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-sims/{param1}/runs/{param2}', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/web-sims/{param1}/runs/{param2}', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/web-sims/{param1}/runs/{param2}', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-sims/{param1}/runs/{param2}");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /web-sims/{param1}/runs/{param2}`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
param2|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": {
    "completedAt": "string",
    "simulationId": 0,
    "id": 0,
    "status": "string",
    "startedAt": "string"
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_web-sims-param1-runs

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/web-sims/{param1}/runs
````

````http
GET https://app.observepoint.com/api/v2/web-sims/{param1}/runs HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-sims/{param1}/runs',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-sims/{param1}/runs', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/web-sims/{param1}/runs', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/web-sims/{param1}/runs', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-sims/{param1}/runs");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /web-sims/{param1}/runs`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    {
      "completedAt": "string",
      "simulationId": 0,
      "id": 0,
      "status": "string",
      "startedAt": "string"
    }
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## POST_web-sims-param1-runs

> Code samples

````shell
# You can also use wget
curl -X post https://app.observepoint.com/api/v2/web-sims/{param1}/runs
````

````http
POST https://app.observepoint.com/api/v2/web-sims/{param1}/runs HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-sims/{param1}/runs',
    method: 'post',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-sims/{param1}/runs', { method: 'POST'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.post 'https://app.observepoint.com/api/v2/web-sims/{param1}/runs', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.post('https://app.observepoint.com/api/v2/web-sims/{param1}/runs', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-sims/{param1}/runs");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("POST");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`POST /web-sims/{param1}/runs`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "name": {
          "type": "string"
        },
        "lastCheck": {
          "type": "string"
        },
        "state": {
          "type": "string"
        },
        "simulationRunning": {
          "type": "boolean"
        },
        "folderId": {
          "type": "integer"
        },
        "options": {
          "type": "object",
          "properties": {
            "location": {
              "type": "string"
            },
            "browserWidth": {
              "type": "integer"
            },
            "reminders": {
              "type": "boolean"
            },
            "userAgent": {
              "type": "string"
            },
            "loadFlash": {
              "type": "boolean"
            },
            "frequency": {
              "type": "string"
            },
            "alerts": {
              "type": "boolean"
            }
          }
        },
        "id": {
          "type": "integer"
        },
        "createdAt": {
          "type": "string"
        },
        "domainId": {
          "type": "integer"
        },
        "actions": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {}
          }
        },
        "nextCheck": {
          "type": "string"
        },
        "userId": {
          "type": "integer"
        },
        "emails": {
          "type": "array",
          "items": {
            "type": "string"
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_web-sims-param1-rules

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/web-sims/{param1}/rules
````

````http
GET https://app.observepoint.com/api/v2/web-sims/{param1}/rules HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-sims/{param1}/rules',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-sims/{param1}/rules', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/web-sims/{param1}/rules', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/web-sims/{param1}/rules', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-sims/{param1}/rules");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /web-sims/{param1}/rules`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "array",
      "items": {
        "type": "object",
        "properties": {
          "name": {
            "type": "string"
          },
          "updatedAt": {
            "type": "string"
          },
          "tags": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {
                "variables": {
                  "type": "array",
                  "items": {
                    "type": "object",
                    "properties": {}
                  }
                },
                "id": {
                  "type": "integer"
                },
                "condition": {
                  "type": "boolean"
                },
                "tagId": {
                  "type": "integer"
                },
                "ruleId": {
                  "type": "integer"
                }
              }
            }
          },
          "pageFilters": {
            "type": "array",
            "items": {
              "type": "object",
              "properties": {}
            }
          },
          "id": {
            "type": "integer"
          },
          "createdAt": {
            "type": "string"
          },
          "ruleSetId": {
            "type": "integer"
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## PUT_web-sims-param1-rules

> Code samples

````shell
# You can also use wget
curl -X put https://app.observepoint.com/api/v2/web-sims/{param1}/rules
````

````http
PUT https://app.observepoint.com/api/v2/web-sims/{param1}/rules HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-sims/{param1}/rules',
    method: 'put',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-sims/{param1}/rules', { method: 'PUT'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.put 'https://app.observepoint.com/api/v2/web-sims/{param1}/rules', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.put('https://app.observepoint.com/api/v2/web-sims/{param1}/rules', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-sims/{param1}/rules");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("PUT");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`PUT /web-sims/{param1}/rules`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
body|body|object|false|No description

> Body parameter

````json
[
  19,
  20
]
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    0
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>

## GET_web-sims-param1-runs-param2-timeline

> Code samples

````shell
# You can also use wget
curl -X get https://app.observepoint.com/api/v2/web-sims/{param1}/runs/{param2}/timeline
````

````http
GET https://app.observepoint.com/api/v2/web-sims/{param1}/runs/{param2}/timeline HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-sims/{param1}/runs/{param2}/timeline',
    method: 'get',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-sims/{param1}/runs/{param2}/timeline', { method: 'GET'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.get 'https://app.observepoint.com/api/v2/web-sims/{param1}/runs/{param2}/timeline', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.get('https://app.observepoint.com/api/v2/web-sims/{param1}/runs/{param2}/timeline', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-sims/{param1}/runs/{param2}/timeline");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("GET");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`GET /web-sims/{param1}/runs/{param2}/timeline`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
param2|path|integer|true|No description

### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "type": "object",
  "properties": {
    "success": {
      "type": "boolean"
    },
    "data": {
      "type": "object",
      "properties": {
        "actions": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "success": {
                "type": "boolean"
              },
              "simplifiedRuleSetupAllowed": {
                "type": "boolean"
              },
              "timestamp": {
                "type": "integer"
              },
              "actionId": {
                "type": "integer"
              },
              "tags": {
                "type": "array",
                "items": {
                  "type": "object",
                  "properties": {
                    "statusCode": {
                      "type": "integer"
                    },
                    "tag": {
                      "type": "object",
                      "properties": {
                        "id": {
                          "type": "integer"
                        },
                        "name": {
                          "type": "string"
                        },
                        "icon": {
                          "type": "string"
                        },
                        "category": {
                          "type": "object",
                          "properties": {
                            "id": {
                              "type": "integer"
                            },
                            "name": {
                              "type": "string"
                            }
                          }
                        }
                      }
                    },
                    "stoppedAt": {
                      "type": "integer"
                    },
                    "duplicates": {
                      "type": "integer"
                    },
                    "responseAt": {
                      "type": "integer"
                    },
                    "variables": {
                      "type": "object",
                      "properties": {}
                    },
                    "multiples": {
                      "type": "integer"
                    },
                    "invalidVariables": {
                      "type": "array",
                      "items": {
                        "type": "object",
                        "properties": {}
                      }
                    },
                    "version": {
                      "type": "string"
                    },
                    "valid": {
                      "type": "boolean"
                    },
                    "startedAt": {
                      "type": "integer"
                    },
                    "position": {
                      "type": "number"
                    },
                    "account": {
                      "type": "string"
                    }
                  }
                }
              },
              "thumbnail": {
                "type": "string"
              },
              "generatedActions": {
                "type": "array",
                "items": {
                  "type": "object",
                  "properties": {}
                }
              },
              "failures": {
                "type": "array",
                "items": {
                  "type": "object",
                  "properties": {
                    "name": {
                      "type": "string"
                    },
                    "failureType": {
                      "type": "string"
                    },
                    "tag": {
                      "type": "object",
                      "properties": {
                        "id": {
                          "type": "integer"
                        },
                        "name": {
                          "type": "string"
                        },
                        "icon": {
                          "type": "string"
                        },
                        "category": {
                          "type": "object",
                          "properties": {
                            "id": {
                              "type": "integer"
                            },
                            "name": {
                              "type": "string"
                            }
                          }
                        }
                      }
                    },
                    "ruleSnapshotId": {
                      "type": "integer"
                    }
                  }
                }
              },
              "screenshot": {
                "type": "string"
              },
              "action": {
                "type": "object",
                "properties": {
                  "url": {
                    "type": "string"
                  },
                  "action": {
                    "type": "string"
                  },
                  "label": {
                    "type": "string"
                  }
                }
              }
            }
          }
        },
        "ruleFailures": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "name": {
                "type": "string"
              },
              "failureType": {
                "type": "string"
              },
              "tag": {
                "type": "object",
                "properties": {
                  "id": {
                    "type": "integer"
                  },
                  "name": {
                    "type": "string"
                  },
                  "icon": {
                    "type": "string"
                  },
                  "category": {
                    "type": "object",
                    "properties": {
                      "id": {
                        "type": "integer"
                      },
                      "name": {
                        "type": "string"
                      }
                    }
                  }
                }
              },
              "ruleSnapshotId": {
                "type": "integer"
              }
            }
          }
        }
      }
    }
  }
}
````
<aside class="success">
This operation does not require authentication
</aside>

## PUT_web-sims-param1-actions-param2-rules

> Code samples

````shell
# You can also use wget
curl -X put https://app.observepoint.com/api/v2/web-sims/{param1}/actions/{param2}/rules
````

````http
PUT https://app.observepoint.com/api/v2/web-sims/{param1}/actions/{param2}/rules HTTP/1.1
Host: app.observepoint.com
Content-Type: application/json
Accept: application/json
````

````html
<script>
  $.ajax({
    url: 'https://app.observepoint.com/api/v2/web-sims/{param1}/actions/{param2}/rules',
    method: 'put',
    success: function(data) {
      console.log(JSON.stringify(data));
    }
  })
</script>
````

````javascript
const request = require('node-fetch');
fetch('https://app.observepoint.com/api/v2/web-sims/{param1}/actions/{param2}/rules', { method: 'PUT'})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});
````

````ruby
require 'rest-client'
require 'json'

result = RestClient.put 'https://app.observepoint.com/api/v2/web-sims/{param1}/actions/{param2}/rules', params:
  {
    # TODO
  }

p JSON.parse(result)
````

````python
import requests

r = requests.put('https://app.observepoint.com/api/v2/web-sims/{param1}/actions/{param2}/rules', params={
  # TODO
})

print r.json()
````

````java
URL obj = new URL("https://app.observepoint.com/api/v2/web-sims/{param1}/actions/{param2}/rules");
HttpURLConnection con = (HttpURLConnection) obj.openConnection();
con.setRequestMethod("PUT");
int responseCode = con.getResponseCode();
BufferedReader in = new BufferedReader(
    new InputStreamReader(con.getInputStream()));
String inputLine;
StringBuffer response = new StringBuffer();
while ((inputLine = in.readLine()) != null) {
    response.append(inputLine);
}
in.close();
System.out.println(response.toString());
````

`PUT /web-sims/{param1}/actions/{param2}/rules`

### Parameters

Parameter|In|Type|Required|Description
---|---|---|---|---|
param1|path|integer|true|No description
param2|path|string|true|No description
body|body|object|false|No description
Authorization|header|string|false|No description
Content-Type|header|string|false|No description

> Body parameter

````json
[
  165
]
````
### Responses

Status|Meaning|Description
---|---|---|
200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|No description

> Example responses

````json
{
  "success": true,
  "data": [
    0
  ]
}
````
<aside class="success">
This operation does not require authentication
</aside>
