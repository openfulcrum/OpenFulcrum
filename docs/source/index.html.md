---
title: OpenFulcrum 0.1
language_tabs:
  - shell: Shell
  - http: HTTP
  - javascript: JavaScript
  - javascript--nodejs: Node.JS
 

toc_footers:
  - >-
 
includes: []
search: true
highlight_theme: darkula
headingLevel: 2

---

<h1 id="OpenFulcrum">The OpenFulcrum API</h1>

> Scroll down for code samples, example requests and responses. Select a language for code samples from the tabs above or the mobile navigation menu.

OpenFulcrum is a set of open APIs for financial products. 

<h1 id="OpenFulcrum-openinvest">OpenInvest</h1>

Open APIs for investment


> Installation

```shell
# install with npm
npm install openinvest

```

## ReadISA

<a id="readISA"></a>

> Code samples

```shell
# You can also use wget
curl -X POST http://petstore.swagger.io/v2/pet \
  -H 'Content-Type: application/json' \
  -H 'Authorization: Bearer {access-token}'

```

```http
POST http://petstore.swagger.io/v2/pet HTTP/1.1
Host: petstore.swagger.io
Content-Type: application/json

```

```javascript
var headers = {
  'Content-Type':'application/json',
  'Authorization':'Bearer {access-token}'

};

$.ajax({
  url: 'http://petstore.swagger.io/v2/pet',
  method: 'post',

  headers: headers,
  success: function(data) {
    console.log(JSON.stringify(data));
  }
})

```

```javascript--nodejs
const request = require('node-fetch');
const inputBody = '{
  "id": 0,
  "category": {
    "id": 0,
    "name": "string"
  },
  "name": "doggie",
  "photoUrls": [
    "string"
  ],
  "tags": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "status": "available"
}';
const headers = {
  'Content-Type':'application/json',
  'Authorization':'Bearer {access-token}'

};

fetch('http://petstore.swagger.io/v2/pet',
{
  method: 'POST',
  body: inputBody,
  headers: headers
})
.then(function(res) {
    return res.json();
}).then(function(body) {
    console.log(body);
});

```

`POST /readISA`

*Get list of ISAs*

> Body parameter

```json
{
  "id": 0,
  "category": {
    "id": 0,
    "name": "string"
  },
  "name": "doggie",
  "photoUrls": [
    "string"
  ],
  "tags": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "status": "available"
}
```


<h1 id="OpenFulcrum-OpenPension">OpenPension</h1>

Coming soon...

> OpenPension coming soon


<h1 id="OpenFulcrum-OpenInsurance">OpenInsurance</h1>

Coming soon...


> OpenInsurance coming soon

