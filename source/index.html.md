---
title: EMS Api v1
language_tabs:
  - csharp: C#
  - python: Python
  - javascript: JavaScript
  - http: HTTP
  - java: Java
language_clients:
  - csharp: ""
  - python: ""
  - javascript: ""
  - http: ""
  - java: ""
toc_footers: []
includes: []
search: false
highlight_theme: darkula
headingLevel: 2

---

<!-- Generator: Widdershins v4.0.1 -->

<h1 id="ems-api">EMS Api v1</h1>

> Scroll down for code samples, example requests and responses. Select a language for code samples from the tabs above or the mobile navigation menu.

# Authentication

- HTTP Authentication, scheme: Basic Login

* API Key (Bearer)
    - Parameter Name: **Authorization**, in: header. JWT Authorization header using the Bearer scheme.

<h1 id="ems-api-account">Account</h1>

## get__account_login

> Code samples

```csharp
var client = new RestClient("https://example.com/account/login");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/account/login", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/account/login");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /account/login HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/account/login")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /account/login`

<h3 id="get__account_login-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|returnUrl|query|string|false|none|

<h3 id="get__account_login-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__account_login

> Code samples

```csharp
var client = new RestClient("https://example.com/account/login");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/account/login", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/account/login");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /account/login HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/account/login")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /account/login`

<h3 id="post__account_login-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Email|query|string|false|none|
|Password|query|string|false|none|
|RememberMe|query|boolean|false|none|
|Errors|query|array[string]|false|none|
|Message|query|string|false|none|
|returnUrl|query|string|false|none|

<h3 id="post__account_login-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__account_register

> Code samples

```csharp
var client = new RestClient("https://example.com/account/register");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/account/register", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/account/register");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /account/register HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/account/register")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /account/register`

<h3 id="get__account_register-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|returnUrl|query|string|false|none|

<h3 id="get__account_register-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__account_register

> Code samples

```csharp
var client = new RestClient("https://example.com/account/register");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/account/register", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/account/register");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /account/register HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/account/register")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /account/register`

<h3 id="post__account_register-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Email|query|string|false|none|
|Password|query|string|false|none|
|ConfirmPassword|query|string|false|none|
|returnUrl|query|string|false|none|

<h3 id="post__account_register-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__account_logoff

> Code samples

```csharp
var client = new RestClient("https://example.com/account/logoff");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/account/logoff", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/account/logoff");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /account/logoff HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/account/logoff")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /account/logoff`

<h3 id="post__account_logoff-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__account_externalLogin

> Code samples

```csharp
var client = new RestClient("https://example.com/account/externalLogin");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/account/externalLogin", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/account/externalLogin");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /account/externalLogin HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/account/externalLogin")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /account/externalLogin`

<h3 id="post__account_externallogin-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|provider|query|string|false|none|
|returnUrl|query|string|false|none|

<h3 id="post__account_externallogin-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__account_ExternalLoginCallback

> Code samples

```csharp
var client = new RestClient("https://example.com/account/ExternalLoginCallback");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/account/ExternalLoginCallback", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/account/ExternalLoginCallback");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /account/ExternalLoginCallback HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/account/ExternalLoginCallback")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /account/ExternalLoginCallback`

<h3 id="get__account_externallogincallback-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|returnUrl|query|string|false|none|

<h3 id="get__account_externallogincallback-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__account_ExternalLoginConfirmation

> Code samples

```csharp
var client = new RestClient("https://example.com/account/ExternalLoginConfirmation");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/account/ExternalLoginConfirmation", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/account/ExternalLoginConfirmation");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /account/ExternalLoginConfirmation HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/account/ExternalLoginConfirmation")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /account/ExternalLoginConfirmation`

<h3 id="post__account_externalloginconfirmation-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Email|query|string|false|none|
|returnUrl|query|string|false|none|

<h3 id="post__account_externalloginconfirmation-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__account_ConfirmEmail

> Code samples

```csharp
var client = new RestClient("https://example.com/account/ConfirmEmail");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/account/ConfirmEmail", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/account/ConfirmEmail");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /account/ConfirmEmail HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/account/ConfirmEmail")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /account/ConfirmEmail`

<h3 id="get__account_confirmemail-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|userId|query|string|false|none|
|code|query|string|false|none|

<h3 id="get__account_confirmemail-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__account_ForgotPassword

> Code samples

```csharp
var client = new RestClient("https://example.com/account/ForgotPassword");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/account/ForgotPassword", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/account/ForgotPassword");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /account/ForgotPassword HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/account/ForgotPassword")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /account/ForgotPassword`

<h3 id="get__account_forgotpassword-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__account_ForgotPassword

> Code samples

```csharp
var client = new RestClient("https://example.com/account/ForgotPassword");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/account/ForgotPassword", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/account/ForgotPassword");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /account/ForgotPassword HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/account/ForgotPassword")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /account/ForgotPassword`

<h3 id="post__account_forgotpassword-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Email|query|string|false|none|

<h3 id="post__account_forgotpassword-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__account_ForgotPasswordConfirmation

> Code samples

```csharp
var client = new RestClient("https://example.com/account/ForgotPasswordConfirmation");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/account/ForgotPasswordConfirmation", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/account/ForgotPasswordConfirmation");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /account/ForgotPasswordConfirmation HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/account/ForgotPasswordConfirmation")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /account/ForgotPasswordConfirmation`

<h3 id="get__account_forgotpasswordconfirmation-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__account_ResetPassword

> Code samples

```csharp
var client = new RestClient("https://example.com/account/ResetPassword");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/account/ResetPassword", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/account/ResetPassword");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /account/ResetPassword HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/account/ResetPassword")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /account/ResetPassword`

<h3 id="get__account_resetpassword-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|code|query|string|false|none|

<h3 id="get__account_resetpassword-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__account_ResetPassword

> Code samples

```csharp
var client = new RestClient("https://example.com/account/ResetPassword");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/account/ResetPassword", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/account/ResetPassword");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /account/ResetPassword HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/account/ResetPassword")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /account/ResetPassword`

<h3 id="post__account_resetpassword-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Email|query|string|false|none|
|Password|query|string|false|none|
|ConfirmPassword|query|string|false|none|
|Code|query|string|false|none|

<h3 id="post__account_resetpassword-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__account_ResetPasswordConfirmation

> Code samples

```csharp
var client = new RestClient("https://example.com/account/ResetPasswordConfirmation");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/account/ResetPasswordConfirmation", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/account/ResetPasswordConfirmation");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /account/ResetPasswordConfirmation HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/account/ResetPasswordConfirmation")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /account/ResetPasswordConfirmation`

<h3 id="get__account_resetpasswordconfirmation-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__account_SendCode

> Code samples

```csharp
var client = new RestClient("https://example.com/account/SendCode");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/account/SendCode", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/account/SendCode");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /account/SendCode HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/account/SendCode")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /account/SendCode`

<h3 id="get__account_sendcode-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|returnUrl|query|string|false|none|
|rememberMe|query|boolean|false|none|

<h3 id="get__account_sendcode-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__account_SendCode

> Code samples

```csharp
var client = new RestClient("https://example.com/account/SendCode");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/account/SendCode", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/account/SendCode");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /account/SendCode HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/account/SendCode")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /account/SendCode`

<h3 id="post__account_sendcode-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Providers|query|array[object]|false|none|
|SelectedProvider|query|string|false|none|
|ReturnUrl|query|string|false|none|
|RememberMe|query|boolean|false|none|

<h3 id="post__account_sendcode-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__account_VerifyCode

> Code samples

```csharp
var client = new RestClient("https://example.com/account/VerifyCode");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/account/VerifyCode", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/account/VerifyCode");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /account/VerifyCode HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/account/VerifyCode")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /account/VerifyCode`

<h3 id="get__account_verifycode-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|provider|query|string|false|none|
|rememberMe|query|boolean|false|none|
|returnUrl|query|string|false|none|

<h3 id="get__account_verifycode-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__account_VerifyCode

> Code samples

```csharp
var client = new RestClient("https://example.com/account/VerifyCode");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/account/VerifyCode", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/account/VerifyCode");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /account/VerifyCode HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/account/VerifyCode")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /account/VerifyCode`

<h3 id="post__account_verifycode-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Provider|query|string|false|none|
|ReturnUrl|query|string|false|none|
|RememberMe|query|boolean|false|none|
|RememberBrowser|query|boolean|false|none|
|Code|query|string|false|none|

<h3 id="post__account_verifycode-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-addon">Addon</h1>

## post__api_Addon_purchase

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Addon/purchase");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"workspaceId\":\"string\",\"addonId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"workspaceId\":\"string\",\"addonId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Addon/purchase", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"workspaceId\":\"string\",\"addonId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Addon/purchase");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Addon/purchase HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 43

{"workspaceId":"string","addonId":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Addon/purchase")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"workspaceId\":\"string\",\"addonId\":\"string\"}")
  .asString();
```

`POST /api/Addon/purchase`

> Body parameter

```json
{
  "workspaceId": "string",
  "addonId": "string"
}
```

<h3 id="post__api_addon_purchase-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[PurchaseAddonDto](#schemapurchaseaddondto)|false|none|

<h3 id="post__api_addon_purchase-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Addon_isInvoicePaid

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Addon/isInvoicePaid");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"workspaceId\":\"string\",\"invoiceId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"workspaceId\":\"string\",\"invoiceId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Addon/isInvoicePaid", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"workspaceId\":\"string\",\"invoiceId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Addon/isInvoicePaid");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Addon/isInvoicePaid HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 45

{"workspaceId":"string","invoiceId":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Addon/isInvoicePaid")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"workspaceId\":\"string\",\"invoiceId\":\"string\"}")
  .asString();
```

`POST /api/Addon/isInvoicePaid`

> Body parameter

```json
{
  "workspaceId": "string",
  "invoiceId": "string"
}
```

<h3 id="post__api_addon_isinvoicepaid-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[InvoiceStatusDto](#schemainvoicestatusdto)|false|none|

<h3 id="post__api_addon_isinvoicepaid-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-agenda">Agenda</h1>

## get__api_event_{eventIdOrSlug}_agenda

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/agenda");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/event/string/agenda", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/event/string/agenda");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/event/string/agenda HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/event/string/agenda")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/event/{eventIdOrSlug}/agenda`

<h3 id="get__api_event_{eventidorslug}_agenda-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|

<h3 id="get__api_event_{eventidorslug}_agenda-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_event_{eventIdOrSlug}_agenda_{agendaId}_track

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/agenda/string/track");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"title\":\"string\",\"headerBackgroundColor\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"title\":\"string\",\"headerBackgroundColor\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/event/string/agenda/string/track", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"title\":\"string\",\"headerBackgroundColor\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/event/string/agenda/string/track");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/event/string/agenda/string/track HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 51

{"title":"string","headerBackgroundColor":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/event/string/agenda/string/track")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"title\":\"string\",\"headerBackgroundColor\":\"string\"}")
  .asString();
```

`POST /api/event/{eventIdOrSlug}/agenda/{agendaId}/track`

> Body parameter

```json
{
  "title": "string",
  "headerBackgroundColor": "string"
}
```

<h3 id="post__api_event_{eventidorslug}_agenda_{agendaid}_track-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|
|agendaId|path|string|true|none|
|body|body|[AddTrackRequest](#schemaaddtrackrequest)|false|none|

<h3 id="post__api_event_{eventidorslug}_agenda_{agendaid}_track-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_event_{eventIdOrSlug}_agenda_{agendaId}_track

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/agenda/string/track");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"title\":\"string\",\"headerBackgroundColor\":\"string\",\"id\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"title\":\"string\",\"headerBackgroundColor\":\"string\",\"id\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/event/string/agenda/string/track", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"title\":\"string\",\"headerBackgroundColor\":\"string\",\"id\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/event/string/agenda/string/track");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/event/string/agenda/string/track HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 65

{"title":"string","headerBackgroundColor":"string","id":"string"}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/event/string/agenda/string/track")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"title\":\"string\",\"headerBackgroundColor\":\"string\",\"id\":\"string\"}")
  .asString();
```

`PUT /api/event/{eventIdOrSlug}/agenda/{agendaId}/track`

> Body parameter

```json
{
  "title": "string",
  "headerBackgroundColor": "string",
  "id": "string"
}
```

<h3 id="put__api_event_{eventidorslug}_agenda_{agendaid}_track-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|
|agendaId|path|string|true|none|
|body|body|[UpdateTrackRequest](#schemaupdatetrackrequest)|false|none|

<h3 id="put__api_event_{eventidorslug}_agenda_{agendaid}_track-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_event_{eventIdOrSlug}_agenda_{agendaId}_track_{trackId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/agenda/string/track/string");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("DELETE", "/api/event/string/agenda/string/track/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/event/string/agenda/string/track/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/event/string/agenda/string/track/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/event/string/agenda/string/track/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`DELETE /api/event/{eventIdOrSlug}/agenda/{agendaId}/track/{trackId}`

<h3 id="delete__api_event_{eventidorslug}_agenda_{agendaid}_track_{trackid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|
|agendaId|path|string|true|none|
|trackId|path|string|true|none|

<h3 id="delete__api_event_{eventidorslug}_agenda_{agendaid}_track_{trackid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_event_{eventIdOrSlug}_agenda_{agendaId}_session

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/agenda/string/session");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"title\":\"string\",\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\",\"trackId\":\"string\",\"description\":\"string\",\"speakerIds\":[\"string\"],\"stageStream\":{\"type\":0,\"url\":\"string\",\"hostUrl\":\"string\",\"additionalUrls\":[{\"type\":0,\"url\":\"string\"}],\"rtmpSettings\":{\"streamKey\":\"string\",\"channelArn\":\"string\",\"recordings\":[\"string\"]},\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\"}},\"groupIds\":[\"string\"],\"isStreamTypeChangeForced\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"title\":\"string\",\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\",\"trackId\":\"string\",\"description\":\"string\",\"speakerIds\":[\"string\"],\"stageStream\":{\"type\":0,\"url\":\"string\",\"hostUrl\":\"string\",\"additionalUrls\":[{\"type\":0,\"url\":\"string\"}],\"rtmpSettings\":{\"streamKey\":\"string\",\"channelArn\":\"string\",\"recordings\":[\"string\"]},\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\"}},\"groupIds\":[\"string\"],\"isStreamTypeChangeForced\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/event/string/agenda/string/session", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"title\":\"string\",\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\",\"trackId\":\"string\",\"description\":\"string\",\"speakerIds\":[\"string\"],\"stageStream\":{\"type\":0,\"url\":\"string\",\"hostUrl\":\"string\",\"additionalUrls\":[{\"type\":0,\"url\":\"string\"}],\"rtmpSettings\":{\"streamKey\":\"string\",\"channelArn\":\"string\",\"recordings\":[\"string\"]},\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\"}},\"groupIds\":[\"string\"],\"isStreamTypeChangeForced\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/event/string/agenda/string/session");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/event/string/agenda/string/session HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 939

{"title":"string","startDate":"2019-08-24T14:15:22Z","endDate":"2019-08-24T14:15:22Z","trackId":"string","description":"string","speakerIds":["string"],"stageStream":{"type":0,"url":"string","hostUrl":"string","additionalUrls":[{"type":0,"url":"string"}],"rtmpSettings":{"streamKey":"string","channelArn":"string","recordings":["string"]},"settings":{"host":{"isChatEnabled":true,"isPeopleEnabled":true,"isLeaveButtonEnabled":true,"isRecordingEnabled":true,"isScreenShareEnabled":true,"isBackgroundEnabled":true,"isVideoEnabled":true,"isAudioEnabled":true,"isBreakoutEnabled":true},"stream":{"isChatEnabled":true,"isPeopleEnabled":true,"isLeaveButtonEnabled":true,"isRecordingEnabled":true,"isScreenShareEnabled":true,"isBackgroundEnabled":true,"isVideoEnabled":true,"isAudioEnabled":true,"isBreakoutEnabled":true},"startDate":"2019-08-24T14:15:22Z","endDate":"2019-08-24T14:15:22Z"}},"groupIds":["string"],"isStreamTypeChangeForced":true}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/event/string/agenda/string/session")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"title\":\"string\",\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\",\"trackId\":\"string\",\"description\":\"string\",\"speakerIds\":[\"string\"],\"stageStream\":{\"type\":0,\"url\":\"string\",\"hostUrl\":\"string\",\"additionalUrls\":[{\"type\":0,\"url\":\"string\"}],\"rtmpSettings\":{\"streamKey\":\"string\",\"channelArn\":\"string\",\"recordings\":[\"string\"]},\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\"}},\"groupIds\":[\"string\"],\"isStreamTypeChangeForced\":true}")
  .asString();
```

`POST /api/event/{eventIdOrSlug}/agenda/{agendaId}/session`

> Body parameter

```json
{
  "title": "string",
  "startDate": "2019-08-24T14:15:22Z",
  "endDate": "2019-08-24T14:15:22Z",
  "trackId": "string",
  "description": "string",
  "speakerIds": [
    "string"
  ],
  "stageStream": {
    "type": 0,
    "url": "string",
    "hostUrl": "string",
    "additionalUrls": [
      {
        "type": 0,
        "url": "string"
      }
    ],
    "rtmpSettings": {
      "streamKey": "string",
      "channelArn": "string",
      "recordings": [
        "string"
      ]
    },
    "settings": {
      "host": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      },
      "stream": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      },
      "startDate": "2019-08-24T14:15:22Z",
      "endDate": "2019-08-24T14:15:22Z"
    }
  },
  "groupIds": [
    "string"
  ],
  "isStreamTypeChangeForced": true
}
```

<h3 id="post__api_event_{eventidorslug}_agenda_{agendaid}_session-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|
|agendaId|path|string|true|none|
|body|body|[AddSessionRequest](#schemaaddsessionrequest)|false|none|

<h3 id="post__api_event_{eventidorslug}_agenda_{agendaid}_session-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_event_{eventIdOrSlug}_agenda_{agendaId}_session

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/agenda/string/session");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"title\":\"string\",\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\",\"trackId\":\"string\",\"description\":\"string\",\"speakerIds\":[\"string\"],\"stageStream\":{\"type\":0,\"url\":\"string\",\"hostUrl\":\"string\",\"additionalUrls\":[{\"type\":0,\"url\":\"string\"}],\"rtmpSettings\":{\"streamKey\":\"string\",\"channelArn\":\"string\",\"recordings\":[\"string\"]},\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\"}},\"groupIds\":[\"string\"],\"isStreamTypeChangeForced\":true,\"id\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"title\":\"string\",\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\",\"trackId\":\"string\",\"description\":\"string\",\"speakerIds\":[\"string\"],\"stageStream\":{\"type\":0,\"url\":\"string\",\"hostUrl\":\"string\",\"additionalUrls\":[{\"type\":0,\"url\":\"string\"}],\"rtmpSettings\":{\"streamKey\":\"string\",\"channelArn\":\"string\",\"recordings\":[\"string\"]},\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\"}},\"groupIds\":[\"string\"],\"isStreamTypeChangeForced\":true,\"id\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/event/string/agenda/string/session", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"title\":\"string\",\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\",\"trackId\":\"string\",\"description\":\"string\",\"speakerIds\":[\"string\"],\"stageStream\":{\"type\":0,\"url\":\"string\",\"hostUrl\":\"string\",\"additionalUrls\":[{\"type\":0,\"url\":\"string\"}],\"rtmpSettings\":{\"streamKey\":\"string\",\"channelArn\":\"string\",\"recordings\":[\"string\"]},\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\"}},\"groupIds\":[\"string\"],\"isStreamTypeChangeForced\":true,\"id\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/event/string/agenda/string/session");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/event/string/agenda/string/session HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 953

{"title":"string","startDate":"2019-08-24T14:15:22Z","endDate":"2019-08-24T14:15:22Z","trackId":"string","description":"string","speakerIds":["string"],"stageStream":{"type":0,"url":"string","hostUrl":"string","additionalUrls":[{"type":0,"url":"string"}],"rtmpSettings":{"streamKey":"string","channelArn":"string","recordings":["string"]},"settings":{"host":{"isChatEnabled":true,"isPeopleEnabled":true,"isLeaveButtonEnabled":true,"isRecordingEnabled":true,"isScreenShareEnabled":true,"isBackgroundEnabled":true,"isVideoEnabled":true,"isAudioEnabled":true,"isBreakoutEnabled":true},"stream":{"isChatEnabled":true,"isPeopleEnabled":true,"isLeaveButtonEnabled":true,"isRecordingEnabled":true,"isScreenShareEnabled":true,"isBackgroundEnabled":true,"isVideoEnabled":true,"isAudioEnabled":true,"isBreakoutEnabled":true},"startDate":"2019-08-24T14:15:22Z","endDate":"2019-08-24T14:15:22Z"}},"groupIds":["string"],"isStreamTypeChangeForced":true,"id":"string"}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/event/string/agenda/string/session")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"title\":\"string\",\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\",\"trackId\":\"string\",\"description\":\"string\",\"speakerIds\":[\"string\"],\"stageStream\":{\"type\":0,\"url\":\"string\",\"hostUrl\":\"string\",\"additionalUrls\":[{\"type\":0,\"url\":\"string\"}],\"rtmpSettings\":{\"streamKey\":\"string\",\"channelArn\":\"string\",\"recordings\":[\"string\"]},\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\"}},\"groupIds\":[\"string\"],\"isStreamTypeChangeForced\":true,\"id\":\"string\"}")
  .asString();
```

`PUT /api/event/{eventIdOrSlug}/agenda/{agendaId}/session`

> Body parameter

```json
{
  "title": "string",
  "startDate": "2019-08-24T14:15:22Z",
  "endDate": "2019-08-24T14:15:22Z",
  "trackId": "string",
  "description": "string",
  "speakerIds": [
    "string"
  ],
  "stageStream": {
    "type": 0,
    "url": "string",
    "hostUrl": "string",
    "additionalUrls": [
      {
        "type": 0,
        "url": "string"
      }
    ],
    "rtmpSettings": {
      "streamKey": "string",
      "channelArn": "string",
      "recordings": [
        "string"
      ]
    },
    "settings": {
      "host": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      },
      "stream": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      },
      "startDate": "2019-08-24T14:15:22Z",
      "endDate": "2019-08-24T14:15:22Z"
    }
  },
  "groupIds": [
    "string"
  ],
  "isStreamTypeChangeForced": true,
  "id": "string"
}
```

<h3 id="put__api_event_{eventidorslug}_agenda_{agendaid}_session-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|
|agendaId|path|string|true|none|
|body|body|[UpdateSessionRequest](#schemaupdatesessionrequest)|false|none|

<h3 id="put__api_event_{eventidorslug}_agenda_{agendaid}_session-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_event_{eventIdOrSlug}_agenda_{agendaId}_session_{sessionId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/agenda/string/session/string");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("DELETE", "/api/event/string/agenda/string/session/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/event/string/agenda/string/session/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/event/string/agenda/string/session/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/event/string/agenda/string/session/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`DELETE /api/event/{eventIdOrSlug}/agenda/{agendaId}/session/{sessionId}`

<h3 id="delete__api_event_{eventidorslug}_agenda_{agendaid}_session_{sessionid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|
|agendaId|path|string|true|none|
|sessionId|path|string|true|none|

<h3 id="delete__api_event_{eventidorslug}_agenda_{agendaid}_session_{sessionid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-asset">Asset</h1>

## get__api_Asset_{key}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Asset/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Asset/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Asset/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Asset/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Asset/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Asset/{key}`

<h3 id="get__api_asset_{key}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|key|path|string|true|none|
|isDownload|query|boolean|false|none|
|size|query|string|false|none|

<h3 id="get__api_asset_{key}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-auth">Auth</h1>

## post__api_Auth_register

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Auth/register");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"email\":\"user@example.com\",\"password\":\"string\",\"name\":\"string\",\"lastName\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"email\":\"user@example.com\",\"password\":\"string\",\"name\":\"string\",\"lastName\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Auth/register", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"email\":\"user@example.com\",\"password\":\"string\",\"name\":\"string\",\"lastName\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Auth/register");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Auth/register HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 84

{"email":"user@example.com","password":"string","name":"string","lastName":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Auth/register")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"email\":\"user@example.com\",\"password\":\"string\",\"name\":\"string\",\"lastName\":\"string\"}")
  .asString();
```

`POST /api/Auth/register`

> Body parameter

```json
{
  "email": "user@example.com",
  "password": "string",
  "name": "string",
  "lastName": "string"
}
```

<h3 id="post__api_auth_register-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[RegisterUserDto](#schemaregisteruserdto)|false|none|

<h3 id="post__api_auth_register-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Auth_login

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Auth/login");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"userName\":\"string\",\"password\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"userName\":\"string\",\"password\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Auth/login", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"userName\":\"string\",\"password\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Auth/login");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Auth/login HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 41

{"userName":"string","password":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Auth/login")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"userName\":\"string\",\"password\":\"string\"}")
  .asString();
```

`POST /api/Auth/login`

> Body parameter

```json
{
  "userName": "string",
  "password": "string"
}
```

<h3 id="post__api_auth_login-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[LoginUserDto](#schemaloginuserdto)|false|none|

<h3 id="post__api_auth_login-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Auth_sendResetPassword

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Auth/sendResetPassword");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"email\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"email\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Auth/sendResetPassword", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"email\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Auth/sendResetPassword");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Auth/sendResetPassword HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 18

{"email":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Auth/sendResetPassword")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"email\":\"string\"}")
  .asString();
```

`POST /api/Auth/sendResetPassword`

> Body parameter

```json
{
  "email": "string"
}
```

<h3 id="post__api_auth_sendresetpassword-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[SendResetPasswordDto](#schemasendresetpassworddto)|false|none|

<h3 id="post__api_auth_sendresetpassword-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Auth_resetPassword

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Auth/resetPassword");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"userId\":\"string\",\"token\":\"string\",\"newPassword\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"userId\":\"string\",\"token\":\"string\",\"newPassword\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Auth/resetPassword", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"userId\":\"string\",\"token\":\"string\",\"newPassword\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Auth/resetPassword");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Auth/resetPassword HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 59

{"userId":"string","token":"string","newPassword":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Auth/resetPassword")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"userId\":\"string\",\"token\":\"string\",\"newPassword\":\"string\"}")
  .asString();
```

`POST /api/Auth/resetPassword`

> Body parameter

```json
{
  "userId": "string",
  "token": "string",
  "newPassword": "string"
}
```

<h3 id="post__api_auth_resetpassword-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[ResetPasswordDto](#schemaresetpassworddto)|false|none|

<h3 id="post__api_auth_resetpassword-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Auth_validateResetToken

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Auth/validateResetToken");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"userId\":\"string\",\"token\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"userId\":\"string\",\"token\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Auth/validateResetToken", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"userId\":\"string\",\"token\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Auth/validateResetToken");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Auth/validateResetToken HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 36

{"userId":"string","token":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Auth/validateResetToken")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"userId\":\"string\",\"token\":\"string\"}")
  .asString();
```

`POST /api/Auth/validateResetToken`

> Body parameter

```json
{
  "userId": "string",
  "token": "string"
}
```

<h3 id="post__api_auth_validateresettoken-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[ValidateResetPasswordTokenRequest](#schemavalidateresetpasswordtokenrequest)|false|none|

<h3 id="post__api_auth_validateresettoken-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Auth_sign-up

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Auth/sign-up");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"username\":\"user@example.com\",\"password\":\"string\",\"conditionsAccepted\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"username\":\"user@example.com\",\"password\":\"string\",\"conditionsAccepted\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Auth/sign-up", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"username\":\"user@example.com\",\"password\":\"string\",\"conditionsAccepted\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Auth/sign-up");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Auth/sign-up HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 77

{"username":"user@example.com","password":"string","conditionsAccepted":true}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Auth/sign-up")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"username\":\"user@example.com\",\"password\":\"string\",\"conditionsAccepted\":true}")
  .asString();
```

`POST /api/Auth/sign-up`

> Body parameter

```json
{
  "username": "user@example.com",
  "password": "string",
  "conditionsAccepted": true
}
```

<h3 id="post__api_auth_sign-up-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[SignUpDto](#schemasignupdto)|false|none|

<h3 id="post__api_auth_sign-up-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Auth_sign-up_confirm_{confirmationId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Auth/sign-up/confirm/string");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/api/Auth/sign-up/confirm/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Auth/sign-up/confirm/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Auth/sign-up/confirm/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Auth/sign-up/confirm/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /api/Auth/sign-up/confirm/{confirmationId}`

<h3 id="post__api_auth_sign-up_confirm_{confirmationid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|confirmationId|path|string|true|none|

<h3 id="post__api_auth_sign-up_confirm_{confirmationid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Auth_sign-up_confirm_resend

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Auth/sign-up/confirm/resend");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"username\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"username\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Auth/sign-up/confirm/resend", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"username\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Auth/sign-up/confirm/resend");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Auth/sign-up/confirm/resend HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 21

{"username":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Auth/sign-up/confirm/resend")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"username\":\"string\"}")
  .asString();
```

`POST /api/Auth/sign-up/confirm/resend`

> Body parameter

```json
{
  "username": "string"
}
```

<h3 id="post__api_auth_sign-up_confirm_resend-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[ResendEmailDto](#schemaresendemaildto)|false|none|

<h3 id="post__api_auth_sign-up_confirm_resend-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-authorization">Authorization</h1>

## get__connect_authorize

> Code samples

```csharp
var client = new RestClient("https://example.com/connect/authorize");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/connect/authorize", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/connect/authorize");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /connect/authorize HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/connect/authorize")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /connect/authorize`

<h3 id="get__connect_authorize-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__connect_authorize

> Code samples

```csharp
var client = new RestClient("https://example.com/connect/authorize");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/connect/authorize", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/connect/authorize");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /connect/authorize HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/connect/authorize")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /connect/authorize`

<h3 id="post__connect_authorize-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__connect_logout

> Code samples

```csharp
var client = new RestClient("https://example.com/connect/logout");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/connect/logout", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/connect/logout");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /connect/logout HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/connect/logout")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /connect/logout`

<h3 id="get__connect_logout-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__connect_logout

> Code samples

```csharp
var client = new RestClient("https://example.com/connect/logout");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/connect/logout", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/connect/logout");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /connect/logout HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/connect/logout")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /connect/logout`

<h3 id="post__connect_logout-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__connect_token

> Code samples

```csharp
var client = new RestClient("https://example.com/connect/token");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/connect/token", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/connect/token");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /connect/token HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/connect/token")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /connect/token`

<h3 id="post__connect_token-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-billing">Billing</h1>

## get__api_Billing_{workspaceIdOrSlug}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Billing/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Billing/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Billing/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Billing/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Billing/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Billing/{workspaceIdOrSlug}`

<h3 id="get__api_billing_{workspaceidorslug}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|workspaceIdOrSlug|path|string|true|none|

<h3 id="get__api_billing_{workspaceidorslug}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Billing_{workspaceIdOrSlug}_history

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Billing/string/history");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Billing/string/history", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Billing/string/history");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Billing/string/history HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Billing/string/history")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Billing/{workspaceIdOrSlug}/history`

<h3 id="get__api_billing_{workspaceidorslug}_history-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|workspaceIdOrSlug|path|string|true|none|

<h3 id="get__api_billing_{workspaceidorslug}_history-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Billing_{workspaceIdOrSlug}_pdf_{invoiceId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Billing/string/pdf/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Billing/string/pdf/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Billing/string/pdf/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Billing/string/pdf/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Billing/string/pdf/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Billing/{workspaceIdOrSlug}/pdf/{invoiceId}`

<h3 id="get__api_billing_{workspaceidorslug}_pdf_{invoiceid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|workspaceIdOrSlug|path|string|true|none|
|invoiceId|path|string|true|none|

<h3 id="get__api_billing_{workspaceidorslug}_pdf_{invoiceid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-changelogitem">ChangeLogItem</h1>

## get__api_change-log

> Code samples

```csharp
var client = new RestClient("https://example.com/api/change-log");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/change-log", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/change-log");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/change-log HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/change-log")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/change-log`

<h3 id="get__api_change-log-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_change-log

> Code samples

```csharp
var client = new RestClient("https://example.com/api/change-log");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"title\":\"string\",\"description\":\"string\",\"notificationDate\":\"2019-08-24T14:15:22Z\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"updatedOn\":\"2019-08-24T14:15:22Z\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"title\":\"string\",\"description\":\"string\",\"notificationDate\":\"2019-08-24T14:15:22Z\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"updatedOn\":\"2019-08-24T14:15:22Z\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/change-log", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"title\":\"string\",\"description\":\"string\",\"notificationDate\":\"2019-08-24T14:15:22Z\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"updatedOn\":\"2019-08-24T14:15:22Z\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/change-log");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/change-log HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 167

{"id":"string","title":"string","description":"string","notificationDate":"2019-08-24T14:15:22Z","createdOn":"2019-08-24T14:15:22Z","updatedOn":"2019-08-24T14:15:22Z"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/change-log")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"title\":\"string\",\"description\":\"string\",\"notificationDate\":\"2019-08-24T14:15:22Z\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"updatedOn\":\"2019-08-24T14:15:22Z\"}")
  .asString();
```

`POST /api/change-log`

> Body parameter

```json
{
  "id": "string",
  "title": "string",
  "description": "string",
  "notificationDate": "2019-08-24T14:15:22Z",
  "createdOn": "2019-08-24T14:15:22Z",
  "updatedOn": "2019-08-24T14:15:22Z"
}
```

<h3 id="post__api_change-log-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[ChangeLogItemDto](#schemachangelogitemdto)|false|none|

<h3 id="post__api_change-log-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_change-log

> Code samples

```csharp
var client = new RestClient("https://example.com/api/change-log");
var request = new RestRequest(Method.PUT);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("PUT", "/api/change-log", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/change-log");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/change-log HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/change-log")
  .header("Authorization", "API_KEY")
  .asString();
```

`PUT /api/change-log`

<h3 id="put__api_change-log-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|date|query|string|false|none|

<h3 id="put__api_change-log-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_change-log_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/change-log/string");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("DELETE", "/api/change-log/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/change-log/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/change-log/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/change-log/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`DELETE /api/change-log/{entryId}`

<h3 id="delete__api_change-log_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|entryId|path|string|true|none|

<h3 id="delete__api_change-log_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_change-log_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/change-log/string");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"title\":\"string\",\"description\":\"string\",\"notificationDate\":\"2019-08-24T14:15:22Z\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"updatedOn\":\"2019-08-24T14:15:22Z\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"title\":\"string\",\"description\":\"string\",\"notificationDate\":\"2019-08-24T14:15:22Z\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"updatedOn\":\"2019-08-24T14:15:22Z\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/change-log/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"title\":\"string\",\"description\":\"string\",\"notificationDate\":\"2019-08-24T14:15:22Z\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"updatedOn\":\"2019-08-24T14:15:22Z\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/change-log/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/change-log/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 167

{"id":"string","title":"string","description":"string","notificationDate":"2019-08-24T14:15:22Z","createdOn":"2019-08-24T14:15:22Z","updatedOn":"2019-08-24T14:15:22Z"}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/change-log/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"title\":\"string\",\"description\":\"string\",\"notificationDate\":\"2019-08-24T14:15:22Z\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"updatedOn\":\"2019-08-24T14:15:22Z\"}")
  .asString();
```

`PUT /api/change-log/{entryId}`

> Body parameter

```json
{
  "id": "string",
  "title": "string",
  "description": "string",
  "notificationDate": "2019-08-24T14:15:22Z",
  "createdOn": "2019-08-24T14:15:22Z",
  "updatedOn": "2019-08-24T14:15:22Z"
}
```

<h3 id="put__api_change-log_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|entryId|path|string|true|none|
|body|body|[ChangeLogItemDto](#schemachangelogitemdto)|false|none|

<h3 id="put__api_change-log_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-communication">Communication</h1>

## get__api_Communication_event_{eventIdOrSlug}_emailIdentities

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Communication/event/string/emailIdentities");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Communication/event/string/emailIdentities", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Communication/event/string/emailIdentities");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Communication/event/string/emailIdentities HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Communication/event/string/emailIdentities")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Communication/event/{eventIdOrSlug}/emailIdentities`

<h3 id="get__api_communication_event_{eventidorslug}_emailidentities-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|

<h3 id="get__api_communication_event_{eventidorslug}_emailidentities-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Communication_event_{eventIdOrSlug}_emailIdentities

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Communication/event/string/emailIdentities");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"email\":\"string\",\"friendlyName\":\"string\",\"isDefault\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"email\":\"string\",\"friendlyName\":\"string\",\"isDefault\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Communication/event/string/emailIdentities", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"email\":\"string\",\"friendlyName\":\"string\",\"isDefault\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Communication/event/string/emailIdentities");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Communication/event/string/emailIdentities HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 59

{"email":"string","friendlyName":"string","isDefault":true}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Communication/event/string/emailIdentities")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"email\":\"string\",\"friendlyName\":\"string\",\"isDefault\":true}")
  .asString();
```

`POST /api/Communication/event/{eventIdOrSlug}/emailIdentities`

> Body parameter

```json
{
  "email": "string",
  "friendlyName": "string",
  "isDefault": true
}
```

<h3 id="post__api_communication_event_{eventidorslug}_emailidentities-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|
|body|body|[VerifyEmailAddressRequest](#schemaverifyemailaddressrequest)|false|none|

<h3 id="post__api_communication_event_{eventidorslug}_emailidentities-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_Communication_event_{eventIdOrSlug}_emailIdentities_{senderEmailId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Communication/event/string/emailIdentities/string");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"email\":\"string\",\"friendlyName\":\"string\",\"isDefault\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"email\":\"string\",\"friendlyName\":\"string\",\"isDefault\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/Communication/event/string/emailIdentities/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"email\":\"string\",\"friendlyName\":\"string\",\"isDefault\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/Communication/event/string/emailIdentities/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/Communication/event/string/emailIdentities/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 59

{"email":"string","friendlyName":"string","isDefault":true}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/Communication/event/string/emailIdentities/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"email\":\"string\",\"friendlyName\":\"string\",\"isDefault\":true}")
  .asString();
```

`PUT /api/Communication/event/{eventIdOrSlug}/emailIdentities/{senderEmailId}`

> Body parameter

```json
{
  "email": "string",
  "friendlyName": "string",
  "isDefault": true
}
```

<h3 id="put__api_communication_event_{eventidorslug}_emailidentities_{senderemailid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|
|senderEmailId|path|string|true|none|
|body|body|[UpdateEmailAddressRequest](#schemaupdateemailaddressrequest)|false|none|

<h3 id="put__api_communication_event_{eventidorslug}_emailidentities_{senderemailid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_Communication_event_{eventIdOrSlug}_emailIdentities_{senderEmailId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Communication/event/string/emailIdentities/string");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("DELETE", "/api/Communication/event/string/emailIdentities/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/Communication/event/string/emailIdentities/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/Communication/event/string/emailIdentities/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/Communication/event/string/emailIdentities/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`DELETE /api/Communication/event/{eventIdOrSlug}/emailIdentities/{senderEmailId}`

<h3 id="delete__api_communication_event_{eventidorslug}_emailidentities_{senderemailid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|
|senderEmailId|path|string|true|none|

<h3 id="delete__api_communication_event_{eventidorslug}_emailidentities_{senderemailid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Communication_workspace_{workspaceIdOrSlug}_emailIdentities

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Communication/workspace/string/emailIdentities");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Communication/workspace/string/emailIdentities", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Communication/workspace/string/emailIdentities");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Communication/workspace/string/emailIdentities HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Communication/workspace/string/emailIdentities")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Communication/workspace/{workspaceIdOrSlug}/emailIdentities`

<h3 id="get__api_communication_workspace_{workspaceidorslug}_emailidentities-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|workspaceIdOrSlug|path|string|true|none|

<h3 id="get__api_communication_workspace_{workspaceidorslug}_emailidentities-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Communication_workspace_{workspaceIdOrSlug}_emailIdentities

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Communication/workspace/string/emailIdentities");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"email\":\"string\",\"friendlyName\":\"string\",\"isDefault\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"email\":\"string\",\"friendlyName\":\"string\",\"isDefault\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Communication/workspace/string/emailIdentities", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"email\":\"string\",\"friendlyName\":\"string\",\"isDefault\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Communication/workspace/string/emailIdentities");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Communication/workspace/string/emailIdentities HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 59

{"email":"string","friendlyName":"string","isDefault":true}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Communication/workspace/string/emailIdentities")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"email\":\"string\",\"friendlyName\":\"string\",\"isDefault\":true}")
  .asString();
```

`POST /api/Communication/workspace/{workspaceIdOrSlug}/emailIdentities`

> Body parameter

```json
{
  "email": "string",
  "friendlyName": "string",
  "isDefault": true
}
```

<h3 id="post__api_communication_workspace_{workspaceidorslug}_emailidentities-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|workspaceIdOrSlug|path|string|true|none|
|body|body|[VerifyEmailAddressRequest](#schemaverifyemailaddressrequest)|false|none|

<h3 id="post__api_communication_workspace_{workspaceidorslug}_emailidentities-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_Communication_workspace_{workspaceIdOrSlug}_emailIdentities_{senderEmailId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Communication/workspace/string/emailIdentities/string");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"email\":\"string\",\"friendlyName\":\"string\",\"isDefault\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"email\":\"string\",\"friendlyName\":\"string\",\"isDefault\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/Communication/workspace/string/emailIdentities/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"email\":\"string\",\"friendlyName\":\"string\",\"isDefault\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/Communication/workspace/string/emailIdentities/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/Communication/workspace/string/emailIdentities/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 59

{"email":"string","friendlyName":"string","isDefault":true}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/Communication/workspace/string/emailIdentities/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"email\":\"string\",\"friendlyName\":\"string\",\"isDefault\":true}")
  .asString();
```

`PUT /api/Communication/workspace/{workspaceIdOrSlug}/emailIdentities/{senderEmailId}`

> Body parameter

```json
{
  "email": "string",
  "friendlyName": "string",
  "isDefault": true
}
```

<h3 id="put__api_communication_workspace_{workspaceidorslug}_emailidentities_{senderemailid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|workspaceIdOrSlug|path|string|true|none|
|senderEmailId|path|string|true|none|
|body|body|[UpdateEmailAddressRequest](#schemaupdateemailaddressrequest)|false|none|

<h3 id="put__api_communication_workspace_{workspaceidorslug}_emailidentities_{senderemailid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_Communication_workspace_{workspaceIdOrSlug}_emailIdentities_{senderEmailId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Communication/workspace/string/emailIdentities/string");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("DELETE", "/api/Communication/workspace/string/emailIdentities/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/Communication/workspace/string/emailIdentities/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/Communication/workspace/string/emailIdentities/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/Communication/workspace/string/emailIdentities/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`DELETE /api/Communication/workspace/{workspaceIdOrSlug}/emailIdentities/{senderEmailId}`

<h3 id="delete__api_communication_workspace_{workspaceidorslug}_emailidentities_{senderemailid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|workspaceIdOrSlug|path|string|true|none|
|senderEmailId|path|string|true|none|

<h3 id="delete__api_communication_workspace_{workspaceidorslug}_emailidentities_{senderemailid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-document">Document</h1>

## get__api_Document_signupTerms

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Document/signupTerms");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Document/signupTerms", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Document/signupTerms");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Document/signupTerms HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Document/signupTerms")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Document/signupTerms`

<h3 id="get__api_document_signupterms-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-event">Event</h1>

## get__api_Event_all

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/all");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Event/all", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Event/all");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Event/all HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Event/all")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Event/all`

<h3 id="get__api_event_all-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Event_updated_{limit}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/updated/0");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Event/updated/0", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Event/updated/0");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Event/updated/0 HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Event/updated/0")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Event/updated/{limit}`

<h3 id="get__api_event_updated_{limit}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|limit|path|integer(int32)|true|none|

<h3 id="get__api_event_updated_{limit}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Event_newest_{limit}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/newest/0");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Event/newest/0", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Event/newest/0");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Event/newest/0 HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Event/newest/0")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Event/newest/{limit}`

<h3 id="get__api_event_newest_{limit}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|limit|path|integer(int32)|true|none|

<h3 id="get__api_event_newest_{limit}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Event_upcoming

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/upcoming");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Event/upcoming", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Event/upcoming");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Event/upcoming HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Event/upcoming")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Event/upcoming`

<h3 id="get__api_event_upcoming-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Event_{eventIdOrSlug}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Event/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Event/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Event/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Event/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Event/{eventIdOrSlug}`

<h3 id="get__api_event_{eventidorslug}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|

<h3 id="get__api_event_{eventidorslug}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_Event_{eventId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/string");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"name\":\"string\",\"slug\":\"string\",\"description\":\"string\",\"venue\":\"string\",\"isPaymentEnabled\":true,\"price\":0,\"paymentApiKey\":\"string\",\"paymentApiSecret\":\"string\",\"timezone\":\"string\",\"currency\":\"string\",\"language\":\"string\",\"dataControllerName\":\"string\",\"dataControllerEmail\":\"user@example.com\",\"dataProcessorName\":\"string\",\"dataProcessorEmail\":\"user@example.com\",\"isLiveEventEnabled\":true,\"isRegistrationEnabled\":true,\"isMinglEvent\":true,\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\",\"isDirty\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"name\":\"string\",\"slug\":\"string\",\"description\":\"string\",\"venue\":\"string\",\"isPaymentEnabled\":true,\"price\":0,\"paymentApiKey\":\"string\",\"paymentApiSecret\":\"string\",\"timezone\":\"string\",\"currency\":\"string\",\"language\":\"string\",\"dataControllerName\":\"string\",\"dataControllerEmail\":\"user@example.com\",\"dataProcessorName\":\"string\",\"dataProcessorEmail\":\"user@example.com\",\"isLiveEventEnabled\":true,\"isRegistrationEnabled\":true,\"isMinglEvent\":true,\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\",\"isDirty\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/Event/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"name\":\"string\",\"slug\":\"string\",\"description\":\"string\",\"venue\":\"string\",\"isPaymentEnabled\":true,\"price\":0,\"paymentApiKey\":\"string\",\"paymentApiSecret\":\"string\",\"timezone\":\"string\",\"currency\":\"string\",\"language\":\"string\",\"dataControllerName\":\"string\",\"dataControllerEmail\":\"user@example.com\",\"dataProcessorName\":\"string\",\"dataProcessorEmail\":\"user@example.com\",\"isLiveEventEnabled\":true,\"isRegistrationEnabled\":true,\"isMinglEvent\":true,\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\",\"isDirty\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/Event/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/Event/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 518

{"name":"string","slug":"string","description":"string","venue":"string","isPaymentEnabled":true,"price":0,"paymentApiKey":"string","paymentApiSecret":"string","timezone":"string","currency":"string","language":"string","dataControllerName":"string","dataControllerEmail":"user@example.com","dataProcessorName":"string","dataProcessorEmail":"user@example.com","isLiveEventEnabled":true,"isRegistrationEnabled":true,"isMinglEvent":true,"startDate":"2019-08-24T14:15:22Z","endDate":"2019-08-24T14:15:22Z","isDirty":true}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/Event/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"name\":\"string\",\"slug\":\"string\",\"description\":\"string\",\"venue\":\"string\",\"isPaymentEnabled\":true,\"price\":0,\"paymentApiKey\":\"string\",\"paymentApiSecret\":\"string\",\"timezone\":\"string\",\"currency\":\"string\",\"language\":\"string\",\"dataControllerName\":\"string\",\"dataControllerEmail\":\"user@example.com\",\"dataProcessorName\":\"string\",\"dataProcessorEmail\":\"user@example.com\",\"isLiveEventEnabled\":true,\"isRegistrationEnabled\":true,\"isMinglEvent\":true,\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\",\"isDirty\":true}")
  .asString();
```

`PUT /api/Event/{eventId}`

> Body parameter

```json
{
  "name": "string",
  "slug": "string",
  "description": "string",
  "venue": "string",
  "isPaymentEnabled": true,
  "price": 0,
  "paymentApiKey": "string",
  "paymentApiSecret": "string",
  "timezone": "string",
  "currency": "string",
  "language": "string",
  "dataControllerName": "string",
  "dataControllerEmail": "user@example.com",
  "dataProcessorName": "string",
  "dataProcessorEmail": "user@example.com",
  "isLiveEventEnabled": true,
  "isRegistrationEnabled": true,
  "isMinglEvent": true,
  "startDate": "2019-08-24T14:15:22Z",
  "endDate": "2019-08-24T14:15:22Z",
  "isDirty": true
}
```

<h3 id="put__api_event_{eventid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[UpdateEventDto](#schemaupdateeventdto)|false|none|

<h3 id="put__api_event_{eventid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_Event_{eventId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/string");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("DELETE", "/api/Event/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/Event/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/Event/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/Event/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`DELETE /api/Event/{eventId}`

<h3 id="delete__api_event_{eventid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|

<h3 id="delete__api_event_{eventid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Event_create

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/create");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"name\":\"string\",\"slug\":\"string\",\"description\":\"string\",\"venue\":\"string\",\"isPaymentEnabled\":true,\"price\":0,\"paymentApiKey\":\"string\",\"paymentApiSecret\":\"string\",\"timezone\":\"string\",\"currency\":\"string\",\"language\":\"string\",\"dataControllerName\":\"string\",\"dataControllerEmail\":\"user@example.com\",\"dataProcessorName\":\"string\",\"dataProcessorEmail\":\"user@example.com\",\"isLiveEventEnabled\":true,\"isRegistrationEnabled\":true,\"isMinglEvent\":true,\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\",\"workspaceId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"name\":\"string\",\"slug\":\"string\",\"description\":\"string\",\"venue\":\"string\",\"isPaymentEnabled\":true,\"price\":0,\"paymentApiKey\":\"string\",\"paymentApiSecret\":\"string\",\"timezone\":\"string\",\"currency\":\"string\",\"language\":\"string\",\"dataControllerName\":\"string\",\"dataControllerEmail\":\"user@example.com\",\"dataProcessorName\":\"string\",\"dataProcessorEmail\":\"user@example.com\",\"isLiveEventEnabled\":true,\"isRegistrationEnabled\":true,\"isMinglEvent\":true,\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\",\"workspaceId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Event/create", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"name\":\"string\",\"slug\":\"string\",\"description\":\"string\",\"venue\":\"string\",\"isPaymentEnabled\":true,\"price\":0,\"paymentApiKey\":\"string\",\"paymentApiSecret\":\"string\",\"timezone\":\"string\",\"currency\":\"string\",\"language\":\"string\",\"dataControllerName\":\"string\",\"dataControllerEmail\":\"user@example.com\",\"dataProcessorName\":\"string\",\"dataProcessorEmail\":\"user@example.com\",\"isLiveEventEnabled\":true,\"isRegistrationEnabled\":true,\"isMinglEvent\":true,\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\",\"workspaceId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Event/create");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Event/create HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 526

{"name":"string","slug":"string","description":"string","venue":"string","isPaymentEnabled":true,"price":0,"paymentApiKey":"string","paymentApiSecret":"string","timezone":"string","currency":"string","language":"string","dataControllerName":"string","dataControllerEmail":"user@example.com","dataProcessorName":"string","dataProcessorEmail":"user@example.com","isLiveEventEnabled":true,"isRegistrationEnabled":true,"isMinglEvent":true,"startDate":"2019-08-24T14:15:22Z","endDate":"2019-08-24T14:15:22Z","workspaceId":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Event/create")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"name\":\"string\",\"slug\":\"string\",\"description\":\"string\",\"venue\":\"string\",\"isPaymentEnabled\":true,\"price\":0,\"paymentApiKey\":\"string\",\"paymentApiSecret\":\"string\",\"timezone\":\"string\",\"currency\":\"string\",\"language\":\"string\",\"dataControllerName\":\"string\",\"dataControllerEmail\":\"user@example.com\",\"dataProcessorName\":\"string\",\"dataProcessorEmail\":\"user@example.com\",\"isLiveEventEnabled\":true,\"isRegistrationEnabled\":true,\"isMinglEvent\":true,\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\",\"workspaceId\":\"string\"}")
  .asString();
```

`POST /api/Event/create`

> Body parameter

```json
{
  "name": "string",
  "slug": "string",
  "description": "string",
  "venue": "string",
  "isPaymentEnabled": true,
  "price": 0,
  "paymentApiKey": "string",
  "paymentApiSecret": "string",
  "timezone": "string",
  "currency": "string",
  "language": "string",
  "dataControllerName": "string",
  "dataControllerEmail": "user@example.com",
  "dataProcessorName": "string",
  "dataProcessorEmail": "user@example.com",
  "isLiveEventEnabled": true,
  "isRegistrationEnabled": true,
  "isMinglEvent": true,
  "startDate": "2019-08-24T14:15:22Z",
  "endDate": "2019-08-24T14:15:22Z",
  "workspaceId": "string"
}
```

<h3 id="post__api_event_create-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[CreateEventDto](#schemacreateeventdto)|false|none|

<h3 id="post__api_event_create-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Event_form

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/form");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"eventId\":\"string\",\"elements\":[{\"id\":\"string\",\"type\":0,\"options\":null,\"logic\":{\"isEnabled\":true,\"components\":[{\"id\":\"string\",\"action\":0,\"fieldId\":\"string\",\"operator\":0,\"value\":\"string\"}]},\"mandatory\":true}],\"formMetadata\":{\"registrationStartDate\":\"2019-08-24T14:15:22Z\",\"registrationEndDate\":\"2019-08-24T14:15:22Z\",\"attendeeLimit\":0,\"isDirty\":true},\"isDirty\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"eventId\":\"string\",\"elements\":[{\"id\":\"string\",\"type\":0,\"options\":null,\"logic\":{\"isEnabled\":true,\"components\":[{\"id\":\"string\",\"action\":0,\"fieldId\":\"string\",\"operator\":0,\"value\":\"string\"}]},\"mandatory\":true}],\"formMetadata\":{\"registrationStartDate\":\"2019-08-24T14:15:22Z\",\"registrationEndDate\":\"2019-08-24T14:15:22Z\",\"attendeeLimit\":0,\"isDirty\":true},\"isDirty\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Event/form", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"eventId\":\"string\",\"elements\":[{\"id\":\"string\",\"type\":0,\"options\":null,\"logic\":{\"isEnabled\":true,\"components\":[{\"id\":\"string\",\"action\":0,\"fieldId\":\"string\",\"operator\":0,\"value\":\"string\"}]},\"mandatory\":true}],\"formMetadata\":{\"registrationStartDate\":\"2019-08-24T14:15:22Z\",\"registrationEndDate\":\"2019-08-24T14:15:22Z\",\"attendeeLimit\":0,\"isDirty\":true},\"isDirty\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Event/form");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Event/form HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 365

{"eventId":"string","elements":[{"id":"string","type":0,"options":null,"logic":{"isEnabled":true,"components":[{"id":"string","action":0,"fieldId":"string","operator":0,"value":"string"}]},"mandatory":true}],"formMetadata":{"registrationStartDate":"2019-08-24T14:15:22Z","registrationEndDate":"2019-08-24T14:15:22Z","attendeeLimit":0,"isDirty":true},"isDirty":true}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Event/form")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"eventId\":\"string\",\"elements\":[{\"id\":\"string\",\"type\":0,\"options\":null,\"logic\":{\"isEnabled\":true,\"components\":[{\"id\":\"string\",\"action\":0,\"fieldId\":\"string\",\"operator\":0,\"value\":\"string\"}]},\"mandatory\":true}],\"formMetadata\":{\"registrationStartDate\":\"2019-08-24T14:15:22Z\",\"registrationEndDate\":\"2019-08-24T14:15:22Z\",\"attendeeLimit\":0,\"isDirty\":true},\"isDirty\":true}")
  .asString();
```

`POST /api/Event/form`

> Body parameter

```json
{
  "eventId": "string",
  "elements": [
    {
      "id": "string",
      "type": 0,
      "options": null,
      "logic": {
        "isEnabled": true,
        "components": [
          {
            "id": "string",
            "action": 0,
            "fieldId": "string",
            "operator": 0,
            "value": "string"
          }
        ]
      },
      "mandatory": true
    }
  ],
  "formMetadata": {
    "registrationStartDate": "2019-08-24T14:15:22Z",
    "registrationEndDate": "2019-08-24T14:15:22Z",
    "attendeeLimit": 0,
    "isDirty": true
  },
  "isDirty": true
}
```

<h3 id="post__api_event_form-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[EventFormUpdateDto](#schemaeventformupdatedto)|false|none|

<h3 id="post__api_event_form-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Event_landingpage

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/landingpage");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"eventId\":\"string\",\"widgets\":[{\"id\":\"string\",\"type\":1,\"options\":null,\"mandatory\":true}],\"branding\":{\"showHeader\":true,\"headerBackgroundColor\":\"string\",\"headerBackgroundUrl\":\"string\",\"headerTextColor\":\"string\",\"headerHeight\":0,\"headerSpacing\":0,\"headerTitleSize\":0,\"transparentHeader\":true,\"faviconUrl\":\"string\",\"backgroundColor\":\"string\",\"backgroundImageUrl\":\"string\",\"backgroundRepeat\":\"string\",\"backgroundPosition\":\"string\",\"fixedBackground\":true},\"templates\":{\"successfulRegistrationHtmlTemplate\":\"string\",\"isDirty\":true},\"isPreview\":true,\"isDirty\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"eventId\":\"string\",\"widgets\":[{\"id\":\"string\",\"type\":1,\"options\":null,\"mandatory\":true}],\"branding\":{\"showHeader\":true,\"headerBackgroundColor\":\"string\",\"headerBackgroundUrl\":\"string\",\"headerTextColor\":\"string\",\"headerHeight\":0,\"headerSpacing\":0,\"headerTitleSize\":0,\"transparentHeader\":true,\"faviconUrl\":\"string\",\"backgroundColor\":\"string\",\"backgroundImageUrl\":\"string\",\"backgroundRepeat\":\"string\",\"backgroundPosition\":\"string\",\"fixedBackground\":true},\"templates\":{\"successfulRegistrationHtmlTemplate\":\"string\",\"isDirty\":true},\"isPreview\":true,\"isDirty\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Event/landingpage", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"eventId\":\"string\",\"widgets\":[{\"id\":\"string\",\"type\":1,\"options\":null,\"mandatory\":true}],\"branding\":{\"showHeader\":true,\"headerBackgroundColor\":\"string\",\"headerBackgroundUrl\":\"string\",\"headerTextColor\":\"string\",\"headerHeight\":0,\"headerSpacing\":0,\"headerTitleSize\":0,\"transparentHeader\":true,\"faviconUrl\":\"string\",\"backgroundColor\":\"string\",\"backgroundImageUrl\":\"string\",\"backgroundRepeat\":\"string\",\"backgroundPosition\":\"string\",\"fixedBackground\":true},\"templates\":{\"successfulRegistrationHtmlTemplate\":\"string\",\"isDirty\":true},\"isPreview\":true,\"isDirty\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Event/landingpage");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Event/landingpage HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 558

{"eventId":"string","widgets":[{"id":"string","type":1,"options":null,"mandatory":true}],"branding":{"showHeader":true,"headerBackgroundColor":"string","headerBackgroundUrl":"string","headerTextColor":"string","headerHeight":0,"headerSpacing":0,"headerTitleSize":0,"transparentHeader":true,"faviconUrl":"string","backgroundColor":"string","backgroundImageUrl":"string","backgroundRepeat":"string","backgroundPosition":"string","fixedBackground":true},"templates":{"successfulRegistrationHtmlTemplate":"string","isDirty":true},"isPreview":true,"isDirty":true}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Event/landingpage")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"eventId\":\"string\",\"widgets\":[{\"id\":\"string\",\"type\":1,\"options\":null,\"mandatory\":true}],\"branding\":{\"showHeader\":true,\"headerBackgroundColor\":\"string\",\"headerBackgroundUrl\":\"string\",\"headerTextColor\":\"string\",\"headerHeight\":0,\"headerSpacing\":0,\"headerTitleSize\":0,\"transparentHeader\":true,\"faviconUrl\":\"string\",\"backgroundColor\":\"string\",\"backgroundImageUrl\":\"string\",\"backgroundRepeat\":\"string\",\"backgroundPosition\":\"string\",\"fixedBackground\":true},\"templates\":{\"successfulRegistrationHtmlTemplate\":\"string\",\"isDirty\":true},\"isPreview\":true,\"isDirty\":true}")
  .asString();
```

`POST /api/Event/landingpage`

> Body parameter

```json
{
  "eventId": "string",
  "widgets": [
    {
      "id": "string",
      "type": 1,
      "options": null,
      "mandatory": true
    }
  ],
  "branding": {
    "showHeader": true,
    "headerBackgroundColor": "string",
    "headerBackgroundUrl": "string",
    "headerTextColor": "string",
    "headerHeight": 0,
    "headerSpacing": 0,
    "headerTitleSize": 0,
    "transparentHeader": true,
    "faviconUrl": "string",
    "backgroundColor": "string",
    "backgroundImageUrl": "string",
    "backgroundRepeat": "string",
    "backgroundPosition": "string",
    "fixedBackground": true
  },
  "templates": {
    "successfulRegistrationHtmlTemplate": "string",
    "isDirty": true
  },
  "isPreview": true,
  "isDirty": true
}
```

<h3 id="post__api_event_landingpage-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[EventLandingPageUpdateDto](#schemaeventlandingpageupdatedto)|false|none|

<h3 id="post__api_event_landingpage-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Event_lobbypage

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/lobbypage");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"eventId\":\"string\",\"elements\":[{\"id\":\"string\",\"category\":1,\"type\":0,\"options\":null,\"mandatory\":true}],\"branding\":{\"backgroundColor\":\"string\",\"textColor\":\"string\",\"navigationBackgroundColor\":\"string\",\"primaryBackgroundColor\":\"string\",\"primaryTextColor\":\"string\",\"secondaryBackgroundColor\":\"string\",\"secondaryTextColor\":\"string\"},\"isPreview\":true,\"isDirty\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"eventId\":\"string\",\"elements\":[{\"id\":\"string\",\"category\":1,\"type\":0,\"options\":null,\"mandatory\":true}],\"branding\":{\"backgroundColor\":\"string\",\"textColor\":\"string\",\"navigationBackgroundColor\":\"string\",\"primaryBackgroundColor\":\"string\",\"primaryTextColor\":\"string\",\"secondaryBackgroundColor\":\"string\",\"secondaryTextColor\":\"string\"},\"isPreview\":true,\"isDirty\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Event/lobbypage", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"eventId\":\"string\",\"elements\":[{\"id\":\"string\",\"category\":1,\"type\":0,\"options\":null,\"mandatory\":true}],\"branding\":{\"backgroundColor\":\"string\",\"textColor\":\"string\",\"navigationBackgroundColor\":\"string\",\"primaryBackgroundColor\":\"string\",\"primaryTextColor\":\"string\",\"secondaryBackgroundColor\":\"string\",\"secondaryTextColor\":\"string\"},\"isPreview\":true,\"isDirty\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Event/lobbypage");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Event/lobbypage HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 361

{"eventId":"string","elements":[{"id":"string","category":1,"type":0,"options":null,"mandatory":true}],"branding":{"backgroundColor":"string","textColor":"string","navigationBackgroundColor":"string","primaryBackgroundColor":"string","primaryTextColor":"string","secondaryBackgroundColor":"string","secondaryTextColor":"string"},"isPreview":true,"isDirty":true}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Event/lobbypage")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"eventId\":\"string\",\"elements\":[{\"id\":\"string\",\"category\":1,\"type\":0,\"options\":null,\"mandatory\":true}],\"branding\":{\"backgroundColor\":\"string\",\"textColor\":\"string\",\"navigationBackgroundColor\":\"string\",\"primaryBackgroundColor\":\"string\",\"primaryTextColor\":\"string\",\"secondaryBackgroundColor\":\"string\",\"secondaryTextColor\":\"string\"},\"isPreview\":true,\"isDirty\":true}")
  .asString();
```

`POST /api/Event/lobbypage`

> Body parameter

```json
{
  "eventId": "string",
  "elements": [
    {
      "id": "string",
      "category": 1,
      "type": 0,
      "options": null,
      "mandatory": true
    }
  ],
  "branding": {
    "backgroundColor": "string",
    "textColor": "string",
    "navigationBackgroundColor": "string",
    "primaryBackgroundColor": "string",
    "primaryTextColor": "string",
    "secondaryBackgroundColor": "string",
    "secondaryTextColor": "string"
  },
  "isPreview": true,
  "isDirty": true
}
```

<h3 id="post__api_event_lobbypage-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[EventLobbyPageUpdateDto](#schemaeventlobbypageupdatedto)|false|none|

<h3 id="post__api_event_lobbypage-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Event_templatepage

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/templatepage");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"successfulRegistrationHtmlTemplate\":\"string\",\"isDirty\":true,\"eventId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"successfulRegistrationHtmlTemplate\":\"string\",\"isDirty\":true,\"eventId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Event/templatepage", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"successfulRegistrationHtmlTemplate\":\"string\",\"isDirty\":true,\"eventId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Event/templatepage");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Event/templatepage HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 81

{"successfulRegistrationHtmlTemplate":"string","isDirty":true,"eventId":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Event/templatepage")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"successfulRegistrationHtmlTemplate\":\"string\",\"isDirty\":true,\"eventId\":\"string\"}")
  .asString();
```

`POST /api/Event/templatepage`

> Body parameter

```json
{
  "successfulRegistrationHtmlTemplate": "string",
  "isDirty": true,
  "eventId": "string"
}
```

<h3 id="post__api_event_templatepage-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[EventTemplatePageUpdateDto](#schemaeventtemplatepageupdatedto)|false|none|

<h3 id="post__api_event_templatepage-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Event_publish

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/publish");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"eventId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"eventId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Event/publish", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"eventId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Event/publish");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Event/publish HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 20

{"eventId":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Event/publish")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"eventId\":\"string\"}")
  .asString();
```

`POST /api/Event/publish`

> Body parameter

```json
{
  "eventId": "string"
}
```

<h3 id="post__api_event_publish-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[PublishEventDto](#schemapublisheventdto)|false|none|

<h3 id="post__api_event_publish-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Event_{eventId}_preview

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/string/preview");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Event/string/preview", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Event/string/preview");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Event/string/preview HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Event/string/preview")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Event/{eventId}/preview`

<h3 id="get__api_event_{eventid}_preview-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|

<h3 id="get__api_event_{eventid}_preview-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Event_{eventIdOrSlug}_sms

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/string/sms");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Event/string/sms", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Event/string/sms");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Event/string/sms HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Event/string/sms")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Event/{eventIdOrSlug}/sms`

<h3 id="get__api_event_{eventidorslug}_sms-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|

<h3 id="get__api_event_{eventidorslug}_sms-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Event_{eventId}_sms_{smsId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/string/sms/string");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/api/Event/string/sms/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Event/string/sms/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Event/string/sms/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Event/string/sms/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /api/Event/{eventId}/sms/{smsId}`

<h3 id="post__api_event_{eventid}_sms_{smsid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|smsId|path|string|true|none|

<h3 id="post__api_event_{eventid}_sms_{smsid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Event_{eventId}_branding

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/string/branding");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"logoUrl\":\"string\",\"faviconUrl\":\"string\",\"primaryButtonBackgroundColor\":\"string\",\"primaryButtonTextColor\":\"string\",\"secondaryButtonBackgroundColor\":\"string\",\"secondaryButtonTextColor\":\"string\",\"socialEventImageUrl\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"logoUrl\":\"string\",\"faviconUrl\":\"string\",\"primaryButtonBackgroundColor\":\"string\",\"primaryButtonTextColor\":\"string\",\"secondaryButtonBackgroundColor\":\"string\",\"secondaryButtonTextColor\":\"string\",\"socialEventImageUrl\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Event/string/branding", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"logoUrl\":\"string\",\"faviconUrl\":\"string\",\"primaryButtonBackgroundColor\":\"string\",\"primaryButtonTextColor\":\"string\",\"secondaryButtonBackgroundColor\":\"string\",\"secondaryButtonTextColor\":\"string\",\"socialEventImageUrl\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Event/string/branding");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Event/string/branding HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 225

{"logoUrl":"string","faviconUrl":"string","primaryButtonBackgroundColor":"string","primaryButtonTextColor":"string","secondaryButtonBackgroundColor":"string","secondaryButtonTextColor":"string","socialEventImageUrl":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Event/string/branding")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"logoUrl\":\"string\",\"faviconUrl\":\"string\",\"primaryButtonBackgroundColor\":\"string\",\"primaryButtonTextColor\":\"string\",\"secondaryButtonBackgroundColor\":\"string\",\"secondaryButtonTextColor\":\"string\",\"socialEventImageUrl\":\"string\"}")
  .asString();
```

`POST /api/Event/{eventId}/branding`

> Body parameter

```json
{
  "logoUrl": "string",
  "faviconUrl": "string",
  "primaryButtonBackgroundColor": "string",
  "primaryButtonTextColor": "string",
  "secondaryButtonBackgroundColor": "string",
  "secondaryButtonTextColor": "string",
  "socialEventImageUrl": "string"
}
```

<h3 id="post__api_event_{eventid}_branding-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[BrandingUpdateDto](#schemabrandingupdatedto)|false|none|

<h3 id="post__api_event_{eventid}_branding-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_Event_{eventId}_branding

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/string/branding");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"logoUrl\":true,\"faviconUrl\":true,\"primaryButtonBackgroundColor\":true,\"primaryButtonTextColor\":true,\"secondaryButtonBackgroundColor\":true,\"secondaryButtonTextColor\":true,\"socialEventImageUrl\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"logoUrl\":true,\"faviconUrl\":true,\"primaryButtonBackgroundColor\":true,\"primaryButtonTextColor\":true,\"secondaryButtonBackgroundColor\":true,\"secondaryButtonTextColor\":true,\"socialEventImageUrl\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("DELETE", "/api/Event/string/branding", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"logoUrl\":true,\"faviconUrl\":true,\"primaryButtonBackgroundColor\":true,\"primaryButtonTextColor\":true,\"secondaryButtonBackgroundColor\":true,\"secondaryButtonTextColor\":true,\"socialEventImageUrl\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/Event/string/branding");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/Event/string/branding HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 197

{"logoUrl":true,"faviconUrl":true,"primaryButtonBackgroundColor":true,"primaryButtonTextColor":true,"secondaryButtonBackgroundColor":true,"secondaryButtonTextColor":true,"socialEventImageUrl":true}
```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/Event/string/branding")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"logoUrl\":true,\"faviconUrl\":true,\"primaryButtonBackgroundColor\":true,\"primaryButtonTextColor\":true,\"secondaryButtonBackgroundColor\":true,\"secondaryButtonTextColor\":true,\"socialEventImageUrl\":true}")
  .asString();
```

`DELETE /api/Event/{eventId}/branding`

> Body parameter

```json
{
  "logoUrl": true,
  "faviconUrl": true,
  "primaryButtonBackgroundColor": true,
  "primaryButtonTextColor": true,
  "secondaryButtonBackgroundColor": true,
  "secondaryButtonTextColor": true,
  "socialEventImageUrl": true
}
```

<h3 id="delete__api_event_{eventid}_branding-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[BrandingDeleteDto](#schemabrandingdeletedto)|false|none|

<h3 id="delete__api_event_{eventid}_branding-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Event_{eventId}_liveSettings

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/string/liveSettings");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"stageStream\":{\"type\":0,\"url\":\"string\",\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true}}},\"isRegisterEnabled\":true,\"isLoginEnabled\":true,\"loginCaption\":\"string\",\"loginDisabledFrom\":\"2019-08-24T14:15:22Z\",\"loginDisabledTo\":\"2019-08-24T14:15:22Z\",\"isGamificationEnabled\":true,\"gamificationUrl\":\"string\",\"platformPages\":[0],\"newsFeed\":[0],\"newsFeedPosts\":[0],\"newsFeedComments\":[0],\"infoPages\":[0],\"userSettings\":[0],\"documents\":[0],\"sponsors\":[0],\"chat\":[0],\"speakers\":[0],\"agenda\":[0],\"support\":[0],\"participants\":[0],\"isParticipantEmailEnabled\":true,\"isParticipantPhoneEnabled\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"stageStream\":{\"type\":0,\"url\":\"string\",\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true}}},\"isRegisterEnabled\":true,\"isLoginEnabled\":true,\"loginCaption\":\"string\",\"loginDisabledFrom\":\"2019-08-24T14:15:22Z\",\"loginDisabledTo\":\"2019-08-24T14:15:22Z\",\"isGamificationEnabled\":true,\"gamificationUrl\":\"string\",\"platformPages\":[0],\"newsFeed\":[0],\"newsFeedPosts\":[0],\"newsFeedComments\":[0],\"infoPages\":[0],\"userSettings\":[0],\"documents\":[0],\"sponsors\":[0],\"chat\":[0],\"speakers\":[0],\"agenda\":[0],\"support\":[0],\"participants\":[0],\"isParticipantEmailEnabled\":true,\"isParticipantPhoneEnabled\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Event/string/liveSettings", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"stageStream\":{\"type\":0,\"url\":\"string\",\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true}}},\"isRegisterEnabled\":true,\"isLoginEnabled\":true,\"loginCaption\":\"string\",\"loginDisabledFrom\":\"2019-08-24T14:15:22Z\",\"loginDisabledTo\":\"2019-08-24T14:15:22Z\",\"isGamificationEnabled\":true,\"gamificationUrl\":\"string\",\"platformPages\":[0],\"newsFeed\":[0],\"newsFeedPosts\":[0],\"newsFeedComments\":[0],\"infoPages\":[0],\"userSettings\":[0],\"documents\":[0],\"sponsors\":[0],\"chat\":[0],\"speakers\":[0],\"agenda\":[0],\"support\":[0],\"participants\":[0],\"isParticipantEmailEnabled\":true,\"isParticipantPhoneEnabled\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Event/string/liveSettings");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Event/string/liveSettings HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 1011

{"stageStream":{"type":0,"url":"string","settings":{"host":{"isChatEnabled":true,"isPeopleEnabled":true,"isLeaveButtonEnabled":true,"isRecordingEnabled":true,"isScreenShareEnabled":true,"isBackgroundEnabled":true,"isVideoEnabled":true,"isAudioEnabled":true,"isBreakoutEnabled":true},"stream":{"isChatEnabled":true,"isPeopleEnabled":true,"isLeaveButtonEnabled":true,"isRecordingEnabled":true,"isScreenShareEnabled":true,"isBackgroundEnabled":true,"isVideoEnabled":true,"isAudioEnabled":true,"isBreakoutEnabled":true}}},"isRegisterEnabled":true,"isLoginEnabled":true,"loginCaption":"string","loginDisabledFrom":"2019-08-24T14:15:22Z","loginDisabledTo":"2019-08-24T14:15:22Z","isGamificationEnabled":true,"gamificationUrl":"string","platformPages":[0],"newsFeed":[0],"newsFeedPosts":[0],"newsFeedComments":[0],"infoPages":[0],"userSettings":[0],"documents":[0],"sponsors":[0],"chat":[0],"speakers":[0],"agenda":[0],"support":[0],"participants":[0],"isParticipantEmailEnabled":true,"isParticipantPhoneEnabled":true}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Event/string/liveSettings")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"stageStream\":{\"type\":0,\"url\":\"string\",\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true}}},\"isRegisterEnabled\":true,\"isLoginEnabled\":true,\"loginCaption\":\"string\",\"loginDisabledFrom\":\"2019-08-24T14:15:22Z\",\"loginDisabledTo\":\"2019-08-24T14:15:22Z\",\"isGamificationEnabled\":true,\"gamificationUrl\":\"string\",\"platformPages\":[0],\"newsFeed\":[0],\"newsFeedPosts\":[0],\"newsFeedComments\":[0],\"infoPages\":[0],\"userSettings\":[0],\"documents\":[0],\"sponsors\":[0],\"chat\":[0],\"speakers\":[0],\"agenda\":[0],\"support\":[0],\"participants\":[0],\"isParticipantEmailEnabled\":true,\"isParticipantPhoneEnabled\":true}")
  .asString();
```

`POST /api/Event/{eventId}/liveSettings`

> Body parameter

```json
{
  "stageStream": {
    "type": 0,
    "url": "string",
    "settings": {
      "host": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      },
      "stream": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      }
    }
  },
  "isRegisterEnabled": true,
  "isLoginEnabled": true,
  "loginCaption": "string",
  "loginDisabledFrom": "2019-08-24T14:15:22Z",
  "loginDisabledTo": "2019-08-24T14:15:22Z",
  "isGamificationEnabled": true,
  "gamificationUrl": "string",
  "platformPages": [
    0
  ],
  "newsFeed": [
    0
  ],
  "newsFeedPosts": [
    0
  ],
  "newsFeedComments": [
    0
  ],
  "infoPages": [
    0
  ],
  "userSettings": [
    0
  ],
  "documents": [
    0
  ],
  "sponsors": [
    0
  ],
  "chat": [
    0
  ],
  "speakers": [
    0
  ],
  "agenda": [
    0
  ],
  "support": [
    0
  ],
  "participants": [
    0
  ],
  "isParticipantEmailEnabled": true,
  "isParticipantPhoneEnabled": true
}
```

<h3 id="post__api_event_{eventid}_livesettings-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[LiveEventSettingsUpdateDto](#schemaliveeventsettingsupdatedto)|false|none|

<h3 id="post__api_event_{eventid}_livesettings-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Event_{eventIdOrSlug}_registrationPage_{registrationAccessKey}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/string/registrationPage/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Event/string/registrationPage/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Event/string/registrationPage/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Event/string/registrationPage/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Event/string/registrationPage/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Event/{eventIdOrSlug}/registrationPage/{registrationAccessKey}`

<h3 id="get__api_event_{eventidorslug}_registrationpage_{registrationaccesskey}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|
|registrationAccessKey|query|string|false|none|

<h3 id="get__api_event_{eventidorslug}_registrationpage_{registrationaccesskey}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Event_{eventIdOrSlug}_emailLog

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/string/emailLog");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Event/string/emailLog", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Event/string/emailLog");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Event/string/emailLog HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Event/string/emailLog")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Event/{eventIdOrSlug}/emailLog`

<h3 id="get__api_event_{eventidorslug}_emaillog-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|

<h3 id="get__api_event_{eventidorslug}_emaillog-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Event_validate-slug

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/validate-slug");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"eventId\":\"string\",\"slug\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"eventId\":\"string\",\"slug\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Event/validate-slug", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"eventId\":\"string\",\"slug\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Event/validate-slug");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Event/validate-slug HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 36

{"eventId":"string","slug":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Event/validate-slug")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"eventId\":\"string\",\"slug\":\"string\"}")
  .asString();
```

`POST /api/Event/validate-slug`

> Body parameter

```json
{
  "eventId": "string",
  "slug": "string"
}
```

<h3 id="post__api_event_validate-slug-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[SlugAvailabilityRequest](#schemaslugavailabilityrequest)|false|none|

<h3 id="post__api_event_validate-slug-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Event_{eventIdOrSlug}_statistics

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/string/statistics");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Event/string/statistics", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Event/string/statistics");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Event/string/statistics HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Event/string/statistics")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Event/{eventIdOrSlug}/statistics`

<h3 id="get__api_event_{eventidorslug}_statistics-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|

<h3 id="get__api_event_{eventidorslug}_statistics-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Event_{eventId}_duplicate

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/string/duplicate");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/api/Event/string/duplicate", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Event/string/duplicate");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Event/string/duplicate HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Event/string/duplicate")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /api/Event/{eventId}/duplicate`

<h3 id="post__api_event_{eventid}_duplicate-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|

<h3 id="post__api_event_{eventid}_duplicate-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## patch__api_Event_{eventId}_feature

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Event/string/feature");
var request = new RestRequest(Method.PATCH);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"type\":0,\"typeString\":0,\"completedOn\":\"2019-08-24T14:15:22Z\",\"disabledOn\":\"2019-08-24T14:15:22Z\",\"order\":0}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"type\":0,\"typeString\":0,\"completedOn\":\"2019-08-24T14:15:22Z\",\"disabledOn\":\"2019-08-24T14:15:22Z\",\"order\":0}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PATCH", "/api/Event/string/feature", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"type\":0,\"typeString\":0,\"completedOn\":\"2019-08-24T14:15:22Z\",\"disabledOn\":\"2019-08-24T14:15:22Z\",\"order\":0}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PATCH", "https://example.com/api/Event/string/feature");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PATCH /api/Event/string/feature HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 108

{"type":0,"typeString":0,"completedOn":"2019-08-24T14:15:22Z","disabledOn":"2019-08-24T14:15:22Z","order":0}
```

```java
HttpResponse<String> response = Unirest.patch("https://example.com/api/Event/string/feature")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"type\":0,\"typeString\":0,\"completedOn\":\"2019-08-24T14:15:22Z\",\"disabledOn\":\"2019-08-24T14:15:22Z\",\"order\":0}")
  .asString();
```

`PATCH /api/Event/{eventId}/feature`

> Body parameter

```json
{
  "type": 0,
  "typeString": 0,
  "completedOn": "2019-08-24T14:15:22Z",
  "disabledOn": "2019-08-24T14:15:22Z",
  "order": 0
}
```

<h3 id="patch__api_event_{eventid}_feature-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[EventFeatureDtoBase](#schemaeventfeaturedtobase)|false|none|

<h3 id="patch__api_event_{eventid}_feature-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-export">Export</h1>

## post__api_Export_{eventId}_participants

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Export/string/participants");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"selectedRows\":[\"string\"],\"selectedColumns\":[\"string\"]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"selectedRows\":[\"string\"],\"selectedColumns\":[\"string\"]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Export/string/participants", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"selectedRows\":[\"string\"],\"selectedColumns\":[\"string\"]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Export/string/participants");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Export/string/participants HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 56

{"selectedRows":["string"],"selectedColumns":["string"]}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Export/string/participants")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"selectedRows\":[\"string\"],\"selectedColumns\":[\"string\"]}")
  .asString();
```

`POST /api/Export/{eventId}/participants`

> Body parameter

```json
{
  "selectedRows": [
    "string"
  ],
  "selectedColumns": [
    "string"
  ]
}
```

<h3 id="post__api_export_{eventid}_participants-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[ExportParticipantsRequest](#schemaexportparticipantsrequest)|false|none|

<h3 id="post__api_export_{eventid}_participants-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Export_{eventId}_polls_{pollId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Export/string/polls/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Export/string/polls/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Export/string/polls/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Export/string/polls/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Export/string/polls/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Export/{eventId}/polls/{pollId}`

<h3 id="get__api_export_{eventid}_polls_{pollid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|pollId|path|string|true|none|

<h3 id="get__api_export_{eventid}_polls_{pollid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Export_{eventId}_example

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Export/string/example");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Export/string/example", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Export/string/example");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Export/string/example HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Export/string/example")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Export/{eventId}/example`

<h3 id="get__api_export_{eventid}_example-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|

<h3 id="get__api_export_{eventid}_example-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Export_{eventId}_timeline

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Export/string/timeline");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Export/string/timeline", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Export/string/timeline");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Export/string/timeline HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Export/string/timeline")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Export/{eventId}/timeline`

<h3 id="get__api_export_{eventid}_timeline-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|

<h3 id="get__api_export_{eventid}_timeline-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Export_{eventId}_emails

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Export/string/emails");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Export/string/emails", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Export/string/emails");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Export/string/emails HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Export/string/emails")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Export/{eventId}/emails`

<h3 id="get__api_export_{eventid}_emails-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|

<h3 id="get__api_export_{eventid}_emails-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Export_{eventId}_sms

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Export/string/sms");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Export/string/sms", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Export/string/sms");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Export/string/sms HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Export/string/sms")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Export/{eventId}/sms`

<h3 id="get__api_export_{eventid}_sms-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|

<h3 id="get__api_export_{eventid}_sms-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Export_sms_{start}_{end}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Export/sms/2019-08-24T14%3A15%3A22Z/2019-08-24T14%3A15%3A22Z");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Export/sms/2019-08-24T14%3A15%3A22Z/2019-08-24T14%3A15%3A22Z", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Export/sms/2019-08-24T14%3A15%3A22Z/2019-08-24T14%3A15%3A22Z");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Export/sms/2019-08-24T14%3A15%3A22Z/2019-08-24T14%3A15%3A22Z HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Export/sms/2019-08-24T14%3A15%3A22Z/2019-08-24T14%3A15%3A22Z")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Export/sms/{start}/{end}`

<h3 id="get__api_export_sms_{start}_{end}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|start|path|string(date-time)|true|none|
|end|path|string(date-time)|true|none|

<h3 id="get__api_export_sms_{start}_{end}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Export_{eventId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Export/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Export/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Export/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Export/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Export/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Export/{eventId}`

<h3 id="get__api_export_{eventid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|

<h3 id="get__api_export_{eventid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-health">Health</h1>

## get__api_Health

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Health");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Health", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Health");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Health HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Health")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Health`

<h3 id="get__api_health-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Health_accessCache

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Health/accessCache");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Health/accessCache", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Health/accessCache");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Health/accessCache HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Health/accessCache")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Health/accessCache`

<h3 id="get__api_health_accesscache-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Health_resetCache

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Health/resetCache");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Health/resetCache", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Health/resetCache");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Health/resetCache HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Health/resetCache")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Health/resetCache`

<h3 id="get__api_health_resetcache-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Health_seedInitial

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Health/seedInitial");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Health/seedInitial", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Health/seedInitial");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Health/seedInitial HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Health/seedInitial")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Health/seedInitial`

<h3 id="get__api_health_seedinitial-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Health_seedEvents

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Health/seedEvents");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Health/seedEvents", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Health/seedEvents");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Health/seedEvents HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Health/seedEvents")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Health/seedEvents`

<h3 id="get__api_health_seedevents-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Health_seedApplications

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Health/seedApplications");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Health/seedApplications", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Health/seedApplications");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Health/seedApplications HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Health/seedApplications")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Health/seedApplications`

<h3 id="get__api_health_seedapplications-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Health_upsertVerificationTemplate

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Health/upsertVerificationTemplate");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Health/upsertVerificationTemplate", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Health/upsertVerificationTemplate");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Health/upsertVerificationTemplate HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Health/upsertVerificationTemplate")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Health/upsertVerificationTemplate`

<h3 id="get__api_health_upsertverificationtemplate-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|environment|query|string|false|none|
|baseUrl|query|string|false|none|

<h3 id="get__api_health_upsertverificationtemplate-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Health_updateEventPresentationFormData_{eventIdOrSlug}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Health/updateEventPresentationFormData/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Health/updateEventPresentationFormData/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Health/updateEventPresentationFormData/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Health/updateEventPresentationFormData/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Health/updateEventPresentationFormData/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Health/updateEventPresentationFormData/{eventIdOrSlug}`

<h3 id="get__api_health_updateeventpresentationformdata_{eventidorslug}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|

<h3 id="get__api_health_updateeventpresentationformdata_{eventidorslug}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Health_recalcaulteAutomaticRegistrationGroupsUsers

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Health/recalcaulteAutomaticRegistrationGroupsUsers");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Health/recalcaulteAutomaticRegistrationGroupsUsers", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Health/recalcaulteAutomaticRegistrationGroupsUsers");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Health/recalcaulteAutomaticRegistrationGroupsUsers HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Health/recalcaulteAutomaticRegistrationGroupsUsers")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Health/recalcaulteAutomaticRegistrationGroupsUsers`

<h3 id="get__api_health_recalcaulteautomaticregistrationgroupsusers-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-helptext">HelpText</h1>

## get__api_HelpText_{type}_{key}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/HelpText/0/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/HelpText/0/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/HelpText/0/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/HelpText/0/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/HelpText/0/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/HelpText/{type}/{key}`

<h3 id="get__api_helptext_{type}_{key}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|type|path|[HelpTextType](#schemahelptexttype)|true|none|
|key|path|string|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|type|0|
|type|1|

<h3 id="get__api_helptext_{type}_{key}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_HelpText_{type}_{key}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/HelpText/0/string");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"content\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"content\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/HelpText/0/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"content\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/HelpText/0/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/HelpText/0/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 20

{"content":"string"}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/HelpText/0/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"content\":\"string\"}")
  .asString();
```

`PUT /api/HelpText/{type}/{key}`

> Body parameter

```json
{
  "content": "string"
}
```

<h3 id="put__api_helptext_{type}_{key}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|type|path|[HelpTextType](#schemahelptexttype)|true|none|
|key|path|string|true|none|
|body|body|[HelpTextRequest](#schemahelptextrequest)|false|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|type|0|
|type|1|

<h3 id="put__api_helptext_{type}_{key}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-home">Home</h1>

## get__home_index

> Code samples

```csharp
var client = new RestClient("https://example.com/home/index");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/home/index", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/home/index");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /home/index HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/home/index")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /home/index`

<h3 id="get__home_index-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-infopage">InfoPage</h1>

## get__api_event_{eventIdOrSlug}_info-pages

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/info-pages");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/event/string/info-pages", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/event/string/info-pages");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/event/string/info-pages HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/event/string/info-pages")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/event/{eventIdOrSlug}/info-pages`

<h3 id="get__api_event_{eventidorslug}_info-pages-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|

<h3 id="get__api_event_{eventidorslug}_info-pages-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_event_{eventId}_info-pages_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/info-pages/string");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("DELETE", "/api/event/string/info-pages/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/event/string/info-pages/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/event/string/info-pages/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/event/string/info-pages/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`DELETE /api/event/{eventId}/info-pages/{entryId}`

<h3 id="delete__api_event_{eventid}_info-pages_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|

<h3 id="delete__api_event_{eventid}_info-pages_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_event_{eventId}_info-pages_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/info-pages/string");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"title\":\"string\",\"content\":\"string\",\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"title\":\"string\",\"content\":\"string\",\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/event/string/info-pages/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"title\":\"string\",\"content\":\"string\",\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/event/string/info-pages/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/event/string/info-pages/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 103

{"id":"string","title":"string","content":"string","order":0,"groupIds":["string"],"platformPages":[0]}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/event/string/info-pages/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"title\":\"string\",\"content\":\"string\",\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}")
  .asString();
```

`PUT /api/event/{eventId}/info-pages/{entryId}`

> Body parameter

```json
{
  "id": "string",
  "title": "string",
  "content": "string",
  "order": 0,
  "groupIds": [
    "string"
  ],
  "platformPages": [
    0
  ]
}
```

<h3 id="put__api_event_{eventid}_info-pages_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|
|body|body|[InfoPageDto](#schemainfopagedto)|false|none|

<h3 id="put__api_event_{eventid}_info-pages_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## patch__api_event_{eventId}_info-pages_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/info-pages/string");
var request = new RestRequest(Method.PATCH);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"title\":\"string\",\"content\":\"string\",\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"title\":\"string\",\"content\":\"string\",\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PATCH", "/api/event/string/info-pages/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"title\":\"string\",\"content\":\"string\",\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PATCH", "https://example.com/api/event/string/info-pages/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PATCH /api/event/string/info-pages/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 89

{"title":"string","content":"string","order":0,"groupIds":["string"],"platformPages":[0]}
```

```java
HttpResponse<String> response = Unirest.patch("https://example.com/api/event/string/info-pages/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"title\":\"string\",\"content\":\"string\",\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}")
  .asString();
```

`PATCH /api/event/{eventId}/info-pages/{entryId}`

> Body parameter

```json
{
  "title": "string",
  "content": "string",
  "order": 0,
  "groupIds": [
    "string"
  ],
  "platformPages": [
    0
  ]
}
```

<h3 id="patch__api_event_{eventid}_info-pages_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|
|body|body|[PartialInfoPageDto](#schemapartialinfopagedto)|false|none|

<h3 id="patch__api_event_{eventid}_info-pages_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_event_{eventId}_info-pages_create

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/info-pages/create");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"title\":\"string\",\"content\":\"string\",\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"title\":\"string\",\"content\":\"string\",\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/event/string/info-pages/create", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"title\":\"string\",\"content\":\"string\",\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/event/string/info-pages/create");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/event/string/info-pages/create HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 103

{"id":"string","title":"string","content":"string","order":0,"groupIds":["string"],"platformPages":[0]}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/event/string/info-pages/create")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"title\":\"string\",\"content\":\"string\",\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}")
  .asString();
```

`POST /api/event/{eventId}/info-pages/create`

> Body parameter

```json
{
  "id": "string",
  "title": "string",
  "content": "string",
  "order": 0,
  "groupIds": [
    "string"
  ],
  "platformPages": [
    0
  ]
}
```

<h3 id="post__api_event_{eventid}_info-pages_create-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[InfoPageDto](#schemainfopagedto)|false|none|

<h3 id="post__api_event_{eventid}_info-pages_create-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## patch__api_event_{eventId}_info-pages_reorder

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/info-pages/reorder");
var request = new RestRequest(Method.PATCH);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"infoPageIds\":[\"string\"]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"infoPageIds\":[\"string\"]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PATCH", "/api/event/string/info-pages/reorder", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"infoPageIds\":[\"string\"]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PATCH", "https://example.com/api/event/string/info-pages/reorder");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PATCH /api/event/string/info-pages/reorder HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 26

{"infoPageIds":["string"]}
```

```java
HttpResponse<String> response = Unirest.patch("https://example.com/api/event/string/info-pages/reorder")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"infoPageIds\":[\"string\"]}")
  .asString();
```

`PATCH /api/event/{eventId}/info-pages/reorder`

> Body parameter

```json
{
  "infoPageIds": [
    "string"
  ]
}
```

<h3 id="patch__api_event_{eventid}_info-pages_reorder-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[ReorderInfoPageDto](#schemareorderinfopagedto)|false|none|

<h3 id="patch__api_event_{eventid}_info-pages_reorder-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-integration">Integration</h1>

## get__api_Integration_workspaces

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Integration/workspaces");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Integration/workspaces", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Integration/workspaces");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Integration/workspaces HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Integration/workspaces")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Integration/workspaces`

<h3 id="get__api_integration_workspaces-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Integration_workspaces_{workspaceId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Integration/workspaces/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Integration/workspaces/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Integration/workspaces/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Integration/workspaces/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Integration/workspaces/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Integration/workspaces/{workspaceId}`

<h3 id="get__api_integration_workspaces_{workspaceid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|workspaceId|path|string|true|none|

<h3 id="get__api_integration_workspaces_{workspaceid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Integration_event_{eventId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Integration/event/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Integration/event/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Integration/event/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Integration/event/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Integration/event/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Integration/event/{eventId}`

<h3 id="get__api_integration_event_{eventid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|

<h3 id="get__api_integration_event_{eventid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Integration_{destination}_clients

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Integration/0/clients");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Integration/0/clients", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Integration/0/clients");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Integration/0/clients HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Integration/0/clients")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Integration/{destination}/clients`

<h3 id="get__api_integration_{destination}_clients-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|destination|path|[IntegrationDestination](#schemaintegrationdestination)|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|destination|0|
|destination|1|

<h3 id="get__api_integration_{destination}_clients-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Integration_{destination}_workspaceClientLinks

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Integration/0/workspaceClientLinks");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Integration/0/workspaceClientLinks", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Integration/0/workspaceClientLinks");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Integration/0/workspaceClientLinks HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Integration/0/workspaceClientLinks")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Integration/{destination}/workspaceClientLinks`

<h3 id="get__api_integration_{destination}_workspaceclientlinks-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|destination|path|[IntegrationDestination](#schemaintegrationdestination)|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|destination|0|
|destination|1|

<h3 id="get__api_integration_{destination}_workspaceclientlinks-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Integration_{destination}_link

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Integration/0/link");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"clientId\":\"string\",\"workspaceId\":\"string\",\"name\":\"string\",\"eventCount\":0,\"isUnlink\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"clientId\":\"string\",\"workspaceId\":\"string\",\"name\":\"string\",\"eventCount\":0,\"isUnlink\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Integration/0/link", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"clientId\":\"string\",\"workspaceId\":\"string\",\"name\":\"string\",\"eventCount\":0,\"isUnlink\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Integration/0/link");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Integration/0/link HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 91

{"clientId":"string","workspaceId":"string","name":"string","eventCount":0,"isUnlink":true}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Integration/0/link")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"clientId\":\"string\",\"workspaceId\":\"string\",\"name\":\"string\",\"eventCount\":0,\"isUnlink\":true}")
  .asString();
```

`POST /api/Integration/{destination}/link`

> Body parameter

```json
{
  "clientId": "string",
  "workspaceId": "string",
  "name": "string",
  "eventCount": 0,
  "isUnlink": true
}
```

<h3 id="post__api_integration_{destination}_link-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|destination|path|[IntegrationDestination](#schemaintegrationdestination)|true|none|
|body|body|[WorkspaceClientLinkDto](#schemaworkspaceclientlinkdto)|false|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|destination|0|
|destination|1|

<h3 id="post__api_integration_{destination}_link-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Integration_{destination}_{workspaceId}_eventLinks

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Integration/0/string/eventLinks");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Integration/0/string/eventLinks", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Integration/0/string/eventLinks");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Integration/0/string/eventLinks HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Integration/0/string/eventLinks")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Integration/{destination}/{workspaceId}/eventLinks`

<h3 id="get__api_integration_{destination}_{workspaceid}_eventlinks-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|destination|path|[IntegrationDestination](#schemaintegrationdestination)|true|none|
|workspaceId|path|string|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|destination|0|
|destination|1|

<h3 id="get__api_integration_{destination}_{workspaceid}_eventlinks-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Integration_{destination}_linkEvent

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Integration/0/linkEvent");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"destination\":0,\"eventId\":\"string\",\"externalEventId\":\"string\",\"externalEventName\":\"string\",\"isUnlink\":true,\"message\":\"string\",\"stackTraceLines\":[\"string\"]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"destination\":0,\"eventId\":\"string\",\"externalEventId\":\"string\",\"externalEventName\":\"string\",\"isUnlink\":true,\"message\":\"string\",\"stackTraceLines\":[\"string\"]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Integration/0/linkEvent", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"destination\":0,\"eventId\":\"string\",\"externalEventId\":\"string\",\"externalEventName\":\"string\",\"isUnlink\":true,\"message\":\"string\",\"stackTraceLines\":[\"string\"]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Integration/0/linkEvent");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Integration/0/linkEvent HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 156

{"destination":0,"eventId":"string","externalEventId":"string","externalEventName":"string","isUnlink":true,"message":"string","stackTraceLines":["string"]}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Integration/0/linkEvent")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"destination\":0,\"eventId\":\"string\",\"externalEventId\":\"string\",\"externalEventName\":\"string\",\"isUnlink\":true,\"message\":\"string\",\"stackTraceLines\":[\"string\"]}")
  .asString();
```

`POST /api/Integration/{destination}/linkEvent`

> Body parameter

```json
{
  "destination": 0,
  "eventId": "string",
  "externalEventId": "string",
  "externalEventName": "string",
  "isUnlink": true,
  "message": "string",
  "stackTraceLines": [
    "string"
  ]
}
```

<h3 id="post__api_integration_{destination}_linkevent-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|destination|path|[IntegrationDestination](#schemaintegrationdestination)|true|none|
|body|body|[EventLinkDto](#schemaeventlinkdto)|false|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|destination|0|
|destination|1|

<h3 id="post__api_integration_{destination}_linkevent-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Integration_{destination}_{workspaceId}_externalEvents

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Integration/0/string/externalEvents");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Integration/0/string/externalEvents", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Integration/0/string/externalEvents");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Integration/0/string/externalEvents HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Integration/0/string/externalEvents")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Integration/{destination}/{workspaceId}/externalEvents`

<h3 id="get__api_integration_{destination}_{workspaceid}_externalevents-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|destination|path|[IntegrationDestination](#schemaintegrationdestination)|true|none|
|workspaceId|path|string|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|destination|0|
|destination|1|

<h3 id="get__api_integration_{destination}_{workspaceid}_externalevents-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Integration_{destination}_{eventId}_registrationLinks

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Integration/0/string/registrationLinks");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Integration/0/string/registrationLinks", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Integration/0/string/registrationLinks");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Integration/0/string/registrationLinks HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Integration/0/string/registrationLinks")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Integration/{destination}/{eventId}/registrationLinks`

<h3 id="get__api_integration_{destination}_{eventid}_registrationlinks-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|destination|path|[IntegrationDestination](#schemaintegrationdestination)|true|none|
|eventId|path|string|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|destination|0|
|destination|1|

<h3 id="get__api_integration_{destination}_{eventid}_registrationlinks-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Integration_{destination}_linkRegistrations

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Integration/0/linkRegistrations");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"eventId\":\"string\",\"registrationIds\":[\"string\"],\"userId\":\"string\",\"parentId\":\"string\",\"isUnlink\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"eventId\":\"string\",\"registrationIds\":[\"string\"],\"userId\":\"string\",\"parentId\":\"string\",\"isUnlink\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Integration/0/linkRegistrations", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"eventId\":\"string\",\"registrationIds\":[\"string\"],\"userId\":\"string\",\"parentId\":\"string\",\"isUnlink\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Integration/0/linkRegistrations");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Integration/0/linkRegistrations HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 103

{"eventId":"string","registrationIds":["string"],"userId":"string","parentId":"string","isUnlink":true}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Integration/0/linkRegistrations")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"eventId\":\"string\",\"registrationIds\":[\"string\"],\"userId\":\"string\",\"parentId\":\"string\",\"isUnlink\":true}")
  .asString();
```

`POST /api/Integration/{destination}/linkRegistrations`

> Body parameter

```json
{
  "eventId": "string",
  "registrationIds": [
    "string"
  ],
  "userId": "string",
  "parentId": "string",
  "isUnlink": true
}
```

<h3 id="post__api_integration_{destination}_linkregistrations-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|destination|path|[IntegrationDestination](#schemaintegrationdestination)|true|none|
|body|body|[RegistrationsLinkDto](#schemaregistrationslinkdto)|false|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|destination|0|
|destination|1|

<h3 id="post__api_integration_{destination}_linkregistrations-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Integration_{destination}_linkRegistration

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Integration/0/linkRegistration");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"eventId\":\"string\",\"registrationId\":\"string\",\"parentId\":\"string\",\"userId\":\"string\",\"isUnlink\":true,\"message\":\"string\",\"stackTraceLines\":[\"string\"]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"eventId\":\"string\",\"registrationId\":\"string\",\"parentId\":\"string\",\"userId\":\"string\",\"isUnlink\":true,\"message\":\"string\",\"stackTraceLines\":[\"string\"]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Integration/0/linkRegistration", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"eventId\":\"string\",\"registrationId\":\"string\",\"parentId\":\"string\",\"userId\":\"string\",\"isUnlink\":true,\"message\":\"string\",\"stackTraceLines\":[\"string\"]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Integration/0/linkRegistration");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Integration/0/linkRegistration HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 148

{"eventId":"string","registrationId":"string","parentId":"string","userId":"string","isUnlink":true,"message":"string","stackTraceLines":["string"]}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Integration/0/linkRegistration")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"eventId\":\"string\",\"registrationId\":\"string\",\"parentId\":\"string\",\"userId\":\"string\",\"isUnlink\":true,\"message\":\"string\",\"stackTraceLines\":[\"string\"]}")
  .asString();
```

`POST /api/Integration/{destination}/linkRegistration`

> Body parameter

```json
{
  "eventId": "string",
  "registrationId": "string",
  "parentId": "string",
  "userId": "string",
  "isUnlink": true,
  "message": "string",
  "stackTraceLines": [
    "string"
  ]
}
```

<h3 id="post__api_integration_{destination}_linkregistration-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|destination|path|[IntegrationDestination](#schemaintegrationdestination)|true|none|
|body|body|[RegistrationLinkRequest](#schemaregistrationlinkrequest)|false|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|destination|0|
|destination|1|

<h3 id="post__api_integration_{destination}_linkregistration-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-livedocument">LiveDocument</h1>

## get__api_event_{eventIdOrSlug}_documents

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/documents");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/event/string/documents", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/event/string/documents");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/event/string/documents HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/event/string/documents")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/event/{eventIdOrSlug}/documents`

<h3 id="get__api_event_{eventidorslug}_documents-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|

<h3 id="get__api_event_{eventidorslug}_documents-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_event_{eventId}_documents_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/documents/string");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("DELETE", "/api/event/string/documents/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/event/string/documents/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/event/string/documents/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/event/string/documents/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`DELETE /api/event/{eventId}/documents/{entryId}`

<h3 id="delete__api_event_{eventid}_documents_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|

<h3 id="delete__api_event_{eventid}_documents_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_event_{eventId}_documents_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/documents/string");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"title\":\"string\",\"description\":\"string\",\"documentUrl\":\"string\",\"isHidden\":true,\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"title\":\"string\",\"description\":\"string\",\"documentUrl\":\"string\",\"isHidden\":true,\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/event/string/documents/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"title\":\"string\",\"description\":\"string\",\"documentUrl\":\"string\",\"isHidden\":true,\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/event/string/documents/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/event/string/documents/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 181

{"id":"string","createdOn":"2019-08-24T14:15:22Z","title":"string","description":"string","documentUrl":"string","isHidden":true,"order":0,"groupIds":["string"],"platformPages":[0]}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/event/string/documents/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"title\":\"string\",\"description\":\"string\",\"documentUrl\":\"string\",\"isHidden\":true,\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}")
  .asString();
```

`PUT /api/event/{eventId}/documents/{entryId}`

> Body parameter

```json
{
  "id": "string",
  "createdOn": "2019-08-24T14:15:22Z",
  "title": "string",
  "description": "string",
  "documentUrl": "string",
  "isHidden": true,
  "order": 0,
  "groupIds": [
    "string"
  ],
  "platformPages": [
    0
  ]
}
```

<h3 id="put__api_event_{eventid}_documents_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|
|body|body|[AdminLiveDocumentDto](#schemaadminlivedocumentdto)|false|none|

<h3 id="put__api_event_{eventid}_documents_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## patch__api_event_{eventId}_documents_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/documents/string");
var request = new RestRequest(Method.PATCH);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"title\":\"string\",\"description\":\"string\",\"documentUrl\":\"string\",\"isHidden\":true,\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"title\":\"string\",\"description\":\"string\",\"documentUrl\":\"string\",\"isHidden\":true,\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PATCH", "/api/event/string/documents/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"title\":\"string\",\"description\":\"string\",\"documentUrl\":\"string\",\"isHidden\":true,\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PATCH", "https://example.com/api/event/string/documents/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PATCH /api/event/string/documents/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 132

{"title":"string","description":"string","documentUrl":"string","isHidden":true,"order":0,"groupIds":["string"],"platformPages":[0]}
```

```java
HttpResponse<String> response = Unirest.patch("https://example.com/api/event/string/documents/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"title\":\"string\",\"description\":\"string\",\"documentUrl\":\"string\",\"isHidden\":true,\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}")
  .asString();
```

`PATCH /api/event/{eventId}/documents/{entryId}`

> Body parameter

```json
{
  "title": "string",
  "description": "string",
  "documentUrl": "string",
  "isHidden": true,
  "order": 0,
  "groupIds": [
    "string"
  ],
  "platformPages": [
    0
  ]
}
```

<h3 id="patch__api_event_{eventid}_documents_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|
|body|body|[PartialLiveDocumentDto](#schemapartiallivedocumentdto)|false|none|

<h3 id="patch__api_event_{eventid}_documents_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_event_{eventId}_documents_create

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/documents/create");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"title\":\"string\",\"description\":\"string\",\"documentUrl\":\"string\",\"isHidden\":true,\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"title\":\"string\",\"description\":\"string\",\"documentUrl\":\"string\",\"isHidden\":true,\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/event/string/documents/create", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"title\":\"string\",\"description\":\"string\",\"documentUrl\":\"string\",\"isHidden\":true,\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/event/string/documents/create");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/event/string/documents/create HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 181

{"id":"string","createdOn":"2019-08-24T14:15:22Z","title":"string","description":"string","documentUrl":"string","isHidden":true,"order":0,"groupIds":["string"],"platformPages":[0]}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/event/string/documents/create")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"title\":\"string\",\"description\":\"string\",\"documentUrl\":\"string\",\"isHidden\":true,\"order\":0,\"groupIds\":[\"string\"],\"platformPages\":[0]}")
  .asString();
```

`POST /api/event/{eventId}/documents/create`

> Body parameter

```json
{
  "id": "string",
  "createdOn": "2019-08-24T14:15:22Z",
  "title": "string",
  "description": "string",
  "documentUrl": "string",
  "isHidden": true,
  "order": 0,
  "groupIds": [
    "string"
  ],
  "platformPages": [
    0
  ]
}
```

<h3 id="post__api_event_{eventid}_documents_create-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[AdminLiveDocumentDto](#schemaadminlivedocumentdto)|false|none|

<h3 id="post__api_event_{eventid}_documents_create-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## patch__api_event_{eventId}_documents_reorder

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/documents/reorder");
var request = new RestRequest(Method.PATCH);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"documentIds\":[\"string\"]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"documentIds\":[\"string\"]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PATCH", "/api/event/string/documents/reorder", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"documentIds\":[\"string\"]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PATCH", "https://example.com/api/event/string/documents/reorder");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PATCH /api/event/string/documents/reorder HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 26

{"documentIds":["string"]}
```

```java
HttpResponse<String> response = Unirest.patch("https://example.com/api/event/string/documents/reorder")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"documentIds\":[\"string\"]}")
  .asString();
```

`PATCH /api/event/{eventId}/documents/reorder`

> Body parameter

```json
{
  "documentIds": [
    "string"
  ]
}
```

<h3 id="patch__api_event_{eventid}_documents_reorder-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[ReorderLiveDocumentDto](#schemareorderlivedocumentdto)|false|none|

<h3 id="patch__api_event_{eventid}_documents_reorder-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-liveevent">LiveEvent</h1>

## get__api_LiveEvent_publicEventInfo_{eventIdOrSlug}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/publicEventInfo/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/publicEventInfo/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/publicEventInfo/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/publicEventInfo/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/publicEventInfo/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/publicEventInfo/{eventIdOrSlug}`

<h3 id="get__api_liveevent_publiceventinfo_{eventidorslug}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|

<h3 id="get__api_liveevent_publiceventinfo_{eventidorslug}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_getEventInfo

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/getEventInfo");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/getEventInfo", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/getEventInfo");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/getEventInfo HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/getEventInfo")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/getEventInfo`

<h3 id="get__api_liveevent_geteventinfo-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_resetPassword_{email}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/resetPassword/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/resetPassword/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/resetPassword/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/resetPassword/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/resetPassword/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/resetPassword/{email}`

<h3 id="get__api_liveevent_{eventslug}_resetpassword_{email}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|email|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_resetpassword_{email}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_getOwnUserInfoFromSession

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/getOwnUserInfoFromSession");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/getOwnUserInfoFromSession", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/getOwnUserInfoFromSession");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/getOwnUserInfoFromSession HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/getOwnUserInfoFromSession")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/getOwnUserInfoFromSession`

<h3 id="get__api_liveevent_{eventslug}_getownuserinfofromsession-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_getownuserinfofromsession-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_generateSignedCookies

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/generateSignedCookies");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/generateSignedCookies", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/generateSignedCookies");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/generateSignedCookies HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/generateSignedCookies")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/generateSignedCookies`

<h3 id="get__api_liveevent_generatesignedcookies-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_eventInfo_{pollAccessKey}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/eventInfo/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/eventInfo/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/eventInfo/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/eventInfo/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/eventInfo/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/eventInfo/{pollAccessKey}`

<h3 id="get__api_liveevent_{eventslug}_eventinfo_{pollaccesskey}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|pollAccessKey|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_eventinfo_{pollaccesskey}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_getAllUsers

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/getAllUsers");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/getAllUsers", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/getAllUsers");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/getAllUsers HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/getAllUsers")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/getAllUsers`

<h3 id="get__api_liveevent_{eventslug}_getallusers-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_getallusers-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_liveGetSpeakerInfo

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/liveGetSpeakerInfo");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/liveGetSpeakerInfo", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/liveGetSpeakerInfo");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/liveGetSpeakerInfo HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/liveGetSpeakerInfo")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/liveGetSpeakerInfo`

<h3 id="get__api_liveevent_{eventslug}_livegetspeakerinfo-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_livegetspeakerinfo-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_LiveEvent_{eventSlug}_sendContactMessage

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/sendContactMessage");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"sponsorId\":\"string\",\"message\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"sponsorId\":\"string\",\"message\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/LiveEvent/string/sendContactMessage", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"sponsorId\":\"string\",\"message\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/LiveEvent/string/sendContactMessage");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/LiveEvent/string/sendContactMessage HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 41

{"sponsorId":"string","message":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/LiveEvent/string/sendContactMessage")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"sponsorId\":\"string\",\"message\":\"string\"}")
  .asString();
```

`POST /api/LiveEvent/{eventSlug}/sendContactMessage`

> Body parameter

```json
{
  "sponsorId": "string",
  "message": "string"
}
```

<h3 id="post__api_liveevent_{eventslug}_sendcontactmessage-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|body|body|[SendContactRequest](#schemasendcontactrequest)|false|none|

<h3 id="post__api_liveevent_{eventslug}_sendcontactmessage-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_sponsors

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/sponsors");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/sponsors", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/sponsors");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/sponsors HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/sponsors")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/sponsors`

<h3 id="get__api_liveevent_{eventslug}_sponsors-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_sponsors-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_sponsors_categories

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/sponsors/categories");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/sponsors/categories", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/sponsors/categories");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/sponsors/categories HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/sponsors/categories")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/sponsors/categories`

<h3 id="get__api_liveevent_{eventslug}_sponsors_categories-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_sponsors_categories-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_sponsors_{sponsorId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/sponsors/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/sponsors/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/sponsors/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/sponsors/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/sponsors/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/sponsors/{sponsorId}`

<h3 id="get__api_liveevent_{eventslug}_sponsors_{sponsorid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|sponsorId|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_sponsors_{sponsorid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_sponsors_{sponsorId}_wherebyRooms

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/sponsors/string/wherebyRooms");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/sponsors/string/wherebyRooms", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/sponsors/string/wherebyRooms");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/sponsors/string/wherebyRooms HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/sponsors/string/wherebyRooms")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/sponsors/{sponsorId}/wherebyRooms`

<h3 id="get__api_liveevent_{eventslug}_sponsors_{sponsorid}_wherebyrooms-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|sponsorId|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_sponsors_{sponsorid}_wherebyrooms-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_sponsors_{sponsorId}_users

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/sponsors/string/users");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/sponsors/string/users", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/sponsors/string/users");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/sponsors/string/users HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/sponsors/string/users")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/sponsors/{sponsorId}/users`

<h3 id="get__api_liveevent_{eventslug}_sponsors_{sponsorid}_users-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|sponsorId|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_sponsors_{sponsorid}_users-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_sponsors_{sponsorId}_polls

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/sponsors/string/polls");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/sponsors/string/polls", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/sponsors/string/polls");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/sponsors/string/polls HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/sponsors/string/polls")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/sponsors/{sponsorId}/polls`

<h3 id="get__api_liveevent_{eventslug}_sponsors_{sponsorid}_polls-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|sponsorId|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_sponsors_{sponsorid}_polls-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_sponsors_{sponsorId}_quizzes

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/sponsors/string/quizzes");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/sponsors/string/quizzes", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/sponsors/string/quizzes");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/sponsors/string/quizzes HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/sponsors/string/quizzes")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/sponsors/{sponsorId}/quizzes`

<h3 id="get__api_liveevent_{eventslug}_sponsors_{sponsorid}_quizzes-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|sponsorId|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_sponsors_{sponsorid}_quizzes-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_sponsors_{sponsorId}_documents

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/sponsors/string/documents");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/sponsors/string/documents", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/sponsors/string/documents");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/sponsors/string/documents HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/sponsors/string/documents")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/sponsors/{sponsorId}/documents`

<h3 id="get__api_liveevent_{eventslug}_sponsors_{sponsorid}_documents-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|sponsorId|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_sponsors_{sponsorid}_documents-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_requestMeeting_{userId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/requestMeeting/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/requestMeeting/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/requestMeeting/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/requestMeeting/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/requestMeeting/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/requestMeeting/{userId}`

<h3 id="get__api_liveevent_{eventslug}_requestmeeting_{userid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|userId|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_requestmeeting_{userid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_getAllDocuments

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/getAllDocuments");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/getAllDocuments", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/getAllDocuments");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/getAllDocuments HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/getAllDocuments")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/getAllDocuments`

<h3 id="get__api_liveevent_{eventslug}_getalldocuments-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_getalldocuments-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_getDocument_{documentId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/getDocument/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/getDocument/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/getDocument/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/getDocument/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/getDocument/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/getDocument/{documentId}`

<h3 id="get__api_liveevent_{eventslug}_getdocument_{documentid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|documentId|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_getdocument_{documentid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_getInfoPages

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/getInfoPages");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/getInfoPages", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/getInfoPages");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/getInfoPages HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/getInfoPages")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/getInfoPages`

<h3 id="get__api_liveevent_{eventslug}_getinfopages-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_getinfopages-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_getPage_{pageId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/getPage/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/getPage/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/getPage/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/getPage/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/getPage/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/getPage/{pageId}`

<h3 id="get__api_liveevent_{eventslug}_getpage_{pageid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|pageId|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_getpage_{pageid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_getPagesByCategoryID_{categoryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/getPagesByCategoryID/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/getPagesByCategoryID/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/getPagesByCategoryID/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/getPagesByCategoryID/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/getPagesByCategoryID/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/getPagesByCategoryID/{categoryId}`

<h3 id="get__api_liveevent_{eventslug}_getpagesbycategoryid_{categoryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|categoryId|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_getpagesbycategoryid_{categoryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_liveGetAgendaInfo

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/liveGetAgendaInfo");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/liveGetAgendaInfo", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/liveGetAgendaInfo");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/liveGetAgendaInfo HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/liveGetAgendaInfo")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/liveGetAgendaInfo`

<h3 id="get__api_liveevent_{eventslug}_livegetagendainfo-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_livegetagendainfo-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_LiveEvent_{eventId}_storeTermsAcceptance_{email}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/storeTermsAcceptance/string");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"termsText\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"termsText\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/LiveEvent/string/storeTermsAcceptance/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"termsText\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/LiveEvent/string/storeTermsAcceptance/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/LiveEvent/string/storeTermsAcceptance/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 22

{"termsText":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/LiveEvent/string/storeTermsAcceptance/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"termsText\":\"string\"}")
  .asString();
```

`POST /api/LiveEvent/{eventId}/storeTermsAcceptance/{email}`

> Body parameter

```json
{
  "termsText": "string"
}
```

<h3 id="post__api_liveevent_{eventid}_storetermsacceptance_{email}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|email|path|string|true|none|
|body|body|[TermsAcceptanceRequest](#schematermsacceptancerequest)|false|none|

<h3 id="post__api_liveevent_{eventid}_storetermsacceptance_{email}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventId}_getTermsText_{email}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/getTermsText/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/getTermsText/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/getTermsText/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/getTermsText/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/getTermsText/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventId}/getTermsText/{email}`

<h3 id="get__api_liveevent_{eventid}_gettermstext_{email}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|email|path|string|true|none|

<h3 id="get__api_liveevent_{eventid}_gettermstext_{email}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventId}_getAllTimelineItems_{limit}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/getAllTimelineItems/0");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/getAllTimelineItems/0", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/getAllTimelineItems/0");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/getAllTimelineItems/0 HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/getAllTimelineItems/0")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventId}/getAllTimelineItems/{limit}`

<h3 id="get__api_liveevent_{eventid}_getalltimelineitems_{limit}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|limit|path|integer(int32)|true|none|

<h3 id="get__api_liveevent_{eventid}_getalltimelineitems_{limit}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventId}_getPromotedTimelineItems

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/getPromotedTimelineItems");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/getPromotedTimelineItems", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/getPromotedTimelineItems");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/getPromotedTimelineItems HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/getPromotedTimelineItems")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventId}/getPromotedTimelineItems`

<h3 id="get__api_liveevent_{eventid}_getpromotedtimelineitems-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|

<h3 id="get__api_liveevent_{eventid}_getpromotedtimelineitems-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_LiveEvent_{eventId}_addTimelineEntry

> Code samples

`POST /api/LiveEvent/{eventId}/addTimelineEntry`

> Body parameter

```yaml
message: string
files:
  - string

```

<h3 id="post__api_liveevent_{eventid}_addtimelineentry-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|object|false|none|
|» message|body|string|false|none|
|» files|body|[string]|false|none|

<h3 id="post__api_liveevent_{eventid}_addtimelineentry-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_LiveEvent_{eventSlug}_addTimelineComment

> Code samples

`POST /api/LiveEvent/{eventSlug}/addTimelineComment`

> Body parameter

```yaml
inReplyTo: string
message: string
files:
  - string

```

<h3 id="post__api_liveevent_{eventslug}_addtimelinecomment-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|body|body|object|false|none|
|» inReplyTo|body|string|false|none|
|» message|body|string|false|none|
|» files|body|[string]|false|none|

<h3 id="post__api_liveevent_{eventslug}_addtimelinecomment-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_LiveEvent_{eventSlug}_deleteTimelineEntry

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/deleteTimelineEntry");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"entryId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"entryId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/LiveEvent/string/deleteTimelineEntry", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"entryId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/LiveEvent/string/deleteTimelineEntry");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/LiveEvent/string/deleteTimelineEntry HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 20

{"entryId":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/LiveEvent/string/deleteTimelineEntry")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"entryId\":\"string\"}")
  .asString();
```

`POST /api/LiveEvent/{eventSlug}/deleteTimelineEntry`

> Body parameter

```json
{
  "entryId": "string"
}
```

<h3 id="post__api_liveevent_{eventslug}_deletetimelineentry-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|body|body|[DeleteTimelineEntryRequest](#schemadeletetimelineentryrequest)|false|none|

<h3 id="post__api_liveevent_{eventslug}_deletetimelineentry-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_LiveEvent_{eventSlug}_likeTimelineEntry

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/likeTimelineEntry");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"entryId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"entryId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/LiveEvent/string/likeTimelineEntry", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"entryId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/LiveEvent/string/likeTimelineEntry");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/LiveEvent/string/likeTimelineEntry HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 20

{"entryId":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/LiveEvent/string/likeTimelineEntry")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"entryId\":\"string\"}")
  .asString();
```

`POST /api/LiveEvent/{eventSlug}/likeTimelineEntry`

> Body parameter

```json
{
  "entryId": "string"
}
```

<h3 id="post__api_liveevent_{eventslug}_liketimelineentry-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|body|body|[LikeTimelineEntryRequest](#schemaliketimelineentryrequest)|false|none|

<h3 id="post__api_liveevent_{eventslug}_liketimelineentry-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_LiveEvent_{eventSlug}_unlikeTimelineEntry

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/unlikeTimelineEntry");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"entryId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"entryId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/LiveEvent/string/unlikeTimelineEntry", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"entryId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/LiveEvent/string/unlikeTimelineEntry");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/LiveEvent/string/unlikeTimelineEntry HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 20

{"entryId":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/LiveEvent/string/unlikeTimelineEntry")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"entryId\":\"string\"}")
  .asString();
```

`POST /api/LiveEvent/{eventSlug}/unlikeTimelineEntry`

> Body parameter

```json
{
  "entryId": "string"
}
```

<h3 id="post__api_liveevent_{eventslug}_unliketimelineentry-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|body|body|[UnlikeTimelineEntryRequest](#schemaunliketimelineentryrequest)|false|none|

<h3 id="post__api_liveevent_{eventslug}_unliketimelineentry-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventId}_liveGetPoll_{pollId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/liveGetPoll/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/liveGetPoll/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/liveGetPoll/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/liveGetPoll/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/liveGetPoll/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventId}/liveGetPoll/{pollId}`

<h3 id="get__api_liveevent_{eventid}_livegetpoll_{pollid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|pollId|path|string|true|none|

<h3 id="get__api_liveevent_{eventid}_livegetpoll_{pollid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventSlug}_pollStream_{pollAccessKey}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/pollStream/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/pollStream/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/pollStream/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/pollStream/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/pollStream/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventSlug}/pollStream/{pollAccessKey}`

<h3 id="get__api_liveevent_{eventslug}_pollstream_{pollaccesskey}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|pollAccessKey|path|string|true|none|

<h3 id="get__api_liveevent_{eventslug}_pollstream_{pollaccesskey}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_LiveEvent_{eventSlug}_togglePollAnswerPresentation_{pollAccessKey}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/togglePollAnswerPresentation/string");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"label\":\"string\",\"presentType\":0}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"label\":\"string\",\"presentType\":0}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/LiveEvent/string/togglePollAnswerPresentation/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"label\":\"string\",\"presentType\":0}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/LiveEvent/string/togglePollAnswerPresentation/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/LiveEvent/string/togglePollAnswerPresentation/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 34

{"label":"string","presentType":0}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/LiveEvent/string/togglePollAnswerPresentation/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"label\":\"string\",\"presentType\":0}")
  .asString();
```

`POST /api/LiveEvent/{eventSlug}/togglePollAnswerPresentation/{pollAccessKey}`

> Body parameter

```json
{
  "label": "string",
  "presentType": 0
}
```

<h3 id="post__api_liveevent_{eventslug}_togglepollanswerpresentation_{pollaccesskey}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|pollAccessKey|path|string|true|none|
|body|body|[TogglePollAnswerPresentationRequest](#schematogglepollanswerpresentationrequest)|false|none|

<h3 id="post__api_liveevent_{eventslug}_togglepollanswerpresentation_{pollaccesskey}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_LiveEvent_{eventSlug}_liveStoreFreeTextAnswer

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/liveStoreFreeTextAnswer");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"pollId\":\"string\",\"label\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"pollId\":\"string\",\"label\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/LiveEvent/string/liveStoreFreeTextAnswer", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"pollId\":\"string\",\"label\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/LiveEvent/string/liveStoreFreeTextAnswer");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/LiveEvent/string/liveStoreFreeTextAnswer HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 36

{"pollId":"string","label":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/LiveEvent/string/liveStoreFreeTextAnswer")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"pollId\":\"string\",\"label\":\"string\"}")
  .asString();
```

`POST /api/LiveEvent/{eventSlug}/liveStoreFreeTextAnswer`

> Body parameter

```json
{
  "pollId": "string",
  "label": "string"
}
```

<h3 id="post__api_liveevent_{eventslug}_livestorefreetextanswer-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|body|body|[StorePollOpenTextAnswerRequest](#schemastorepollopentextanswerrequest)|false|none|

<h3 id="post__api_liveevent_{eventslug}_livestorefreetextanswer-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_LiveEvent_{eventSlug}_liveStorePollAnswer

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/liveStorePollAnswer");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"pollId\":\"string\",\"questionType\":\"string\",\"alternatives\":[\"string\"]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"pollId\":\"string\",\"questionType\":\"string\",\"alternatives\":[\"string\"]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/LiveEvent/string/liveStorePollAnswer", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"pollId\":\"string\",\"questionType\":\"string\",\"alternatives\":[\"string\"]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/LiveEvent/string/liveStorePollAnswer");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/LiveEvent/string/liveStorePollAnswer HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 69

{"pollId":"string","questionType":"string","alternatives":["string"]}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/LiveEvent/string/liveStorePollAnswer")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"pollId\":\"string\",\"questionType\":\"string\",\"alternatives\":[\"string\"]}")
  .asString();
```

`POST /api/LiveEvent/{eventSlug}/liveStorePollAnswer`

> Body parameter

```json
{
  "pollId": "string",
  "questionType": "string",
  "alternatives": [
    "string"
  ]
}
```

<h3 id="post__api_liveevent_{eventslug}_livestorepollanswer-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|body|body|[StorePollAnswerRequest](#schemastorepollanswerrequest)|false|none|

<h3 id="post__api_liveevent_{eventslug}_livestorepollanswer-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_LiveEvent_{eventSlug}_updateUser

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/updateUser");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"userId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"email\":\"string\",\"description\":\"string\",\"company\":\"string\",\"jobTitle\":\"string\",\"fullName\":\"string\",\"phoneNumber\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"userId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"email\":\"string\",\"description\":\"string\",\"company\":\"string\",\"jobTitle\":\"string\",\"fullName\":\"string\",\"phoneNumber\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/LiveEvent/string/updateUser", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"userId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"email\":\"string\",\"description\":\"string\",\"company\":\"string\",\"jobTitle\":\"string\",\"fullName\":\"string\",\"phoneNumber\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/LiveEvent/string/updateUser");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/LiveEvent/string/updateUser HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 177

{"userId":"string","name":"string","lastName":"string","email":"string","description":"string","company":"string","jobTitle":"string","fullName":"string","phoneNumber":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/LiveEvent/string/updateUser")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"userId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"email\":\"string\",\"description\":\"string\",\"company\":\"string\",\"jobTitle\":\"string\",\"fullName\":\"string\",\"phoneNumber\":\"string\"}")
  .asString();
```

`POST /api/LiveEvent/{eventSlug}/updateUser`

> Body parameter

```json
{
  "userId": "string",
  "name": "string",
  "lastName": "string",
  "email": "string",
  "description": "string",
  "company": "string",
  "jobTitle": "string",
  "fullName": "string",
  "phoneNumber": "string"
}
```

<h3 id="post__api_liveevent_{eventslug}_updateuser-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|body|body|[UpdateUserRequest](#schemaupdateuserrequest)|false|none|

<h3 id="post__api_liveevent_{eventslug}_updateuser-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_LiveEvent_{eventSlug}_toggleUserVisibility

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/toggleUserVisibility");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/api/LiveEvent/string/toggleUserVisibility", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/LiveEvent/string/toggleUserVisibility");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/LiveEvent/string/toggleUserVisibility HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/LiveEvent/string/toggleUserVisibility")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /api/LiveEvent/{eventSlug}/toggleUserVisibility`

<h3 id="post__api_liveevent_{eventslug}_toggleuservisibility-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|

<h3 id="post__api_liveevent_{eventslug}_toggleuservisibility-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_LiveEvent_{eventSlug}_uploadUserAvatar

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/uploadUserAvatar");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"imageBase64WithContext\":\"string\",\"fileName\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"imageBase64WithContext\":\"string\",\"fileName\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/LiveEvent/string/uploadUserAvatar", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"imageBase64WithContext\":\"string\",\"fileName\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/LiveEvent/string/uploadUserAvatar");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/LiveEvent/string/uploadUserAvatar HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 55

{"imageBase64WithContext":"string","fileName":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/LiveEvent/string/uploadUserAvatar")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"imageBase64WithContext\":\"string\",\"fileName\":\"string\"}")
  .asString();
```

`POST /api/LiveEvent/{eventSlug}/uploadUserAvatar`

> Body parameter

```json
{
  "imageBase64WithContext": "string",
  "fileName": "string"
}
```

<h3 id="post__api_liveevent_{eventslug}_uploaduseravatar-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventSlug|path|string|true|none|
|body|body|[UpdateUserPictureRequest](#schemaupdateuserpicturerequest)|false|none|

<h3 id="post__api_liveevent_{eventslug}_uploaduseravatar-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventId}_getAllSelfieOverlays

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/getAllSelfieOverlays");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/getAllSelfieOverlays", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/getAllSelfieOverlays");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/getAllSelfieOverlays HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/getAllSelfieOverlays")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventId}/getAllSelfieOverlays`

<h3 id="get__api_liveevent_{eventid}_getallselfieoverlays-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|

<h3 id="get__api_liveevent_{eventid}_getallselfieoverlays-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventId}_getAllOnlineUsers

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/getAllOnlineUsers");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/getAllOnlineUsers", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/getAllOnlineUsers");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/getAllOnlineUsers HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/getAllOnlineUsers")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventId}/getAllOnlineUsers`

<h3 id="get__api_liveevent_{eventid}_getallonlineusers-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|

<h3 id="get__api_liveevent_{eventid}_getallonlineusers-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_{eventId}_chat

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/chat");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/string/chat", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/string/chat");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/string/chat HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/string/chat")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/{eventId}/chat`

<h3 id="get__api_liveevent_{eventid}_chat-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|

<h3 id="get__api_liveevent_{eventid}_chat-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_LiveEvent_{eventId}_chat

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/chat");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"userId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"userId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/LiveEvent/string/chat", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"userId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/LiveEvent/string/chat");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/LiveEvent/string/chat HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 19

{"userId":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/LiveEvent/string/chat")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"userId\":\"string\"}")
  .asString();
```

`POST /api/LiveEvent/{eventId}/chat`

> Body parameter

```json
{
  "userId": "string"
}
```

<h3 id="post__api_liveevent_{eventid}_chat-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[CreateChatRequest](#schemacreatechatrequest)|false|none|

<h3 id="post__api_liveevent_{eventid}_chat-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_LiveEvent_{eventId}_chat_{chatId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/chat/string");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"message\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"message\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/LiveEvent/string/chat/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"message\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/LiveEvent/string/chat/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/LiveEvent/string/chat/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 20

{"message":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/LiveEvent/string/chat/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"message\":\"string\"}")
  .asString();
```

`POST /api/LiveEvent/{eventId}/chat/{chatId}`

> Body parameter

```json
{
  "message": "string"
}
```

<h3 id="post__api_liveevent_{eventid}_chat_{chatid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|chatId|path|string|true|none|
|body|body|[SendMessageRequest](#schemasendmessagerequest)|false|none|

<h3 id="post__api_liveevent_{eventid}_chat_{chatid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_LiveEvent_{eventId}_chat_{chatId}_read

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/string/chat/string/read");
var request = new RestRequest(Method.PUT);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("PUT", "/api/LiveEvent/string/chat/string/read", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/LiveEvent/string/chat/string/read");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/LiveEvent/string/chat/string/read HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/LiveEvent/string/chat/string/read")
  .header("Authorization", "API_KEY")
  .asString();
```

`PUT /api/LiveEvent/{eventId}/chat/{chatId}/read`

<h3 id="put__api_liveevent_{eventid}_chat_{chatid}_read-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|chatId|path|string|true|none|

<h3 id="put__api_liveevent_{eventid}_chat_{chatid}_read-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_LiveEvent_manifest

> Code samples

```csharp
var client = new RestClient("https://example.com/api/LiveEvent/manifest");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/LiveEvent/manifest", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/LiveEvent/manifest");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/LiveEvent/manifest HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/LiveEvent/manifest")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/LiveEvent/manifest`

<h3 id="get__api_liveevent_manifest-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-log">Log</h1>

## post__api_Log_debug

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Log/debug");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/api/Log/debug", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Log/debug");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Log/debug HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Log/debug")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /api/Log/debug`

<h3 id="post__api_log_debug-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|text|query|string|false|none|

<h3 id="post__api_log_debug-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Log_info

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Log/info");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/api/Log/info", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Log/info");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Log/info HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Log/info")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /api/Log/info`

<h3 id="post__api_log_info-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|text|query|string|false|none|

<h3 id="post__api_log_info-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Log_error

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Log/error");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"text\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"text\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Log/error", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"text\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Log/error");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Log/error HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 17

{"text":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Log/error")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"text\":\"string\"}")
  .asString();
```

`POST /api/Log/error`

> Body parameter

```json
{
  "text": "string"
}
```

<h3 id="post__api_log_error-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[ErrorDto](#schemaerrordto)|false|none|

<h3 id="post__api_log_error-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-participants">Participants</h1>

## get__api_Participants_{eventIdOrSlug}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Participants/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Participants/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Participants/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Participants/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Participants/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Participants/{eventIdOrSlug}`

<h3 id="get__api_participants_{eventidorslug}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|
|ValueConverter|query|[IValueConverter](#schemaivalueconverter)|false|none|
|RowIds|query|array[string]|false|none|
|ColumnIds|query|array[string]|false|none|
|Search|query|string|false|none|
|SortBy|query|string|false|none|
|SortAsc|query|boolean|false|none|
|Skip|query|integer(int32)|false|none|
|Take|query|integer(int32)|false|none|
|IsComputedOnServer|query|boolean|false|none|
|IncludeGuests|query|boolean|false|none|
|IncludeParent|query|boolean|false|none|
|GroupFilter|query|string|false|none|
|StatusFilter|query|string|false|none|
|LoggedInFilter|query|boolean|false|none|
|IsProfileVisibleFilter|query|boolean|false|none|
|GroupFilterList|query|array[string]|false|none|
|StatusFilterList|query|array[integer]|false|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|StatusFilterList|0|
|StatusFilterList|1|
|StatusFilterList|2|
|StatusFilterList|3|
|StatusFilterList|4|

<h3 id="get__api_participants_{eventidorslug}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_Participants_{eventId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Participants/string");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"registrationIds\":[\"string\"]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"registrationIds\":[\"string\"]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("DELETE", "/api/Participants/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"registrationIds\":[\"string\"]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/Participants/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/Participants/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 30

{"registrationIds":["string"]}
```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/Participants/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"registrationIds\":[\"string\"]}")
  .asString();
```

`DELETE /api/Participants/{eventId}`

> Body parameter

```json
{
  "registrationIds": [
    "string"
  ]
}
```

<h3 id="delete__api_participants_{eventid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[RegistrationDeleteDto](#schemaregistrationdeletedto)|false|none|

<h3 id="delete__api_participants_{eventid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-partner">Partner</h1>

## get__api_Partner

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Partner");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Partner", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Partner");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Partner HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Partner")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Partner`

<h3 id="get__api_partner-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Partner_create

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Partner/create");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"name\":\"string\",\"companyId\":\"string\",\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"city\":\"string\",\"country\":\"string\",\"email\":\"string\",\"contactName\":\"string\",\"contactLastName\":\"string\",\"contactEmail\":\"string\",\"contactPhone\":\"string\",\"phone\":\"string\",\"invoiceEmail\":\"string\",\"users\":[{\"userId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"email\":\"string\",\"role\":\"string\"}]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"name\":\"string\",\"companyId\":\"string\",\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"city\":\"string\",\"country\":\"string\",\"email\":\"string\",\"contactName\":\"string\",\"contactLastName\":\"string\",\"contactEmail\":\"string\",\"contactPhone\":\"string\",\"phone\":\"string\",\"invoiceEmail\":\"string\",\"users\":[{\"userId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"email\":\"string\",\"role\":\"string\"}]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Partner/create", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"name\":\"string\",\"companyId\":\"string\",\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"city\":\"string\",\"country\":\"string\",\"email\":\"string\",\"contactName\":\"string\",\"contactLastName\":\"string\",\"contactEmail\":\"string\",\"contactPhone\":\"string\",\"phone\":\"string\",\"invoiceEmail\":\"string\",\"users\":[{\"userId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"email\":\"string\",\"role\":\"string\"}]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Partner/create");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Partner/create HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 376

{"name":"string","companyId":"string","addressLine1":"string","addressLine2":"string","city":"string","country":"string","email":"string","contactName":"string","contactLastName":"string","contactEmail":"string","contactPhone":"string","phone":"string","invoiceEmail":"string","users":[{"userId":"string","name":"string","lastName":"string","email":"string","role":"string"}]}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Partner/create")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"name\":\"string\",\"companyId\":\"string\",\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"city\":\"string\",\"country\":\"string\",\"email\":\"string\",\"contactName\":\"string\",\"contactLastName\":\"string\",\"contactEmail\":\"string\",\"contactPhone\":\"string\",\"phone\":\"string\",\"invoiceEmail\":\"string\",\"users\":[{\"userId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"email\":\"string\",\"role\":\"string\"}]}")
  .asString();
```

`POST /api/Partner/create`

> Body parameter

```json
{
  "name": "string",
  "companyId": "string",
  "addressLine1": "string",
  "addressLine2": "string",
  "city": "string",
  "country": "string",
  "email": "string",
  "contactName": "string",
  "contactLastName": "string",
  "contactEmail": "string",
  "contactPhone": "string",
  "phone": "string",
  "invoiceEmail": "string",
  "users": [
    {
      "userId": "string",
      "name": "string",
      "lastName": "string",
      "email": "string",
      "role": "string"
    }
  ]
}
```

<h3 id="post__api_partner_create-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[SavePartnerWorkspaceDto](#schemasavepartnerworkspacedto)|false|none|

<h3 id="post__api_partner_create-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_Partner_{partnerId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Partner/string");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"name\":\"string\",\"companyId\":\"string\",\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"city\":\"string\",\"country\":\"string\",\"email\":\"string\",\"contactName\":\"string\",\"contactLastName\":\"string\",\"contactEmail\":\"string\",\"contactPhone\":\"string\",\"phone\":\"string\",\"invoiceEmail\":\"string\",\"users\":[{\"userId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"email\":\"string\",\"role\":\"string\"}]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"name\":\"string\",\"companyId\":\"string\",\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"city\":\"string\",\"country\":\"string\",\"email\":\"string\",\"contactName\":\"string\",\"contactLastName\":\"string\",\"contactEmail\":\"string\",\"contactPhone\":\"string\",\"phone\":\"string\",\"invoiceEmail\":\"string\",\"users\":[{\"userId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"email\":\"string\",\"role\":\"string\"}]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/Partner/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"name\":\"string\",\"companyId\":\"string\",\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"city\":\"string\",\"country\":\"string\",\"email\":\"string\",\"contactName\":\"string\",\"contactLastName\":\"string\",\"contactEmail\":\"string\",\"contactPhone\":\"string\",\"phone\":\"string\",\"invoiceEmail\":\"string\",\"users\":[{\"userId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"email\":\"string\",\"role\":\"string\"}]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/Partner/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/Partner/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 376

{"name":"string","companyId":"string","addressLine1":"string","addressLine2":"string","city":"string","country":"string","email":"string","contactName":"string","contactLastName":"string","contactEmail":"string","contactPhone":"string","phone":"string","invoiceEmail":"string","users":[{"userId":"string","name":"string","lastName":"string","email":"string","role":"string"}]}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/Partner/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"name\":\"string\",\"companyId\":\"string\",\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"city\":\"string\",\"country\":\"string\",\"email\":\"string\",\"contactName\":\"string\",\"contactLastName\":\"string\",\"contactEmail\":\"string\",\"contactPhone\":\"string\",\"phone\":\"string\",\"invoiceEmail\":\"string\",\"users\":[{\"userId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"email\":\"string\",\"role\":\"string\"}]}")
  .asString();
```

`PUT /api/Partner/{partnerId}`

> Body parameter

```json
{
  "name": "string",
  "companyId": "string",
  "addressLine1": "string",
  "addressLine2": "string",
  "city": "string",
  "country": "string",
  "email": "string",
  "contactName": "string",
  "contactLastName": "string",
  "contactEmail": "string",
  "contactPhone": "string",
  "phone": "string",
  "invoiceEmail": "string",
  "users": [
    {
      "userId": "string",
      "name": "string",
      "lastName": "string",
      "email": "string",
      "role": "string"
    }
  ]
}
```

<h3 id="put__api_partner_{partnerid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|partnerId|path|string|true|none|
|body|body|[SavePartnerWorkspaceDto](#schemasavepartnerworkspacedto)|false|none|

<h3 id="put__api_partner_{partnerid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_Partner_users

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Partner/users");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"partnerId\":\"string\",\"users\":[\"string\"]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"partnerId\":\"string\",\"users\":[\"string\"]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/Partner/users", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"partnerId\":\"string\",\"users\":[\"string\"]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/Partner/users");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/Partner/users HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 41

{"partnerId":"string","users":["string"]}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/Partner/users")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"partnerId\":\"string\",\"users\":[\"string\"]}")
  .asString();
```

`PUT /api/Partner/users`

> Body parameter

```json
{
  "partnerId": "string",
  "users": [
    "string"
  ]
}
```

<h3 id="put__api_partner_users-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[AddPartnerWorkspaceUsersDto](#schemaaddpartnerworkspaceusersdto)|false|none|

<h3 id="put__api_partner_users-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Partner_{partnerIdOrSlug}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Partner/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Partner/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Partner/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Partner/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Partner/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Partner/{partnerIdOrSlug}`

<h3 id="get__api_partner_{partneridorslug}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|partnerIdOrSlug|path|string|true|none|

<h3 id="get__api_partner_{partneridorslug}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_Partner_user

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Partner/user");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"partnerId\":\"string\",\"email\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"partnerId\":\"string\",\"email\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("DELETE", "/api/Partner/user", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"partnerId\":\"string\",\"email\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/Partner/user");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/Partner/user HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 39

{"partnerId":"string","email":"string"}
```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/Partner/user")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"partnerId\":\"string\",\"email\":\"string\"}")
  .asString();
```

`DELETE /api/Partner/user`

> Body parameter

```json
{
  "partnerId": "string",
  "email": "string"
}
```

<h3 id="delete__api_partner_user-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[DeletePartnerWorkspaceUserDto](#schemadeletepartnerworkspaceuserdto)|false|none|

<h3 id="delete__api_partner_user-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-payment">Payment</h1>

## get__api_Payment_check

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Payment/check");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Payment/check", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Payment/check");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Payment/check HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Payment/check")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Payment/check`

<h3 id="get__api_payment_check-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|paymentApiSecret|query|string|false|none|

<h3 id="get__api_payment_check-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Payment_secret_{eventId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Payment/secret/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Payment/secret/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Payment/secret/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Payment/secret/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Payment/secret/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Payment/secret/{eventId}`

<h3 id="get__api_payment_secret_{eventid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|

<h3 id="get__api_payment_secret_{eventid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-poll">Poll</h1>

## get__api_event_{eventIdOrSlug}_polls

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/polls");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/event/string/polls", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/event/string/polls");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/event/string/polls HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/event/string/polls")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/event/{eventIdOrSlug}/polls`

<h3 id="get__api_event_{eventidorslug}_polls-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|

<h3 id="get__api_event_{eventidorslug}_polls-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_event_{eventId}_polls_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/polls/string");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("DELETE", "/api/event/string/polls/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/event/string/polls/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/event/string/polls/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/event/string/polls/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`DELETE /api/event/{eventId}/polls/{entryId}`

<h3 id="delete__api_event_{eventid}_polls_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|

<h3 id="delete__api_event_{eventid}_polls_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_event_{eventId}_polls_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/polls/string");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"title\":\"string\",\"description\":\"string\",\"isPublicResults\":true,\"order\":0,\"pollType\":0}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"title\":\"string\",\"description\":\"string\",\"isPublicResults\":true,\"order\":0,\"pollType\":0}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/event/string/polls/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"title\":\"string\",\"description\":\"string\",\"isPublicResults\":true,\"order\":0,\"pollType\":0}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/event/string/polls/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/event/string/polls/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 101

{"id":"string","title":"string","description":"string","isPublicResults":true,"order":0,"pollType":0}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/event/string/polls/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"title\":\"string\",\"description\":\"string\",\"isPublicResults\":true,\"order\":0,\"pollType\":0}")
  .asString();
```

`PUT /api/event/{eventId}/polls/{entryId}`

> Body parameter

```json
{
  "id": "string",
  "title": "string",
  "description": "string",
  "isPublicResults": true,
  "order": 0,
  "pollType": 0
}
```

<h3 id="put__api_event_{eventid}_polls_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|
|body|body|[PollDto](#schemapolldto)|false|none|

<h3 id="put__api_event_{eventid}_polls_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## patch__api_event_{eventId}_polls_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/polls/string");
var request = new RestRequest(Method.PATCH);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PATCH", "/api/event/string/polls/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PATCH", "https://example.com/api/event/string/polls/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PATCH /api/event/string/polls/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 2

{}
```

```java
HttpResponse<String> response = Unirest.patch("https://example.com/api/event/string/polls/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{}")
  .asString();
```

`PATCH /api/event/{eventId}/polls/{entryId}`

> Body parameter

```json
{}
```

<h3 id="patch__api_event_{eventid}_polls_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|
|body|body|[PartialPollDto](#schemapartialpolldto)|false|none|

<h3 id="patch__api_event_{eventid}_polls_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_event_{eventId}_polls_create

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/polls/create");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"title\":\"string\",\"description\":\"string\",\"isPublicResults\":true,\"order\":0,\"pollType\":0}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"title\":\"string\",\"description\":\"string\",\"isPublicResults\":true,\"order\":0,\"pollType\":0}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/event/string/polls/create", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"title\":\"string\",\"description\":\"string\",\"isPublicResults\":true,\"order\":0,\"pollType\":0}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/event/string/polls/create");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/event/string/polls/create HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 101

{"id":"string","title":"string","description":"string","isPublicResults":true,"order":0,"pollType":0}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/event/string/polls/create")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"title\":\"string\",\"description\":\"string\",\"isPublicResults\":true,\"order\":0,\"pollType\":0}")
  .asString();
```

`POST /api/event/{eventId}/polls/create`

> Body parameter

```json
{
  "id": "string",
  "title": "string",
  "description": "string",
  "isPublicResults": true,
  "order": 0,
  "pollType": 0
}
```

<h3 id="post__api_event_{eventid}_polls_create-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[PollDto](#schemapolldto)|false|none|

<h3 id="post__api_event_{eventid}_polls_create-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## patch__api_event_{eventId}_polls_reorder

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/polls/reorder");
var request = new RestRequest(Method.PATCH);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"pollIds\":[\"string\"]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"pollIds\":[\"string\"]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PATCH", "/api/event/string/polls/reorder", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"pollIds\":[\"string\"]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PATCH", "https://example.com/api/event/string/polls/reorder");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PATCH /api/event/string/polls/reorder HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 22

{"pollIds":["string"]}
```

```java
HttpResponse<String> response = Unirest.patch("https://example.com/api/event/string/polls/reorder")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"pollIds\":[\"string\"]}")
  .asString();
```

`PATCH /api/event/{eventId}/polls/reorder`

> Body parameter

```json
{
  "pollIds": [
    "string"
  ]
}
```

<h3 id="patch__api_event_{eventid}_polls_reorder-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[ReorderPollDto](#schemareorderpolldto)|false|none|

<h3 id="patch__api_event_{eventid}_polls_reorder-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_event_{eventId}_polls_vote

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/polls/vote");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"label\":\"string\",\"pollId\":\"string\",\"answeredBy\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"label\":\"string\",\"pollId\":\"string\",\"answeredBy\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/event/string/polls/vote", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"label\":\"string\",\"pollId\":\"string\",\"answeredBy\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/event/string/polls/vote");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/event/string/polls/vote HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 93

{"label":"string","pollId":"string","answeredBy":"string","createdOn":"2019-08-24T14:15:22Z"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/event/string/polls/vote")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"label\":\"string\",\"pollId\":\"string\",\"answeredBy\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\"}")
  .asString();
```

`POST /api/event/{eventId}/polls/vote`

> Body parameter

```json
{
  "label": "string",
  "pollId": "string",
  "answeredBy": "string",
  "createdOn": "2019-08-24T14:15:22Z"
}
```

<h3 id="post__api_event_{eventid}_polls_vote-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[AdminPollVoteDto](#schemaadminpollvotedto)|false|none|

<h3 id="post__api_event_{eventid}_polls_vote-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_event_{eventId}_polls_{entryId}_reset

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/polls/string/reset");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/event/string/polls/string/reset", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/event/string/polls/string/reset");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/event/string/polls/string/reset HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/event/string/polls/string/reset")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/event/{eventId}/polls/{entryId}/reset`

<h3 id="get__api_event_{eventid}_polls_{entryid}_reset-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|

<h3 id="get__api_event_{eventid}_polls_{entryid}_reset-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-product">Product</h1>

## get__api_Product

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Product");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Product", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Product");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Product HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Product")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Product`

<h3 id="get__api_product-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Product_createPaymentIntent

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Product/createPaymentIntent");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"zipCode\":\"string\",\"state\":\"string\",\"stateCode\":\"string\",\"country\":\"string\",\"city\":\"string\",\"firstName\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"paymentMethodId\":\"string\",\"planName\":\"string\",\"planPriceId\":\"string\",\"totalPrice\":0,\"companyName\":\"string\",\"invoiceEmail\":\"string\",\"vatId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"zipCode\":\"string\",\"state\":\"string\",\"stateCode\":\"string\",\"country\":\"string\",\"city\":\"string\",\"firstName\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"paymentMethodId\":\"string\",\"planName\":\"string\",\"planPriceId\":\"string\",\"totalPrice\":0,\"companyName\":\"string\",\"invoiceEmail\":\"string\",\"vatId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Product/createPaymentIntent", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"zipCode\":\"string\",\"state\":\"string\",\"stateCode\":\"string\",\"country\":\"string\",\"city\":\"string\",\"firstName\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"paymentMethodId\":\"string\",\"planName\":\"string\",\"planPriceId\":\"string\",\"totalPrice\":0,\"companyName\":\"string\",\"invoiceEmail\":\"string\",\"vatId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Product/createPaymentIntent");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Product/createPaymentIntent HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 350

{"addressLine1":"string","addressLine2":"string","zipCode":"string","state":"string","stateCode":"string","country":"string","city":"string","firstName":"string","lastName":"string","company":"string","paymentMethodId":"string","planName":"string","planPriceId":"string","totalPrice":0,"companyName":"string","invoiceEmail":"string","vatId":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Product/createPaymentIntent")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"zipCode\":\"string\",\"state\":\"string\",\"stateCode\":\"string\",\"country\":\"string\",\"city\":\"string\",\"firstName\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"paymentMethodId\":\"string\",\"planName\":\"string\",\"planPriceId\":\"string\",\"totalPrice\":0,\"companyName\":\"string\",\"invoiceEmail\":\"string\",\"vatId\":\"string\"}")
  .asString();
```

`POST /api/Product/createPaymentIntent`

> Body parameter

```json
{
  "addressLine1": "string",
  "addressLine2": "string",
  "zipCode": "string",
  "state": "string",
  "stateCode": "string",
  "country": "string",
  "city": "string",
  "firstName": "string",
  "lastName": "string",
  "company": "string",
  "paymentMethodId": "string",
  "planName": "string",
  "planPriceId": "string",
  "totalPrice": 0,
  "companyName": "string",
  "invoiceEmail": "string",
  "vatId": "string"
}
```

<h3 id="post__api_product_createpaymentintent-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[PortalCreatePaymentIntentRequest](#schemaportalcreatepaymentintentrequest)|false|none|

<h3 id="post__api_product_createpaymentintent-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Product_confirmPaymentIntent

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Product/confirmPaymentIntent");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"paymentIntentId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"paymentIntentId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Product/confirmPaymentIntent", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"paymentIntentId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Product/confirmPaymentIntent");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Product/confirmPaymentIntent HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 28

{"paymentIntentId":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Product/confirmPaymentIntent")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"paymentIntentId\":\"string\"}")
  .asString();
```

`POST /api/Product/confirmPaymentIntent`

> Body parameter

```json
{
  "paymentIntentId": "string"
}
```

<h3 id="post__api_product_confirmpaymentintent-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[PortalConfirmPaymentIntentRequest](#schemaportalconfirmpaymentintentrequest)|false|none|

<h3 id="post__api_product_confirmpaymentintent-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Product_checkout

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Product/checkout");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"zipCode\":\"string\",\"state\":\"string\",\"stateCode\":\"string\",\"country\":\"string\",\"city\":\"string\",\"firstName\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"planPriceId\":\"string\",\"workspaceId\":\"string\",\"paymentIntentId\":\"string\",\"companyName\":\"string\",\"cardHolderFirstName\":\"string\",\"cardHolderLastName\":\"string\",\"vatId\":\"string\",\"invoiceEmail\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"zipCode\":\"string\",\"state\":\"string\",\"stateCode\":\"string\",\"country\":\"string\",\"city\":\"string\",\"firstName\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"planPriceId\":\"string\",\"workspaceId\":\"string\",\"paymentIntentId\":\"string\",\"companyName\":\"string\",\"cardHolderFirstName\":\"string\",\"cardHolderLastName\":\"string\",\"vatId\":\"string\",\"invoiceEmail\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Product/checkout", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"zipCode\":\"string\",\"state\":\"string\",\"stateCode\":\"string\",\"country\":\"string\",\"city\":\"string\",\"firstName\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"planPriceId\":\"string\",\"workspaceId\":\"string\",\"paymentIntentId\":\"string\",\"companyName\":\"string\",\"cardHolderFirstName\":\"string\",\"cardHolderLastName\":\"string\",\"vatId\":\"string\",\"invoiceEmail\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Product/checkout");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Product/checkout HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 399

{"addressLine1":"string","addressLine2":"string","zipCode":"string","state":"string","stateCode":"string","country":"string","city":"string","firstName":"string","lastName":"string","company":"string","planPriceId":"string","workspaceId":"string","paymentIntentId":"string","companyName":"string","cardHolderFirstName":"string","cardHolderLastName":"string","vatId":"string","invoiceEmail":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Product/checkout")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"zipCode\":\"string\",\"state\":\"string\",\"stateCode\":\"string\",\"country\":\"string\",\"city\":\"string\",\"firstName\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"planPriceId\":\"string\",\"workspaceId\":\"string\",\"paymentIntentId\":\"string\",\"companyName\":\"string\",\"cardHolderFirstName\":\"string\",\"cardHolderLastName\":\"string\",\"vatId\":\"string\",\"invoiceEmail\":\"string\"}")
  .asString();
```

`POST /api/Product/checkout`

> Body parameter

```json
{
  "addressLine1": "string",
  "addressLine2": "string",
  "zipCode": "string",
  "state": "string",
  "stateCode": "string",
  "country": "string",
  "city": "string",
  "firstName": "string",
  "lastName": "string",
  "company": "string",
  "planPriceId": "string",
  "workspaceId": "string",
  "paymentIntentId": "string",
  "companyName": "string",
  "cardHolderFirstName": "string",
  "cardHolderLastName": "string",
  "vatId": "string",
  "invoiceEmail": "string"
}
```

<h3 id="post__api_product_checkout-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[PortalCheckoutRequest](#schemaportalcheckoutrequest)|false|none|

<h3 id="post__api_product_checkout-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Product_subscription_{workspaceId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Product/subscription/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Product/subscription/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Product/subscription/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Product/subscription/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Product/subscription/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Product/subscription/{workspaceId}`

<h3 id="get__api_product_subscription_{workspaceid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|workspaceId|path|string|true|none|

<h3 id="get__api_product_subscription_{workspaceid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Product_updatePayment

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Product/updatePayment");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"workspaceId\":\"string\",\"temporaryToken\":\"string\",\"firstName\":\"string\",\"lastName\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"workspaceId\":\"string\",\"temporaryToken\":\"string\",\"firstName\":\"string\",\"lastName\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Product/updatePayment", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"workspaceId\":\"string\",\"temporaryToken\":\"string\",\"firstName\":\"string\",\"lastName\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Product/updatePayment");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Product/updatePayment HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 91

{"workspaceId":"string","temporaryToken":"string","firstName":"string","lastName":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Product/updatePayment")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"workspaceId\":\"string\",\"temporaryToken\":\"string\",\"firstName\":\"string\",\"lastName\":\"string\"}")
  .asString();
```

`POST /api/Product/updatePayment`

> Body parameter

```json
{
  "workspaceId": "string",
  "temporaryToken": "string",
  "firstName": "string",
  "lastName": "string"
}
```

<h3 id="post__api_product_updatepayment-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[UpdatePaymentMethodDto](#schemaupdatepaymentmethoddto)|false|none|

<h3 id="post__api_product_updatepayment-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Product_cancelSubscription

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Product/cancelSubscription");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"workspaceId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"workspaceId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Product/cancelSubscription", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"workspaceId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Product/cancelSubscription");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Product/cancelSubscription HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 24

{"workspaceId":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Product/cancelSubscription")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"workspaceId\":\"string\"}")
  .asString();
```

`POST /api/Product/cancelSubscription`

> Body parameter

```json
{
  "workspaceId": "string"
}
```

<h3 id="post__api_product_cancelsubscription-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[CancelSubscriptionDto](#schemacancelsubscriptiondto)|false|none|

<h3 id="post__api_product_cancelsubscription-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Product_priceEstimate

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Product/priceEstimate");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"zipCode\":\"string\",\"state\":\"string\",\"stateCode\":\"string\",\"country\":\"string\",\"city\":\"string\",\"firstName\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"paymentMethodId\":\"string\",\"planName\":\"string\",\"planPriceId\":\"string\",\"totalPrice\":0,\"companyName\":\"string\",\"invoiceEmail\":\"string\",\"vatId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"zipCode\":\"string\",\"state\":\"string\",\"stateCode\":\"string\",\"country\":\"string\",\"city\":\"string\",\"firstName\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"paymentMethodId\":\"string\",\"planName\":\"string\",\"planPriceId\":\"string\",\"totalPrice\":0,\"companyName\":\"string\",\"invoiceEmail\":\"string\",\"vatId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Product/priceEstimate", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"zipCode\":\"string\",\"state\":\"string\",\"stateCode\":\"string\",\"country\":\"string\",\"city\":\"string\",\"firstName\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"paymentMethodId\":\"string\",\"planName\":\"string\",\"planPriceId\":\"string\",\"totalPrice\":0,\"companyName\":\"string\",\"invoiceEmail\":\"string\",\"vatId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Product/priceEstimate");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Product/priceEstimate HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 350

{"addressLine1":"string","addressLine2":"string","zipCode":"string","state":"string","stateCode":"string","country":"string","city":"string","firstName":"string","lastName":"string","company":"string","paymentMethodId":"string","planName":"string","planPriceId":"string","totalPrice":0,"companyName":"string","invoiceEmail":"string","vatId":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Product/priceEstimate")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"zipCode\":\"string\",\"state\":\"string\",\"stateCode\":\"string\",\"country\":\"string\",\"city\":\"string\",\"firstName\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"paymentMethodId\":\"string\",\"planName\":\"string\",\"planPriceId\":\"string\",\"totalPrice\":0,\"companyName\":\"string\",\"invoiceEmail\":\"string\",\"vatId\":\"string\"}")
  .asString();
```

`POST /api/Product/priceEstimate`

> Body parameter

```json
{
  "addressLine1": "string",
  "addressLine2": "string",
  "zipCode": "string",
  "state": "string",
  "stateCode": "string",
  "country": "string",
  "city": "string",
  "firstName": "string",
  "lastName": "string",
  "company": "string",
  "paymentMethodId": "string",
  "planName": "string",
  "planPriceId": "string",
  "totalPrice": 0,
  "companyName": "string",
  "invoiceEmail": "string",
  "vatId": "string"
}
```

<h3 id="post__api_product_priceestimate-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[PortalCreatePaymentIntentRequest](#schemaportalcreatepaymentintentrequest)|false|none|

<h3 id="post__api_product_priceestimate-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-promotedmessage">PromotedMessage</h1>

## get__api_event_{eventIdOrSlug}_promoted-messages

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/promoted-messages");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/event/string/promoted-messages", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/event/string/promoted-messages");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/event/string/promoted-messages HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/event/string/promoted-messages")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/event/{eventIdOrSlug}/promoted-messages`

<h3 id="get__api_event_{eventidorslug}_promoted-messages-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|

<h3 id="get__api_event_{eventidorslug}_promoted-messages-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_event_{eventId}_promoted-messages_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/promoted-messages/string");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("DELETE", "/api/event/string/promoted-messages/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/event/string/promoted-messages/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/event/string/promoted-messages/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/event/string/promoted-messages/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`DELETE /api/event/{eventId}/promoted-messages/{entryId}`

<h3 id="delete__api_event_{eventid}_promoted-messages_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|

<h3 id="delete__api_event_{eventid}_promoted-messages_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_event_{eventId}_promoted-messages_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/promoted-messages/string");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"fromDate\":\"2019-08-24T14:15:22Z\",\"toDate\":\"2019-08-24T14:15:22Z\",\"message\":\"string\",\"isHidden\":true,\"isVisibleOnTop\":true,\"groupIds\":[\"string\"],\"platformPages\":[0]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"fromDate\":\"2019-08-24T14:15:22Z\",\"toDate\":\"2019-08-24T14:15:22Z\",\"message\":\"string\",\"isHidden\":true,\"isVisibleOnTop\":true,\"groupIds\":[\"string\"],\"platformPages\":[0]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/event/string/promoted-messages/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"fromDate\":\"2019-08-24T14:15:22Z\",\"toDate\":\"2019-08-24T14:15:22Z\",\"message\":\"string\",\"isHidden\":true,\"isVisibleOnTop\":true,\"groupIds\":[\"string\"],\"platformPages\":[0]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/event/string/promoted-messages/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/event/string/promoted-messages/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 180

{"id":"string","fromDate":"2019-08-24T14:15:22Z","toDate":"2019-08-24T14:15:22Z","message":"string","isHidden":true,"isVisibleOnTop":true,"groupIds":["string"],"platformPages":[0]}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/event/string/promoted-messages/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"fromDate\":\"2019-08-24T14:15:22Z\",\"toDate\":\"2019-08-24T14:15:22Z\",\"message\":\"string\",\"isHidden\":true,\"isVisibleOnTop\":true,\"groupIds\":[\"string\"],\"platformPages\":[0]}")
  .asString();
```

`PUT /api/event/{eventId}/promoted-messages/{entryId}`

> Body parameter

```json
{
  "id": "string",
  "fromDate": "2019-08-24T14:15:22Z",
  "toDate": "2019-08-24T14:15:22Z",
  "message": "string",
  "isHidden": true,
  "isVisibleOnTop": true,
  "groupIds": [
    "string"
  ],
  "platformPages": [
    0
  ]
}
```

<h3 id="put__api_event_{eventid}_promoted-messages_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|
|body|body|[PromotedMessageDto](#schemapromotedmessagedto)|false|none|

<h3 id="put__api_event_{eventid}_promoted-messages_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## patch__api_event_{eventId}_promoted-messages_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/promoted-messages/string");
var request = new RestRequest(Method.PATCH);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"fromDate\":\"2019-08-24T14:15:22Z\",\"toDate\":\"2019-08-24T14:15:22Z\",\"message\":\"string\",\"isHidden\":true,\"isVisibleOnTop\":true,\"groupIds\":[\"string\"],\"platformPages\":[0]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"fromDate\":\"2019-08-24T14:15:22Z\",\"toDate\":\"2019-08-24T14:15:22Z\",\"message\":\"string\",\"isHidden\":true,\"isVisibleOnTop\":true,\"groupIds\":[\"string\"],\"platformPages\":[0]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PATCH", "/api/event/string/promoted-messages/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"fromDate\":\"2019-08-24T14:15:22Z\",\"toDate\":\"2019-08-24T14:15:22Z\",\"message\":\"string\",\"isHidden\":true,\"isVisibleOnTop\":true,\"groupIds\":[\"string\"],\"platformPages\":[0]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PATCH", "https://example.com/api/event/string/promoted-messages/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PATCH /api/event/string/promoted-messages/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 166

{"fromDate":"2019-08-24T14:15:22Z","toDate":"2019-08-24T14:15:22Z","message":"string","isHidden":true,"isVisibleOnTop":true,"groupIds":["string"],"platformPages":[0]}
```

```java
HttpResponse<String> response = Unirest.patch("https://example.com/api/event/string/promoted-messages/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"fromDate\":\"2019-08-24T14:15:22Z\",\"toDate\":\"2019-08-24T14:15:22Z\",\"message\":\"string\",\"isHidden\":true,\"isVisibleOnTop\":true,\"groupIds\":[\"string\"],\"platformPages\":[0]}")
  .asString();
```

`PATCH /api/event/{eventId}/promoted-messages/{entryId}`

> Body parameter

```json
{
  "fromDate": "2019-08-24T14:15:22Z",
  "toDate": "2019-08-24T14:15:22Z",
  "message": "string",
  "isHidden": true,
  "isVisibleOnTop": true,
  "groupIds": [
    "string"
  ],
  "platformPages": [
    0
  ]
}
```

<h3 id="patch__api_event_{eventid}_promoted-messages_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|
|body|body|[PartialPromotedMessageDto](#schemapartialpromotedmessagedto)|false|none|

<h3 id="patch__api_event_{eventid}_promoted-messages_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_event_{eventId}_promoted-messages_create

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/promoted-messages/create");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"fromDate\":\"2019-08-24T14:15:22Z\",\"toDate\":\"2019-08-24T14:15:22Z\",\"message\":\"string\",\"isHidden\":true,\"isVisibleOnTop\":true,\"groupIds\":[\"string\"],\"platformPages\":[0]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"fromDate\":\"2019-08-24T14:15:22Z\",\"toDate\":\"2019-08-24T14:15:22Z\",\"message\":\"string\",\"isHidden\":true,\"isVisibleOnTop\":true,\"groupIds\":[\"string\"],\"platformPages\":[0]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/event/string/promoted-messages/create", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"fromDate\":\"2019-08-24T14:15:22Z\",\"toDate\":\"2019-08-24T14:15:22Z\",\"message\":\"string\",\"isHidden\":true,\"isVisibleOnTop\":true,\"groupIds\":[\"string\"],\"platformPages\":[0]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/event/string/promoted-messages/create");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/event/string/promoted-messages/create HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 180

{"id":"string","fromDate":"2019-08-24T14:15:22Z","toDate":"2019-08-24T14:15:22Z","message":"string","isHidden":true,"isVisibleOnTop":true,"groupIds":["string"],"platformPages":[0]}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/event/string/promoted-messages/create")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"fromDate\":\"2019-08-24T14:15:22Z\",\"toDate\":\"2019-08-24T14:15:22Z\",\"message\":\"string\",\"isHidden\":true,\"isVisibleOnTop\":true,\"groupIds\":[\"string\"],\"platformPages\":[0]}")
  .asString();
```

`POST /api/event/{eventId}/promoted-messages/create`

> Body parameter

```json
{
  "id": "string",
  "fromDate": "2019-08-24T14:15:22Z",
  "toDate": "2019-08-24T14:15:22Z",
  "message": "string",
  "isHidden": true,
  "isVisibleOnTop": true,
  "groupIds": [
    "string"
  ],
  "platformPages": [
    0
  ]
}
```

<h3 id="post__api_event_{eventid}_promoted-messages_create-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[PromotedMessageDto](#schemapromotedmessagedto)|false|none|

<h3 id="post__api_event_{eventid}_promoted-messages_create-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-registration">Registration</h1>

## post__api_Registration

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Registration");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"eventId\":\"string\",\"formFields\":{\"property1\":\"string\",\"property2\":\"string\"},\"paymentIntentId\":\"string\",\"paymentIntentClientSecret\":\"string\",\"registrationAccessKey\":\"string\",\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"language\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"eventId\":\"string\",\"formFields\":{\"property1\":\"string\",\"property2\":\"string\"},\"paymentIntentId\":\"string\",\"paymentIntentClientSecret\":\"string\",\"registrationAccessKey\":\"string\",\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"language\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Registration", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"eventId\":\"string\",\"formFields\":{\"property1\":\"string\",\"property2\":\"string\"},\"paymentIntentId\":\"string\",\"paymentIntentClientSecret\":\"string\",\"registrationAccessKey\":\"string\",\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"language\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Registration");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Registration HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 299

{"eventId":"string","formFields":{"property1":"string","property2":"string"},"paymentIntentId":"string","paymentIntentClientSecret":"string","registrationAccessKey":"string","reservations":[{"id":"string","entityId":"string","token":"string","contextId":"string","isUsed":true}],"language":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Registration")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"eventId\":\"string\",\"formFields\":{\"property1\":\"string\",\"property2\":\"string\"},\"paymentIntentId\":\"string\",\"paymentIntentClientSecret\":\"string\",\"registrationAccessKey\":\"string\",\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"language\":\"string\"}")
  .asString();
```

`POST /api/Registration`

> Body parameter

```json
{
  "eventId": "string",
  "formFields": {
    "property1": "string",
    "property2": "string"
  },
  "paymentIntentId": "string",
  "paymentIntentClientSecret": "string",
  "registrationAccessKey": "string",
  "reservations": [
    {
      "id": "string",
      "entityId": "string",
      "token": "string",
      "contextId": "string",
      "isUsed": true
    }
  ],
  "language": "string"
}
```

<h3 id="post__api_registration-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[RegisterEventDto](#schemaregistereventdto)|false|none|

<h3 id="post__api_registration-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Registration_createPaymentIntent

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Registration/createPaymentIntent");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"eventId\":\"string\",\"formFields\":{\"property1\":\"string\",\"property2\":\"string\"},\"price\":0,\"registrationAccessKey\":\"string\",\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"language\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"eventId\":\"string\",\"formFields\":{\"property1\":\"string\",\"property2\":\"string\"},\"price\":0,\"registrationAccessKey\":\"string\",\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"language\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Registration/createPaymentIntent", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"eventId\":\"string\",\"formFields\":{\"property1\":\"string\",\"property2\":\"string\"},\"price\":0,\"registrationAccessKey\":\"string\",\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"language\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Registration/createPaymentIntent");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Registration/createPaymentIntent HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 245

{"eventId":"string","formFields":{"property1":"string","property2":"string"},"price":0,"registrationAccessKey":"string","reservations":[{"id":"string","entityId":"string","token":"string","contextId":"string","isUsed":true}],"language":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Registration/createPaymentIntent")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"eventId\":\"string\",\"formFields\":{\"property1\":\"string\",\"property2\":\"string\"},\"price\":0,\"registrationAccessKey\":\"string\",\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"language\":\"string\"}")
  .asString();
```

`POST /api/Registration/createPaymentIntent`

> Body parameter

```json
{
  "eventId": "string",
  "formFields": {
    "property1": "string",
    "property2": "string"
  },
  "price": 0,
  "registrationAccessKey": "string",
  "reservations": [
    {
      "id": "string",
      "entityId": "string",
      "token": "string",
      "contextId": "string",
      "isUsed": true
    }
  ],
  "language": "string"
}
```

<h3 id="post__api_registration_createpaymentintent-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[CreatePaymentIntentDto](#schemacreatepaymentintentdto)|false|none|

<h3 id="post__api_registration_createpaymentintent-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_Registration_create

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Registration/create");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"registrationId\":\"string\",\"eventId\":\"string\",\"values\":{\"property1\":\"string\",\"property2\":\"string\"},\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"ticket\":{\"url\":\"string\",\"barcode\":\"string\"}}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"registrationId\":\"string\",\"eventId\":\"string\",\"values\":{\"property1\":\"string\",\"property2\":\"string\"},\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"ticket\":{\"url\":\"string\",\"barcode\":\"string\"}}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/Registration/create", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"registrationId\":\"string\",\"eventId\":\"string\",\"values\":{\"property1\":\"string\",\"property2\":\"string\"},\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"ticket\":{\"url\":\"string\",\"barcode\":\"string\"}}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/Registration/create");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/Registration/create HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 249

{"registrationId":"string","eventId":"string","values":{"property1":"string","property2":"string"},"reservations":[{"id":"string","entityId":"string","token":"string","contextId":"string","isUsed":true}],"ticket":{"url":"string","barcode":"string"}}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/Registration/create")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"registrationId\":\"string\",\"eventId\":\"string\",\"values\":{\"property1\":\"string\",\"property2\":\"string\"},\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"ticket\":{\"url\":\"string\",\"barcode\":\"string\"}}")
  .asString();
```

`PUT /api/Registration/create`

> Body parameter

```json
{
  "registrationId": "string",
  "eventId": "string",
  "values": {
    "property1": "string",
    "property2": "string"
  },
  "reservations": [
    {
      "id": "string",
      "entityId": "string",
      "token": "string",
      "contextId": "string",
      "isUsed": true
    }
  ],
  "ticket": {
    "url": "string",
    "barcode": "string"
  }
}
```

<h3 id="put__api_registration_create-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[CreateRegistrationDto](#schemacreateregistrationdto)|false|none|

<h3 id="put__api_registration_create-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Registration_update

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Registration/update");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"eventId\":\"string\",\"registrationId\":\"string\",\"values\":{\"property1\":\"string\",\"property2\":\"string\"},\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"ticket\":{\"url\":\"string\",\"barcode\":\"string\"}}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"eventId\":\"string\",\"registrationId\":\"string\",\"values\":{\"property1\":\"string\",\"property2\":\"string\"},\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"ticket\":{\"url\":\"string\",\"barcode\":\"string\"}}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Registration/update", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"eventId\":\"string\",\"registrationId\":\"string\",\"values\":{\"property1\":\"string\",\"property2\":\"string\"},\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"ticket\":{\"url\":\"string\",\"barcode\":\"string\"}}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Registration/update");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Registration/update HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 249

{"eventId":"string","registrationId":"string","values":{"property1":"string","property2":"string"},"reservations":[{"id":"string","entityId":"string","token":"string","contextId":"string","isUsed":true}],"ticket":{"url":"string","barcode":"string"}}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Registration/update")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"eventId\":\"string\",\"registrationId\":\"string\",\"values\":{\"property1\":\"string\",\"property2\":\"string\"},\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"ticket\":{\"url\":\"string\",\"barcode\":\"string\"}}")
  .asString();
```

`POST /api/Registration/update`

> Body parameter

```json
{
  "eventId": "string",
  "registrationId": "string",
  "values": {
    "property1": "string",
    "property2": "string"
  },
  "reservations": [
    {
      "id": "string",
      "entityId": "string",
      "token": "string",
      "contextId": "string",
      "isUsed": true
    }
  ],
  "ticket": {
    "url": "string",
    "barcode": "string"
  }
}
```

<h3 id="post__api_registration_update-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[UpdateRegistrationDto](#schemaupdateregistrationdto)|false|none|

<h3 id="post__api_registration_update-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Registration_sendEmail

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Registration/sendEmail");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"eventId\":\"string\",\"senderIdentityId\":\"string\",\"subject\":\"string\",\"template\":\"string\",\"destinations\":[{\"registrationId\":\"string\",\"email\":\"string\",\"replacementData\":{\"property1\":null,\"property2\":null}}]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"eventId\":\"string\",\"senderIdentityId\":\"string\",\"subject\":\"string\",\"template\":\"string\",\"destinations\":[{\"registrationId\":\"string\",\"email\":\"string\",\"replacementData\":{\"property1\":null,\"property2\":null}}]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Registration/sendEmail", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"eventId\":\"string\",\"senderIdentityId\":\"string\",\"subject\":\"string\",\"template\":\"string\",\"destinations\":[{\"registrationId\":\"string\",\"email\":\"string\",\"replacementData\":{\"property1\":null,\"property2\":null}}]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Registration/sendEmail");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Registration/sendEmail HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 203

{"eventId":"string","senderIdentityId":"string","subject":"string","template":"string","destinations":[{"registrationId":"string","email":"string","replacementData":{"property1":null,"property2":null}}]}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Registration/sendEmail")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"eventId\":\"string\",\"senderIdentityId\":\"string\",\"subject\":\"string\",\"template\":\"string\",\"destinations\":[{\"registrationId\":\"string\",\"email\":\"string\",\"replacementData\":{\"property1\":null,\"property2\":null}}]}")
  .asString();
```

`POST /api/Registration/sendEmail`

> Body parameter

```json
{
  "eventId": "string",
  "senderIdentityId": "string",
  "subject": "string",
  "template": "string",
  "destinations": [
    {
      "registrationId": "string",
      "email": "string",
      "replacementData": {
        "property1": null,
        "property2": null
      }
    }
  ]
}
```

<h3 id="post__api_registration_sendemail-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[SendEmailDto](#schemasendemaildto)|false|none|

<h3 id="post__api_registration_sendemail-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Registration_sendSms

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Registration/sendSms");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"eventId\":\"string\",\"sender\":\"string\",\"template\":\"string\",\"destinations\":[{\"registrationId\":\"string\",\"phoneNumber\":\"string\",\"text\":\"string\",\"messageId\":\"string\",\"error\":{\"errorName\":\"string\",\"errorDescription\":\"string\"}}],\"sendDateTime\":\"2019-08-24T14:15:22Z\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"eventId\":\"string\",\"sender\":\"string\",\"template\":\"string\",\"destinations\":[{\"registrationId\":\"string\",\"phoneNumber\":\"string\",\"text\":\"string\",\"messageId\":\"string\",\"error\":{\"errorName\":\"string\",\"errorDescription\":\"string\"}}],\"sendDateTime\":\"2019-08-24T14:15:22Z\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Registration/sendSms", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"eventId\":\"string\",\"sender\":\"string\",\"template\":\"string\",\"destinations\":[{\"registrationId\":\"string\",\"phoneNumber\":\"string\",\"text\":\"string\",\"messageId\":\"string\",\"error\":{\"errorName\":\"string\",\"errorDescription\":\"string\"}}],\"sendDateTime\":\"2019-08-24T14:15:22Z\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Registration/sendSms");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Registration/sendSms HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 260

{"eventId":"string","sender":"string","template":"string","destinations":[{"registrationId":"string","phoneNumber":"string","text":"string","messageId":"string","error":{"errorName":"string","errorDescription":"string"}}],"sendDateTime":"2019-08-24T14:15:22Z"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Registration/sendSms")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"eventId\":\"string\",\"sender\":\"string\",\"template\":\"string\",\"destinations\":[{\"registrationId\":\"string\",\"phoneNumber\":\"string\",\"text\":\"string\",\"messageId\":\"string\",\"error\":{\"errorName\":\"string\",\"errorDescription\":\"string\"}}],\"sendDateTime\":\"2019-08-24T14:15:22Z\"}")
  .asString();
```

`POST /api/Registration/sendSms`

> Body parameter

```json
{
  "eventId": "string",
  "sender": "string",
  "template": "string",
  "destinations": [
    {
      "registrationId": "string",
      "phoneNumber": "string",
      "text": "string",
      "messageId": "string",
      "error": {
        "errorName": "string",
        "errorDescription": "string"
      }
    }
  ],
  "sendDateTime": "2019-08-24T14:15:22Z"
}
```

<h3 id="post__api_registration_sendsms-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[SendSmsDto](#schemasendsmsdto)|false|none|

<h3 id="post__api_registration_sendsms-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Registration_decline

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Registration/decline");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"eventId\":\"string\",\"registrationAccessKey\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"eventId\":\"string\",\"registrationAccessKey\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Registration/decline", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"eventId\":\"string\",\"registrationAccessKey\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Registration/decline");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Registration/decline HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 53

{"eventId":"string","registrationAccessKey":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Registration/decline")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"eventId\":\"string\",\"registrationAccessKey\":\"string\"}")
  .asString();
```

`POST /api/Registration/decline`

> Body parameter

```json
{
  "eventId": "string",
  "registrationAccessKey": "string"
}
```

<h3 id="post__api_registration_decline-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[DeclineRegistrationDto](#schemadeclineregistrationdto)|false|none|

<h3 id="post__api_registration_decline-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Registration_saveGuest

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Registration/saveGuest");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"parentRegistrationId\":\"string\",\"registrationId\":\"string\",\"values\":{\"property1\":\"string\",\"property2\":\"string\"},\"eventId\":\"string\",\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"contextId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"parentRegistrationId\":\"string\",\"registrationId\":\"string\",\"values\":{\"property1\":\"string\",\"property2\":\"string\"},\"eventId\":\"string\",\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"contextId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Registration/saveGuest", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"parentRegistrationId\":\"string\",\"registrationId\":\"string\",\"values\":{\"property1\":\"string\",\"property2\":\"string\"},\"eventId\":\"string\",\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"contextId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Registration/saveGuest");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Registration/saveGuest HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 257

{"parentRegistrationId":"string","registrationId":"string","values":{"property1":"string","property2":"string"},"eventId":"string","reservations":[{"id":"string","entityId":"string","token":"string","contextId":"string","isUsed":true}],"contextId":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Registration/saveGuest")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"parentRegistrationId\":\"string\",\"registrationId\":\"string\",\"values\":{\"property1\":\"string\",\"property2\":\"string\"},\"eventId\":\"string\",\"reservations\":[{\"id\":\"string\",\"entityId\":\"string\",\"token\":\"string\",\"contextId\":\"string\",\"isUsed\":true}],\"contextId\":\"string\"}")
  .asString();
```

`POST /api/Registration/saveGuest`

> Body parameter

```json
{
  "parentRegistrationId": "string",
  "registrationId": "string",
  "values": {
    "property1": "string",
    "property2": "string"
  },
  "eventId": "string",
  "reservations": [
    {
      "id": "string",
      "entityId": "string",
      "token": "string",
      "contextId": "string",
      "isUsed": true
    }
  ],
  "contextId": "string"
}
```

<h3 id="post__api_registration_saveguest-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[SaveGuestDto](#schemasaveguestdto)|false|none|

<h3 id="post__api_registration_saveguest-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Registration_bulkEdit

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Registration/bulkEdit");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"eventId\":\"string\",\"registrationIds\":[\"string\"],\"status\":0,\"clearReservations\":true,\"addToGroups\":[{\"value\":\"string\",\"isNew\":true}]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"eventId\":\"string\",\"registrationIds\":[\"string\"],\"status\":0,\"clearReservations\":true,\"addToGroups\":[{\"value\":\"string\",\"isNew\":true}]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Registration/bulkEdit", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"eventId\":\"string\",\"registrationIds\":[\"string\"],\"status\":0,\"clearReservations\":true,\"addToGroups\":[{\"value\":\"string\",\"isNew\":true}]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Registration/bulkEdit");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Registration/bulkEdit HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 133

{"eventId":"string","registrationIds":["string"],"status":0,"clearReservations":true,"addToGroups":[{"value":"string","isNew":true}]}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Registration/bulkEdit")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"eventId\":\"string\",\"registrationIds\":[\"string\"],\"status\":0,\"clearReservations\":true,\"addToGroups\":[{\"value\":\"string\",\"isNew\":true}]}")
  .asString();
```

`POST /api/Registration/bulkEdit`

> Body parameter

```json
{
  "eventId": "string",
  "registrationIds": [
    "string"
  ],
  "status": 0,
  "clearReservations": true,
  "addToGroups": [
    {
      "value": "string",
      "isNew": true
    }
  ]
}
```

<h3 id="post__api_registration_bulkedit-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[RegistrationBulkEditDto](#schemaregistrationbulkeditdto)|false|none|

<h3 id="post__api_registration_bulkedit-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-registrationgroup">RegistrationGroup</h1>

## get__api_event_{eventIdOrSlug}_groups

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/groups");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/event/string/groups", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/event/string/groups");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/event/string/groups HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/event/string/groups")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/event/{eventIdOrSlug}/groups`

<h3 id="get__api_event_{eventidorslug}_groups-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|

<h3 id="get__api_event_{eventidorslug}_groups-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_event_{eventId}_groups_{entityId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/groups/string");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("DELETE", "/api/event/string/groups/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/event/string/groups/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/event/string/groups/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/event/string/groups/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`DELETE /api/event/{eventId}/groups/{entityId}`

<h3 id="delete__api_event_{eventid}_groups_{entityid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entityId|path|string|true|none|

<h3 id="delete__api_event_{eventid}_groups_{entityid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## patch__api_event_{eventId}_groups_{entityId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/groups/string");
var request = new RestRequest(Method.PATCH);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"name\":\"string\",\"userIds\":[\"string\"]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"name\":\"string\",\"userIds\":[\"string\"]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PATCH", "/api/event/string/groups/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"name\":\"string\",\"userIds\":[\"string\"]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PATCH", "https://example.com/api/event/string/groups/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PATCH /api/event/string/groups/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 38

{"name":"string","userIds":["string"]}
```

```java
HttpResponse<String> response = Unirest.patch("https://example.com/api/event/string/groups/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"name\":\"string\",\"userIds\":[\"string\"]}")
  .asString();
```

`PATCH /api/event/{eventId}/groups/{entityId}`

> Body parameter

```json
{
  "name": "string",
  "userIds": [
    "string"
  ]
}
```

<h3 id="patch__api_event_{eventid}_groups_{entityid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entityId|path|string|true|none|
|body|body|[PartialRegistrationGroupDto](#schemapartialregistrationgroupdto)|false|none|

<h3 id="patch__api_event_{eventid}_groups_{entityid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_event_{eventId}_groups

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/groups");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"eventId\":\"string\",\"type\":0,\"subType\":0,\"name\":\"string\",\"userIds\":[\"string\"],\"elementId\":\"string\",\"elementLabel\":\"string\",\"elementChoiceId\":\"string\",\"elementChoiceLabel\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"eventId\":\"string\",\"type\":0,\"subType\":0,\"name\":\"string\",\"userIds\":[\"string\"],\"elementId\":\"string\",\"elementLabel\":\"string\",\"elementChoiceId\":\"string\",\"elementChoiceLabel\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/event/string/groups", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"eventId\":\"string\",\"type\":0,\"subType\":0,\"name\":\"string\",\"userIds\":[\"string\"],\"elementId\":\"string\",\"elementLabel\":\"string\",\"elementChoiceId\":\"string\",\"elementChoiceLabel\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/event/string/groups");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/event/string/groups HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 194

{"id":"string","eventId":"string","type":0,"subType":0,"name":"string","userIds":["string"],"elementId":"string","elementLabel":"string","elementChoiceId":"string","elementChoiceLabel":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/event/string/groups")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"eventId\":\"string\",\"type\":0,\"subType\":0,\"name\":\"string\",\"userIds\":[\"string\"],\"elementId\":\"string\",\"elementLabel\":\"string\",\"elementChoiceId\":\"string\",\"elementChoiceLabel\":\"string\"}")
  .asString();
```

`POST /api/event/{eventId}/groups`

> Body parameter

```json
{
  "id": "string",
  "eventId": "string",
  "type": 0,
  "subType": 0,
  "name": "string",
  "userIds": [
    "string"
  ],
  "elementId": "string",
  "elementLabel": "string",
  "elementChoiceId": "string",
  "elementChoiceLabel": "string"
}
```

<h3 id="post__api_event_{eventid}_groups-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[RegistrationGroupDto](#schemaregistrationgroupdto)|false|none|

<h3 id="post__api_event_{eventid}_groups-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_event_{eventId}_groups_batch-update

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/groups/batch-update");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"items\":[{\"groupId\":\"string\",\"userId\":\"string\"}]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"items\":[{\"groupId\":\"string\",\"userId\":\"string\"}]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/event/string/groups/batch-update", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"items\":[{\"groupId\":\"string\",\"userId\":\"string\"}]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/event/string/groups/batch-update");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/event/string/groups/batch-update HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 50

{"items":[{"groupId":"string","userId":"string"}]}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/event/string/groups/batch-update")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"items\":[{\"groupId\":\"string\",\"userId\":\"string\"}]}")
  .asString();
```

`PUT /api/event/{eventId}/groups/batch-update`

> Body parameter

```json
{
  "items": [
    {
      "groupId": "string",
      "userId": "string"
    }
  ]
}
```

<h3 id="put__api_event_{eventid}_groups_batch-update-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[BatchRegistrationGroupDto](#schemabatchregistrationgroupdto)|false|none|

<h3 id="put__api_event_{eventid}_groups_batch-update-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_event_{eventId}_groups_batch-delete

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/groups/batch-delete");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"items\":[{\"groupId\":\"string\",\"userId\":\"string\"}]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"items\":[{\"groupId\":\"string\",\"userId\":\"string\"}]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("DELETE", "/api/event/string/groups/batch-delete", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"items\":[{\"groupId\":\"string\",\"userId\":\"string\"}]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/event/string/groups/batch-delete");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/event/string/groups/batch-delete HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 50

{"items":[{"groupId":"string","userId":"string"}]}
```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/event/string/groups/batch-delete")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"items\":[{\"groupId\":\"string\",\"userId\":\"string\"}]}")
  .asString();
```

`DELETE /api/event/{eventId}/groups/batch-delete`

> Body parameter

```json
{
  "items": [
    {
      "groupId": "string",
      "userId": "string"
    }
  ]
}
```

<h3 id="delete__api_event_{eventid}_groups_batch-delete-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[BatchRegistrationGroupDto](#schemabatchregistrationgroupdto)|false|none|

<h3 id="delete__api_event_{eventid}_groups_batch-delete-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-reservation">Reservation</h1>

## get__api_Reservation_getUsedTicketQuantity_{topParentReferenceId}_{entityId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Reservation/getUsedTicketQuantity/string/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Reservation/getUsedTicketQuantity/string/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Reservation/getUsedTicketQuantity/string/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Reservation/getUsedTicketQuantity/string/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Reservation/getUsedTicketQuantity/string/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Reservation/getUsedTicketQuantity/{topParentReferenceId}/{entityId}`

<h3 id="get__api_reservation_getusedticketquantity_{topparentreferenceid}_{entityid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|topParentReferenceId|path|string|true|none|
|entityId|path|string|true|none|

<h3 id="get__api_reservation_getusedticketquantity_{topparentreferenceid}_{entityid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Reservation_getAvailableQuantities_{topParentReferenceId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Reservation/getAvailableQuantities/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Reservation/getAvailableQuantities/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Reservation/getAvailableQuantities/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Reservation/getAvailableQuantities/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Reservation/getAvailableQuantities/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Reservation/getAvailableQuantities/{topParentReferenceId}`

<h3 id="get__api_reservation_getavailablequantities_{topparentreferenceid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|topParentReferenceId|path|string|true|none|

<h3 id="get__api_reservation_getavailablequantities_{topparentreferenceid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Reservation_getReservations_{topParentReferenceId}_{registrationIdOrAccessKey}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Reservation/getReservations/string/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Reservation/getReservations/string/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Reservation/getReservations/string/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Reservation/getReservations/string/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Reservation/getReservations/string/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Reservation/getReservations/{topParentReferenceId}/{registrationIdOrAccessKey}`

<h3 id="get__api_reservation_getreservations_{topparentreferenceid}_{registrationidoraccesskey}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|topParentReferenceId|path|string|true|none|
|registrationIdOrAccessKey|path|string|true|none|

<h3 id="get__api_reservation_getreservations_{topparentreferenceid}_{registrationidoraccesskey}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Reservation_reserve

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Reservation/reserve");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"topParentReferenceId\":\"string\",\"contextId\":\"string\",\"entityId\":\"string\",\"previousEntityId\":\"string\",\"language\":\"string\",\"isRegistrationPage\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"topParentReferenceId\":\"string\",\"contextId\":\"string\",\"entityId\":\"string\",\"previousEntityId\":\"string\",\"language\":\"string\",\"isRegistrationPage\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Reservation/reserve", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"topParentReferenceId\":\"string\",\"contextId\":\"string\",\"entityId\":\"string\",\"previousEntityId\":\"string\",\"language\":\"string\",\"isRegistrationPage\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Reservation/reserve");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Reservation/reserve HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 148

{"topParentReferenceId":"string","contextId":"string","entityId":"string","previousEntityId":"string","language":"string","isRegistrationPage":true}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Reservation/reserve")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"topParentReferenceId\":\"string\",\"contextId\":\"string\",\"entityId\":\"string\",\"previousEntityId\":\"string\",\"language\":\"string\",\"isRegistrationPage\":true}")
  .asString();
```

`POST /api/Reservation/reserve`

> Body parameter

```json
{
  "topParentReferenceId": "string",
  "contextId": "string",
  "entityId": "string",
  "previousEntityId": "string",
  "language": "string",
  "isRegistrationPage": true
}
```

<h3 id="post__api_reservation_reserve-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[ReservationRequest](#schemareservationrequest)|false|none|

<h3 id="post__api_reservation_reserve-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Reservation_release

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Reservation/release");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"eventId\":\"string\",\"ids\":[\"string\"]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"eventId\":\"string\",\"ids\":[\"string\"]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Reservation/release", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"eventId\":\"string\",\"ids\":[\"string\"]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Reservation/release");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Reservation/release HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 37

{"eventId":"string","ids":["string"]}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Reservation/release")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"eventId\":\"string\",\"ids\":[\"string\"]}")
  .asString();
```

`POST /api/Reservation/release`

> Body parameter

```json
{
  "eventId": "string",
  "ids": [
    "string"
  ]
}
```

<h3 id="post__api_reservation_release-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[ReleaseReservationsDto](#schemareleasereservationsdto)|false|none|

<h3 id="post__api_reservation_release-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Reservation_getReservationsStatistics_{eventId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Reservation/getReservationsStatistics/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Reservation/getReservationsStatistics/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Reservation/getReservationsStatistics/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Reservation/getReservationsStatistics/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Reservation/getReservationsStatistics/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Reservation/getReservationsStatistics/{eventId}`

<h3 id="get__api_reservation_getreservationsstatistics_{eventid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|

<h3 id="get__api_reservation_getreservationsstatistics_{eventid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-sms">Sms</h1>

## post__api_sms_status

> Code samples

```csharp
var client = new RestClient("https://example.com/api/sms/status");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"results\":[{\"bulkId\":\"string\",\"messageId\":\"string\",\"to\":\"string\",\"from\":\"string\",\"text\":\"string\",\"sentAt\":\"2019-08-24T14:15:22Z\",\"doneAt\":\"2019-08-24T14:15:22Z\",\"smsCount\":0,\"mccMnc\":\"string\",\"price\":{\"pricePerMessage\":0,\"pricePerLookup\":0,\"currency\":\"string\"},\"status\":{\"groupId\":0,\"groupName\":\"string\",\"id\":0,\"name\":\"string\",\"description\":\"string\",\"action\":\"string\"},\"error\":{\"groupId\":0,\"groupName\":\"string\",\"id\":0,\"name\":\"string\",\"description\":\"string\",\"permanent\":true},\"callbackData\":\"string\"}]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"results\":[{\"bulkId\":\"string\",\"messageId\":\"string\",\"to\":\"string\",\"from\":\"string\",\"text\":\"string\",\"sentAt\":\"2019-08-24T14:15:22Z\",\"doneAt\":\"2019-08-24T14:15:22Z\",\"smsCount\":0,\"mccMnc\":\"string\",\"price\":{\"pricePerMessage\":0,\"pricePerLookup\":0,\"currency\":\"string\"},\"status\":{\"groupId\":0,\"groupName\":\"string\",\"id\":0,\"name\":\"string\",\"description\":\"string\",\"action\":\"string\"},\"error\":{\"groupId\":0,\"groupName\":\"string\",\"id\":0,\"name\":\"string\",\"description\":\"string\",\"permanent\":true},\"callbackData\":\"string\"}]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/sms/status", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"results\":[{\"bulkId\":\"string\",\"messageId\":\"string\",\"to\":\"string\",\"from\":\"string\",\"text\":\"string\",\"sentAt\":\"2019-08-24T14:15:22Z\",\"doneAt\":\"2019-08-24T14:15:22Z\",\"smsCount\":0,\"mccMnc\":\"string\",\"price\":{\"pricePerMessage\":0,\"pricePerLookup\":0,\"currency\":\"string\"},\"status\":{\"groupId\":0,\"groupName\":\"string\",\"id\":0,\"name\":\"string\",\"description\":\"string\",\"action\":\"string\"},\"error\":{\"groupId\":0,\"groupName\":\"string\",\"id\":0,\"name\":\"string\",\"description\":\"string\",\"permanent\":true},\"callbackData\":\"string\"}]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/sms/status");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/sms/status HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 502

{"results":[{"bulkId":"string","messageId":"string","to":"string","from":"string","text":"string","sentAt":"2019-08-24T14:15:22Z","doneAt":"2019-08-24T14:15:22Z","smsCount":0,"mccMnc":"string","price":{"pricePerMessage":0,"pricePerLookup":0,"currency":"string"},"status":{"groupId":0,"groupName":"string","id":0,"name":"string","description":"string","action":"string"},"error":{"groupId":0,"groupName":"string","id":0,"name":"string","description":"string","permanent":true},"callbackData":"string"}]}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/sms/status")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"results\":[{\"bulkId\":\"string\",\"messageId\":\"string\",\"to\":\"string\",\"from\":\"string\",\"text\":\"string\",\"sentAt\":\"2019-08-24T14:15:22Z\",\"doneAt\":\"2019-08-24T14:15:22Z\",\"smsCount\":0,\"mccMnc\":\"string\",\"price\":{\"pricePerMessage\":0,\"pricePerLookup\":0,\"currency\":\"string\"},\"status\":{\"groupId\":0,\"groupName\":\"string\",\"id\":0,\"name\":\"string\",\"description\":\"string\",\"action\":\"string\"},\"error\":{\"groupId\":0,\"groupName\":\"string\",\"id\":0,\"name\":\"string\",\"description\":\"string\",\"permanent\":true},\"callbackData\":\"string\"}]}")
  .asString();
```

`POST /api/sms/status`

> Body parameter

```json
{
  "results": [
    {
      "bulkId": "string",
      "messageId": "string",
      "to": "string",
      "from": "string",
      "text": "string",
      "sentAt": "2019-08-24T14:15:22Z",
      "doneAt": "2019-08-24T14:15:22Z",
      "smsCount": 0,
      "mccMnc": "string",
      "price": {
        "pricePerMessage": 0,
        "pricePerLookup": 0,
        "currency": "string"
      },
      "status": {
        "groupId": 0,
        "groupName": "string",
        "id": 0,
        "name": "string",
        "description": "string",
        "action": "string"
      },
      "error": {
        "groupId": 0,
        "groupName": "string",
        "id": 0,
        "name": "string",
        "description": "string",
        "permanent": true
      },
      "callbackData": "string"
    }
  ]
}
```

<h3 id="post__api_sms_status-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[SMSReportResponse](#schemasmsreportresponse)|false|none|

<h3 id="post__api_sms_status-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-speaker">Speaker</h1>

## get__api_event_{eventIdOrSlug}_speakers

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/speakers");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/event/string/speakers", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/event/string/speakers");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/event/string/speakers HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/event/string/speakers")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/event/{eventIdOrSlug}/speakers`

<h3 id="get__api_event_{eventidorslug}_speakers-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|

<h3 id="get__api_event_{eventidorslug}_speakers-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_event_{eventId}_speakers_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/speakers/string");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("DELETE", "/api/event/string/speakers/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/event/string/speakers/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/event/string/speakers/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/event/string/speakers/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`DELETE /api/event/{eventId}/speakers/{entryId}`

<h3 id="delete__api_event_{eventid}_speakers_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|

<h3 id="delete__api_event_{eventid}_speakers_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_event_{eventId}_speakers_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/speakers/string");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"eventId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"jobTitle\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"description\":\"string\",\"profileImageUrl\":\"string\",\"order\":0,\"links\":[{\"url\":\"string\"}]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"eventId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"jobTitle\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"description\":\"string\",\"profileImageUrl\":\"string\",\"order\":0,\"links\":[{\"url\":\"string\"}]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/event/string/speakers/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"eventId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"jobTitle\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"description\":\"string\",\"profileImageUrl\":\"string\",\"order\":0,\"links\":[{\"url\":\"string\"}]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/event/string/speakers/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/event/string/speakers/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 236

{"id":"string","eventId":"string","name":"string","lastName":"string","company":"string","jobTitle":"string","email":"string","phoneNumber":"string","description":"string","profileImageUrl":"string","order":0,"links":[{"url":"string"}]}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/event/string/speakers/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"eventId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"jobTitle\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"description\":\"string\",\"profileImageUrl\":\"string\",\"order\":0,\"links\":[{\"url\":\"string\"}]}")
  .asString();
```

`PUT /api/event/{eventId}/speakers/{entryId}`

> Body parameter

```json
{
  "id": "string",
  "eventId": "string",
  "name": "string",
  "lastName": "string",
  "company": "string",
  "jobTitle": "string",
  "email": "string",
  "phoneNumber": "string",
  "description": "string",
  "profileImageUrl": "string",
  "order": 0,
  "links": [
    {
      "url": "string"
    }
  ]
}
```

<h3 id="put__api_event_{eventid}_speakers_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|
|body|body|[SpeakerDto](#schemaspeakerdto)|false|none|

<h3 id="put__api_event_{eventid}_speakers_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## patch__api_event_{eventId}_speakers_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/speakers/string");
var request = new RestRequest(Method.PATCH);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PATCH", "/api/event/string/speakers/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PATCH", "https://example.com/api/event/string/speakers/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PATCH /api/event/string/speakers/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 2

{}
```

```java
HttpResponse<String> response = Unirest.patch("https://example.com/api/event/string/speakers/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{}")
  .asString();
```

`PATCH /api/event/{eventId}/speakers/{entryId}`

> Body parameter

```json
{}
```

<h3 id="patch__api_event_{eventid}_speakers_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|
|body|body|[PartialSpeakerDto](#schemapartialspeakerdto)|false|none|

<h3 id="patch__api_event_{eventid}_speakers_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_event_{eventId}_speakers

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/speakers");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"eventId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"jobTitle\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"description\":\"string\",\"profileImageUrl\":\"string\",\"order\":0,\"links\":[{\"url\":\"string\"}]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"eventId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"jobTitle\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"description\":\"string\",\"profileImageUrl\":\"string\",\"order\":0,\"links\":[{\"url\":\"string\"}]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/event/string/speakers", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"eventId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"jobTitle\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"description\":\"string\",\"profileImageUrl\":\"string\",\"order\":0,\"links\":[{\"url\":\"string\"}]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/event/string/speakers");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/event/string/speakers HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 236

{"id":"string","eventId":"string","name":"string","lastName":"string","company":"string","jobTitle":"string","email":"string","phoneNumber":"string","description":"string","profileImageUrl":"string","order":0,"links":[{"url":"string"}]}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/event/string/speakers")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"eventId\":\"string\",\"name\":\"string\",\"lastName\":\"string\",\"company\":\"string\",\"jobTitle\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"description\":\"string\",\"profileImageUrl\":\"string\",\"order\":0,\"links\":[{\"url\":\"string\"}]}")
  .asString();
```

`POST /api/event/{eventId}/speakers`

> Body parameter

```json
{
  "id": "string",
  "eventId": "string",
  "name": "string",
  "lastName": "string",
  "company": "string",
  "jobTitle": "string",
  "email": "string",
  "phoneNumber": "string",
  "description": "string",
  "profileImageUrl": "string",
  "order": 0,
  "links": [
    {
      "url": "string"
    }
  ]
}
```

<h3 id="post__api_event_{eventid}_speakers-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[SpeakerDto](#schemaspeakerdto)|false|none|

<h3 id="post__api_event_{eventid}_speakers-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## patch__api_event_{eventId}_speakers_reorder

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/speakers/reorder");
var request = new RestRequest(Method.PATCH);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"speakerIds\":[\"string\"]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"speakerIds\":[\"string\"]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PATCH", "/api/event/string/speakers/reorder", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"speakerIds\":[\"string\"]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PATCH", "https://example.com/api/event/string/speakers/reorder");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PATCH /api/event/string/speakers/reorder HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 25

{"speakerIds":["string"]}
```

```java
HttpResponse<String> response = Unirest.patch("https://example.com/api/event/string/speakers/reorder")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"speakerIds\":[\"string\"]}")
  .asString();
```

`PATCH /api/event/{eventId}/speakers/reorder`

> Body parameter

```json
{
  "speakerIds": [
    "string"
  ]
}
```

<h3 id="patch__api_event_{eventid}_speakers_reorder-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[ReorderSpeakerDto](#schemareorderspeakerdto)|false|none|

<h3 id="patch__api_event_{eventid}_speakers_reorder-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-sponsor">Sponsor</h1>

## get__api_event_{eventIdOrSlug}_sponsors

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/sponsors");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/event/string/sponsors", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/event/string/sponsors");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/event/string/sponsors HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/event/string/sponsors")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/event/{eventIdOrSlug}/sponsors`

<h3 id="get__api_event_{eventidorslug}_sponsors-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|

<h3 id="get__api_event_{eventidorslug}_sponsors-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_event_{eventId}_sponsors_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/sponsors/string");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("DELETE", "/api/event/string/sponsors/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/event/string/sponsors/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/event/string/sponsors/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/event/string/sponsors/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`DELETE /api/event/{eventId}/sponsors/{entryId}`

<h3 id="delete__api_event_{eventid}_sponsors_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|

<h3 id="delete__api_event_{eventid}_sponsors_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_event_{eventId}_sponsors_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/sponsors/string");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"name\":\"string\",\"logoUrl\":\"string\",\"description\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"website\":\"string\",\"address\":\"string\",\"links\":[{\"url\":\"string\"}],\"stageStream\":{\"type\":0,\"url\":\"string\",\"hostUrl\":\"string\",\"additionalUrls\":[{\"type\":0,\"url\":\"string\"}],\"rtmpSettings\":{\"streamKey\":\"string\",\"channelArn\":\"string\",\"recordings\":[\"string\"]},\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\"}},\"order\":0,\"isStreamTypeChangeForced\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"name\":\"string\",\"logoUrl\":\"string\",\"description\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"website\":\"string\",\"address\":\"string\",\"links\":[{\"url\":\"string\"}],\"stageStream\":{\"type\":0,\"url\":\"string\",\"hostUrl\":\"string\",\"additionalUrls\":[{\"type\":0,\"url\":\"string\"}],\"rtmpSettings\":{\"streamKey\":\"string\",\"channelArn\":\"string\",\"recordings\":[\"string\"]},\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\"}},\"order\":0,\"isStreamTypeChangeForced\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/event/string/sponsors/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"name\":\"string\",\"logoUrl\":\"string\",\"description\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"website\":\"string\",\"address\":\"string\",\"links\":[{\"url\":\"string\"}],\"stageStream\":{\"type\":0,\"url\":\"string\",\"hostUrl\":\"string\",\"additionalUrls\":[{\"type\":0,\"url\":\"string\"}],\"rtmpSettings\":{\"streamKey\":\"string\",\"channelArn\":\"string\",\"recordings\":[\"string\"]},\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\"}},\"order\":0,\"isStreamTypeChangeForced\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/event/string/sponsors/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/event/string/sponsors/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 953

{"id":"string","name":"string","logoUrl":"string","description":"string","email":"string","phoneNumber":"string","website":"string","address":"string","links":[{"url":"string"}],"stageStream":{"type":0,"url":"string","hostUrl":"string","additionalUrls":[{"type":0,"url":"string"}],"rtmpSettings":{"streamKey":"string","channelArn":"string","recordings":["string"]},"settings":{"host":{"isChatEnabled":true,"isPeopleEnabled":true,"isLeaveButtonEnabled":true,"isRecordingEnabled":true,"isScreenShareEnabled":true,"isBackgroundEnabled":true,"isVideoEnabled":true,"isAudioEnabled":true,"isBreakoutEnabled":true},"stream":{"isChatEnabled":true,"isPeopleEnabled":true,"isLeaveButtonEnabled":true,"isRecordingEnabled":true,"isScreenShareEnabled":true,"isBackgroundEnabled":true,"isVideoEnabled":true,"isAudioEnabled":true,"isBreakoutEnabled":true},"startDate":"2019-08-24T14:15:22Z","endDate":"2019-08-24T14:15:22Z"}},"order":0,"isStreamTypeChangeForced":true}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/event/string/sponsors/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"name\":\"string\",\"logoUrl\":\"string\",\"description\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"website\":\"string\",\"address\":\"string\",\"links\":[{\"url\":\"string\"}],\"stageStream\":{\"type\":0,\"url\":\"string\",\"hostUrl\":\"string\",\"additionalUrls\":[{\"type\":0,\"url\":\"string\"}],\"rtmpSettings\":{\"streamKey\":\"string\",\"channelArn\":\"string\",\"recordings\":[\"string\"]},\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\"}},\"order\":0,\"isStreamTypeChangeForced\":true}")
  .asString();
```

`PUT /api/event/{eventId}/sponsors/{entryId}`

> Body parameter

```json
{
  "id": "string",
  "name": "string",
  "logoUrl": "string",
  "description": "string",
  "email": "string",
  "phoneNumber": "string",
  "website": "string",
  "address": "string",
  "links": [
    {
      "url": "string"
    }
  ],
  "stageStream": {
    "type": 0,
    "url": "string",
    "hostUrl": "string",
    "additionalUrls": [
      {
        "type": 0,
        "url": "string"
      }
    ],
    "rtmpSettings": {
      "streamKey": "string",
      "channelArn": "string",
      "recordings": [
        "string"
      ]
    },
    "settings": {
      "host": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      },
      "stream": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      },
      "startDate": "2019-08-24T14:15:22Z",
      "endDate": "2019-08-24T14:15:22Z"
    }
  },
  "order": 0,
  "isStreamTypeChangeForced": true
}
```

<h3 id="put__api_event_{eventid}_sponsors_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|
|body|body|[SaveSponsorDto](#schemasavesponsordto)|false|none|

<h3 id="put__api_event_{eventid}_sponsors_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## patch__api_event_{eventId}_sponsors_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/sponsors/string");
var request = new RestRequest(Method.PATCH);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"name\":\"string\",\"logoUrl\":\"string\",\"description\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"website\":\"string\",\"address\":\"string\",\"links\":[{\"url\":\"string\"}],\"order\":0}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"name\":\"string\",\"logoUrl\":\"string\",\"description\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"website\":\"string\",\"address\":\"string\",\"links\":[{\"url\":\"string\"}],\"order\":0}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PATCH", "/api/event/string/sponsors/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"name\":\"string\",\"logoUrl\":\"string\",\"description\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"website\":\"string\",\"address\":\"string\",\"links\":[{\"url\":\"string\"}],\"order\":0}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PATCH", "https://example.com/api/event/string/sponsors/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PATCH /api/event/string/sponsors/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 174

{"name":"string","logoUrl":"string","description":"string","email":"string","phoneNumber":"string","website":"string","address":"string","links":[{"url":"string"}],"order":0}
```

```java
HttpResponse<String> response = Unirest.patch("https://example.com/api/event/string/sponsors/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"name\":\"string\",\"logoUrl\":\"string\",\"description\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"website\":\"string\",\"address\":\"string\",\"links\":[{\"url\":\"string\"}],\"order\":0}")
  .asString();
```

`PATCH /api/event/{eventId}/sponsors/{entryId}`

> Body parameter

```json
{
  "name": "string",
  "logoUrl": "string",
  "description": "string",
  "email": "string",
  "phoneNumber": "string",
  "website": "string",
  "address": "string",
  "links": [
    {
      "url": "string"
    }
  ],
  "order": 0
}
```

<h3 id="patch__api_event_{eventid}_sponsors_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|
|body|body|[PartialSponsorDto](#schemapartialsponsordto)|false|none|

<h3 id="patch__api_event_{eventid}_sponsors_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_event_{eventId}_sponsors

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/sponsors");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"name\":\"string\",\"logoUrl\":\"string\",\"description\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"website\":\"string\",\"address\":\"string\",\"links\":[{\"url\":\"string\"}],\"stageStream\":{\"type\":0,\"url\":\"string\",\"hostUrl\":\"string\",\"additionalUrls\":[{\"type\":0,\"url\":\"string\"}],\"rtmpSettings\":{\"streamKey\":\"string\",\"channelArn\":\"string\",\"recordings\":[\"string\"]},\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\"}},\"order\":0,\"isStreamTypeChangeForced\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"name\":\"string\",\"logoUrl\":\"string\",\"description\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"website\":\"string\",\"address\":\"string\",\"links\":[{\"url\":\"string\"}],\"stageStream\":{\"type\":0,\"url\":\"string\",\"hostUrl\":\"string\",\"additionalUrls\":[{\"type\":0,\"url\":\"string\"}],\"rtmpSettings\":{\"streamKey\":\"string\",\"channelArn\":\"string\",\"recordings\":[\"string\"]},\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\"}},\"order\":0,\"isStreamTypeChangeForced\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/event/string/sponsors", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"name\":\"string\",\"logoUrl\":\"string\",\"description\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"website\":\"string\",\"address\":\"string\",\"links\":[{\"url\":\"string\"}],\"stageStream\":{\"type\":0,\"url\":\"string\",\"hostUrl\":\"string\",\"additionalUrls\":[{\"type\":0,\"url\":\"string\"}],\"rtmpSettings\":{\"streamKey\":\"string\",\"channelArn\":\"string\",\"recordings\":[\"string\"]},\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\"}},\"order\":0,\"isStreamTypeChangeForced\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/event/string/sponsors");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/event/string/sponsors HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 953

{"id":"string","name":"string","logoUrl":"string","description":"string","email":"string","phoneNumber":"string","website":"string","address":"string","links":[{"url":"string"}],"stageStream":{"type":0,"url":"string","hostUrl":"string","additionalUrls":[{"type":0,"url":"string"}],"rtmpSettings":{"streamKey":"string","channelArn":"string","recordings":["string"]},"settings":{"host":{"isChatEnabled":true,"isPeopleEnabled":true,"isLeaveButtonEnabled":true,"isRecordingEnabled":true,"isScreenShareEnabled":true,"isBackgroundEnabled":true,"isVideoEnabled":true,"isAudioEnabled":true,"isBreakoutEnabled":true},"stream":{"isChatEnabled":true,"isPeopleEnabled":true,"isLeaveButtonEnabled":true,"isRecordingEnabled":true,"isScreenShareEnabled":true,"isBackgroundEnabled":true,"isVideoEnabled":true,"isAudioEnabled":true,"isBreakoutEnabled":true},"startDate":"2019-08-24T14:15:22Z","endDate":"2019-08-24T14:15:22Z"}},"order":0,"isStreamTypeChangeForced":true}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/event/string/sponsors")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"name\":\"string\",\"logoUrl\":\"string\",\"description\":\"string\",\"email\":\"string\",\"phoneNumber\":\"string\",\"website\":\"string\",\"address\":\"string\",\"links\":[{\"url\":\"string\"}],\"stageStream\":{\"type\":0,\"url\":\"string\",\"hostUrl\":\"string\",\"additionalUrls\":[{\"type\":0,\"url\":\"string\"}],\"rtmpSettings\":{\"streamKey\":\"string\",\"channelArn\":\"string\",\"recordings\":[\"string\"]},\"settings\":{\"host\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"stream\":{\"isChatEnabled\":true,\"isPeopleEnabled\":true,\"isLeaveButtonEnabled\":true,\"isRecordingEnabled\":true,\"isScreenShareEnabled\":true,\"isBackgroundEnabled\":true,\"isVideoEnabled\":true,\"isAudioEnabled\":true,\"isBreakoutEnabled\":true},\"startDate\":\"2019-08-24T14:15:22Z\",\"endDate\":\"2019-08-24T14:15:22Z\"}},\"order\":0,\"isStreamTypeChangeForced\":true}")
  .asString();
```

`POST /api/event/{eventId}/sponsors`

> Body parameter

```json
{
  "id": "string",
  "name": "string",
  "logoUrl": "string",
  "description": "string",
  "email": "string",
  "phoneNumber": "string",
  "website": "string",
  "address": "string",
  "links": [
    {
      "url": "string"
    }
  ],
  "stageStream": {
    "type": 0,
    "url": "string",
    "hostUrl": "string",
    "additionalUrls": [
      {
        "type": 0,
        "url": "string"
      }
    ],
    "rtmpSettings": {
      "streamKey": "string",
      "channelArn": "string",
      "recordings": [
        "string"
      ]
    },
    "settings": {
      "host": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      },
      "stream": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      },
      "startDate": "2019-08-24T14:15:22Z",
      "endDate": "2019-08-24T14:15:22Z"
    }
  },
  "order": 0,
  "isStreamTypeChangeForced": true
}
```

<h3 id="post__api_event_{eventid}_sponsors-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[SaveSponsorDto](#schemasavesponsordto)|false|none|

<h3 id="post__api_event_{eventid}_sponsors-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## patch__api_event_{eventId}_sponsors_reorder

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/sponsors/reorder");
var request = new RestRequest(Method.PATCH);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"sponsorIds\":[\"string\"]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"sponsorIds\":[\"string\"]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PATCH", "/api/event/string/sponsors/reorder", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"sponsorIds\":[\"string\"]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PATCH", "https://example.com/api/event/string/sponsors/reorder");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PATCH /api/event/string/sponsors/reorder HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 25

{"sponsorIds":["string"]}
```

```java
HttpResponse<String> response = Unirest.patch("https://example.com/api/event/string/sponsors/reorder")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"sponsorIds\":[\"string\"]}")
  .asString();
```

`PATCH /api/event/{eventId}/sponsors/reorder`

> Body parameter

```json
{
  "sponsorIds": [
    "string"
  ]
}
```

<h3 id="patch__api_event_{eventid}_sponsors_reorder-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[ReorderSponsorDto](#schemareordersponsordto)|false|none|

<h3 id="patch__api_event_{eventid}_sponsors_reorder-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-template">Template</h1>

## get__api_Template_{eventIdOrSlug}_{type}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Template/string/0");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Template/string/0", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Template/string/0");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Template/string/0 HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Template/string/0")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Template/{eventIdOrSlug}/{type}`

<h3 id="get__api_template_{eventidorslug}_{type}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|
|type|path|[TemplateType](#schematemplatetype)|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|type|0|
|type|1|

<h3 id="get__api_template_{eventidorslug}_{type}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Template_{eventIdOrSlug}_{type}_editor

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Template/string/0/editor");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Template/string/0/editor", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Template/string/0/editor");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Template/string/0/editor HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Template/string/0/editor")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Template/{eventIdOrSlug}/{type}/editor`

<h3 id="get__api_template_{eventidorslug}_{type}_editor-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|
|type|path|[TemplateType](#schematemplatetype)|true|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|type|0|
|type|1|

<h3 id="get__api_template_{eventidorslug}_{type}_editor-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_Template_{eventId}_delete_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Template/string/delete/string");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("DELETE", "/api/Template/string/delete/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/Template/string/delete/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/Template/string/delete/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/Template/string/delete/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`DELETE /api/Template/{eventId}/delete/{entryId}`

<h3 id="delete__api_template_{eventid}_delete_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|

<h3 id="delete__api_template_{eventid}_delete_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Template_{eventId}_create

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Template/string/create");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"code\":\"string\",\"name\":\"string\",\"description\":\"string\",\"content\":\"string\",\"subject\":\"string\",\"emailSenderIdentityId\":\"string\",\"type\":0}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"code\":\"string\",\"name\":\"string\",\"description\":\"string\",\"content\":\"string\",\"subject\":\"string\",\"emailSenderIdentityId\":\"string\",\"type\":0}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Template/string/create", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"code\":\"string\",\"name\":\"string\",\"description\":\"string\",\"content\":\"string\",\"subject\":\"string\",\"emailSenderIdentityId\":\"string\",\"type\":0}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Template/string/create");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Template/string/create HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 185

{"id":"string","createdOn":"2019-08-24T14:15:22Z","code":"string","name":"string","description":"string","content":"string","subject":"string","emailSenderIdentityId":"string","type":0}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Template/string/create")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"code\":\"string\",\"name\":\"string\",\"description\":\"string\",\"content\":\"string\",\"subject\":\"string\",\"emailSenderIdentityId\":\"string\",\"type\":0}")
  .asString();
```

`POST /api/Template/{eventId}/create`

> Body parameter

```json
{
  "id": "string",
  "createdOn": "2019-08-24T14:15:22Z",
  "code": "string",
  "name": "string",
  "description": "string",
  "content": "string",
  "subject": "string",
  "emailSenderIdentityId": "string",
  "type": 0
}
```

<h3 id="post__api_template_{eventid}_create-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[TemplateDto](#schematemplatedto)|false|none|

<h3 id="post__api_template_{eventid}_create-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_Template_{eventId}_update_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Template/string/update/string");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"id\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"code\":\"string\",\"name\":\"string\",\"description\":\"string\",\"content\":\"string\",\"subject\":\"string\",\"emailSenderIdentityId\":\"string\",\"type\":0}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"id\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"code\":\"string\",\"name\":\"string\",\"description\":\"string\",\"content\":\"string\",\"subject\":\"string\",\"emailSenderIdentityId\":\"string\",\"type\":0}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/Template/string/update/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"id\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"code\":\"string\",\"name\":\"string\",\"description\":\"string\",\"content\":\"string\",\"subject\":\"string\",\"emailSenderIdentityId\":\"string\",\"type\":0}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/Template/string/update/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/Template/string/update/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 185

{"id":"string","createdOn":"2019-08-24T14:15:22Z","code":"string","name":"string","description":"string","content":"string","subject":"string","emailSenderIdentityId":"string","type":0}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/Template/string/update/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"id\":\"string\",\"createdOn\":\"2019-08-24T14:15:22Z\",\"code\":\"string\",\"name\":\"string\",\"description\":\"string\",\"content\":\"string\",\"subject\":\"string\",\"emailSenderIdentityId\":\"string\",\"type\":0}")
  .asString();
```

`PUT /api/Template/{eventId}/update/{entryId}`

> Body parameter

```json
{
  "id": "string",
  "createdOn": "2019-08-24T14:15:22Z",
  "code": "string",
  "name": "string",
  "description": "string",
  "content": "string",
  "subject": "string",
  "emailSenderIdentityId": "string",
  "type": 0
}
```

<h3 id="put__api_template_{eventid}_update_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|
|body|body|[TemplateDto](#schematemplatedto)|false|none|

<h3 id="put__api_template_{eventid}_update_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## patch__api_Template_{eventId}_reorder

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Template/string/reorder");
var request = new RestRequest(Method.PATCH);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"templateIds\":[\"string\"]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"templateIds\":[\"string\"]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PATCH", "/api/Template/string/reorder", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"templateIds\":[\"string\"]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PATCH", "https://example.com/api/Template/string/reorder");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PATCH /api/Template/string/reorder HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 26

{"templateIds":["string"]}
```

```java
HttpResponse<String> response = Unirest.patch("https://example.com/api/Template/string/reorder")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"templateIds\":[\"string\"]}")
  .asString();
```

`PATCH /api/Template/{eventId}/reorder`

> Body parameter

```json
{
  "templateIds": [
    "string"
  ]
}
```

<h3 id="patch__api_template_{eventid}_reorder-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|body|body|[ReorderTemplateDto](#schemareordertemplatedto)|false|none|

<h3 id="patch__api_template_{eventid}_reorder-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-timeline">Timeline</h1>

## get__api_event_{eventIdOrSlug}_timeline

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/timeline");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/event/string/timeline", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/event/string/timeline");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/event/string/timeline HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/event/string/timeline")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/event/{eventIdOrSlug}/timeline`

<h3 id="get__api_event_{eventidorslug}_timeline-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventIdOrSlug|path|string|true|none|

<h3 id="get__api_event_{eventidorslug}_timeline-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_event_{eventId}_timeline_{entryId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/event/string/timeline/string");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("DELETE", "/api/event/string/timeline/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/event/string/timeline/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/event/string/timeline/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/event/string/timeline/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`DELETE /api/event/{eventId}/timeline/{entryId}`

<h3 id="delete__api_event_{eventid}_timeline_{entryid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|entryId|path|string|true|none|

<h3 id="delete__api_event_{eventid}_timeline_{entryid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-upload">Upload</h1>

## post__api_Upload_{eventId}_files

> Code samples

`POST /api/Upload/{eventId}/files`

> Body parameter

```yaml
files:
  - string

```

<h3 id="post__api_upload_{eventid}_files-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|resizeTo|query|integer(int32)|false|none|
|body|body|object|false|none|
|» files|body|[string]|false|none|

<h3 id="post__api_upload_{eventid}_files-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Upload_single

> Code samples

`POST /api/Upload/single`

> Body parameter

```yaml
eventId: string
files:
  - string

```

<h3 id="post__api_upload_single-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|object|false|none|
|» eventId|body|string|false|none|
|» files|body|[string]|false|none|

<h3 id="post__api_upload_single-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Upload_{eventId}_invitees

> Code samples

`POST /api/Upload/{eventId}/invitees`

> Body parameter

```yaml
Files:
  - string

```

<h3 id="post__api_upload_{eventid}_invitees-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|eventId|path|string|true|none|
|MetadataJson|query|string|false|none|
|body|body|object|false|none|
|» Files|body|[string]|false|none|

<h3 id="post__api_upload_{eventid}_invitees-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Upload_{workspaceId}

> Code samples

`POST /api/Upload/{workspaceId}`

> Body parameter

```yaml
Files:
  - string

```

<h3 id="post__api_upload_{workspaceid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|workspaceId|path|string|true|none|
|body|body|object|false|none|
|» Files|body|[string]|false|none|

<h3 id="post__api_upload_{workspaceid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-userinfo">Userinfo</h1>

## get__connect_userinfo

> Code samples

```csharp
var client = new RestClient("https://example.com/connect/userinfo");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/connect/userinfo", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/connect/userinfo");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /connect/userinfo HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/connect/userinfo")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /connect/userinfo`

<h3 id="get__connect_userinfo-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__connect_userinfo

> Code samples

```csharp
var client = new RestClient("https://example.com/connect/userinfo");
var request = new RestRequest(Method.POST);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("POST", "/connect/userinfo", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/connect/userinfo");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /connect/userinfo HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.post("https://example.com/connect/userinfo")
  .header("Authorization", "API_KEY")
  .asString();
```

`POST /connect/userinfo`

<h3 id="post__connect_userinfo-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-users">Users</h1>

## get__api_Users

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Users");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Users", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Users");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Users HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Users")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Users`

<h3 id="get__api_users-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Users_current

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Users/current");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Users/current", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Users/current");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Users/current HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Users/current")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Users/current`

<h3 id="get__api_users_current-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_Users_current

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Users/current");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"name\":\"string\",\"lastName\":\"string\",\"phoneNumber\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"name\":\"string\",\"lastName\":\"string\",\"phoneNumber\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/Users/current", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"name\":\"string\",\"lastName\":\"string\",\"phoneNumber\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/Users/current");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/Users/current HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 60

{"name":"string","lastName":"string","phoneNumber":"string"}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/Users/current")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"name\":\"string\",\"lastName\":\"string\",\"phoneNumber\":\"string\"}")
  .asString();
```

`PUT /api/Users/current`

> Body parameter

```json
{
  "name": "string",
  "lastName": "string",
  "phoneNumber": "string"
}
```

<h3 id="put__api_users_current-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[UpdateUserDto](#schemaupdateuserdto)|false|none|

<h3 id="put__api_users_current-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_Users_workspace

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Users/workspace");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"workspaceId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"workspaceId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/Users/workspace", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"workspaceId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/Users/workspace");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/Users/workspace HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 24

{"workspaceId":"string"}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/Users/workspace")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"workspaceId\":\"string\"}")
  .asString();
```

`PUT /api/Users/workspace`

> Body parameter

```json
{
  "workspaceId": "string"
}
```

<h3 id="put__api_users_workspace-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[UpdateUserWorkspaceDto](#schemaupdateuserworkspacedto)|false|none|

<h3 id="put__api_users_workspace-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

<h1 id="ems-api-workspace">Workspace</h1>

## get__api_Workspace

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Workspace");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Workspace", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Workspace");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Workspace HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Workspace")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Workspace`

<h3 id="get__api_workspace-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|Simple|query|boolean|false|none|

<h3 id="get__api_workspace-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Workspace_create

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Workspace/create");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"name\":\"string\",\"companyId\":\"string\",\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"contactName\":\"string\",\"zipCode\":\"string\",\"city\":\"string\",\"state\":\"string\",\"country\":\"string\",\"contactLastName\":\"string\",\"phone\":\"string\",\"invoiceEmail\":\"user@example.com\",\"partnerWorkspaceId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"name\":\"string\",\"companyId\":\"string\",\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"contactName\":\"string\",\"zipCode\":\"string\",\"city\":\"string\",\"state\":\"string\",\"country\":\"string\",\"contactLastName\":\"string\",\"phone\":\"string\",\"invoiceEmail\":\"user@example.com\",\"partnerWorkspaceId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Workspace/create", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"name\":\"string\",\"companyId\":\"string\",\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"contactName\":\"string\",\"zipCode\":\"string\",\"city\":\"string\",\"state\":\"string\",\"country\":\"string\",\"contactLastName\":\"string\",\"phone\":\"string\",\"invoiceEmail\":\"user@example.com\",\"partnerWorkspaceId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Workspace/create");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Workspace/create HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 288

{"name":"string","companyId":"string","addressLine1":"string","addressLine2":"string","contactName":"string","zipCode":"string","city":"string","state":"string","country":"string","contactLastName":"string","phone":"string","invoiceEmail":"user@example.com","partnerWorkspaceId":"string"}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Workspace/create")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"name\":\"string\",\"companyId\":\"string\",\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"contactName\":\"string\",\"zipCode\":\"string\",\"city\":\"string\",\"state\":\"string\",\"country\":\"string\",\"contactLastName\":\"string\",\"phone\":\"string\",\"invoiceEmail\":\"user@example.com\",\"partnerWorkspaceId\":\"string\"}")
  .asString();
```

`POST /api/Workspace/create`

> Body parameter

```json
{
  "name": "string",
  "companyId": "string",
  "addressLine1": "string",
  "addressLine2": "string",
  "contactName": "string",
  "zipCode": "string",
  "city": "string",
  "state": "string",
  "country": "string",
  "contactLastName": "string",
  "phone": "string",
  "invoiceEmail": "user@example.com",
  "partnerWorkspaceId": "string"
}
```

<h3 id="post__api_workspace_create-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[SaveWorkspaceDto](#schemasaveworkspacedto)|false|none|

<h3 id="post__api_workspace_create-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_Workspace_{workspaceId}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Workspace/string");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"name\":\"string\",\"companyId\":\"string\",\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"contactName\":\"string\",\"zipCode\":\"string\",\"city\":\"string\",\"state\":\"string\",\"country\":\"string\",\"contactLastName\":\"string\",\"phone\":\"string\",\"invoiceEmail\":\"user@example.com\",\"partnerWorkspaceId\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"name\":\"string\",\"companyId\":\"string\",\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"contactName\":\"string\",\"zipCode\":\"string\",\"city\":\"string\",\"state\":\"string\",\"country\":\"string\",\"contactLastName\":\"string\",\"phone\":\"string\",\"invoiceEmail\":\"user@example.com\",\"partnerWorkspaceId\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/Workspace/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"name\":\"string\",\"companyId\":\"string\",\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"contactName\":\"string\",\"zipCode\":\"string\",\"city\":\"string\",\"state\":\"string\",\"country\":\"string\",\"contactLastName\":\"string\",\"phone\":\"string\",\"invoiceEmail\":\"user@example.com\",\"partnerWorkspaceId\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/Workspace/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/Workspace/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 288

{"name":"string","companyId":"string","addressLine1":"string","addressLine2":"string","contactName":"string","zipCode":"string","city":"string","state":"string","country":"string","contactLastName":"string","phone":"string","invoiceEmail":"user@example.com","partnerWorkspaceId":"string"}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/Workspace/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"name\":\"string\",\"companyId\":\"string\",\"addressLine1\":\"string\",\"addressLine2\":\"string\",\"contactName\":\"string\",\"zipCode\":\"string\",\"city\":\"string\",\"state\":\"string\",\"country\":\"string\",\"contactLastName\":\"string\",\"phone\":\"string\",\"invoiceEmail\":\"user@example.com\",\"partnerWorkspaceId\":\"string\"}")
  .asString();
```

`PUT /api/Workspace/{workspaceId}`

> Body parameter

```json
{
  "name": "string",
  "companyId": "string",
  "addressLine1": "string",
  "addressLine2": "string",
  "contactName": "string",
  "zipCode": "string",
  "city": "string",
  "state": "string",
  "country": "string",
  "contactLastName": "string",
  "phone": "string",
  "invoiceEmail": "user@example.com",
  "partnerWorkspaceId": "string"
}
```

<h3 id="put__api_workspace_{workspaceid}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|workspaceId|path|string|true|none|
|body|body|[SaveWorkspaceDto](#schemasaveworkspacedto)|false|none|

<h3 id="put__api_workspace_{workspaceid}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_Workspace_users

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Workspace/users");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"workspaceId\":\"string\",\"users\":[\"string\"]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"workspaceId\":\"string\",\"users\":[\"string\"]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/Workspace/users", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"workspaceId\":\"string\",\"users\":[\"string\"]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/Workspace/users");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/Workspace/users HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 43

{"workspaceId":"string","users":["string"]}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/Workspace/users")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"workspaceId\":\"string\",\"users\":[\"string\"]}")
  .asString();
```

`PUT /api/Workspace/users`

> Body parameter

```json
{
  "workspaceId": "string",
  "users": [
    "string"
  ]
}
```

<h3 id="put__api_workspace_users-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[AddWorkspaceUsersDto](#schemaaddworkspaceusersdto)|false|none|

<h3 id="put__api_workspace_users-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## delete__api_Workspace_user

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Workspace/user");
var request = new RestRequest(Method.DELETE);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"workspaceId\":\"string\",\"email\":\"string\"}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"workspaceId\":\"string\",\"email\":\"string\"}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("DELETE", "/api/Workspace/user", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"workspaceId\":\"string\",\"email\":\"string\"}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("DELETE", "https://example.com/api/Workspace/user");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
DELETE /api/Workspace/user HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 41

{"workspaceId":"string","email":"string"}
```

```java
HttpResponse<String> response = Unirest.delete("https://example.com/api/Workspace/user")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"workspaceId\":\"string\",\"email\":\"string\"}")
  .asString();
```

`DELETE /api/Workspace/user`

> Body parameter

```json
{
  "workspaceId": "string",
  "email": "string"
}
```

<h3 id="delete__api_workspace_user-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|body|body|[DeleteWorkspaceUserDto](#schemadeleteworkspaceuserdto)|false|none|

<h3 id="delete__api_workspace_user-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Workspace_{workspaceIdOrSlug}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Workspace/string");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Workspace/string", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Workspace/string");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Workspace/string HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Workspace/string")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Workspace/{workspaceIdOrSlug}`

<h3 id="get__api_workspace_{workspaceidorslug}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|workspaceIdOrSlug|path|string|true|none|

<h3 id="get__api_workspace_{workspaceidorslug}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Workspace_own

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Workspace/own");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Workspace/own", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Workspace/own");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Workspace/own HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Workspace/own")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Workspace/own`

<h3 id="get__api_workspace_own-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Workspace_{workspaceIdOrSlug}_limits

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Workspace/string/limits");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Workspace/string/limits", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Workspace/string/limits");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Workspace/string/limits HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Workspace/string/limits")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Workspace/{workspaceIdOrSlug}/limits`

<h3 id="get__api_workspace_{workspaceidorslug}_limits-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|workspaceIdOrSlug|path|string|true|none|

<h3 id="get__api_workspace_{workspaceidorslug}_limits-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Workspace_{workspaceIdOrSlug}_statistics

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Workspace/string/statistics");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Workspace/string/statistics", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Workspace/string/statistics");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Workspace/string/statistics HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Workspace/string/statistics")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Workspace/{workspaceIdOrSlug}/statistics`

<h3 id="get__api_workspace_{workspaceidorslug}_statistics-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|workspaceIdOrSlug|path|string|true|none|

<h3 id="get__api_workspace_{workspaceidorslug}_statistics-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## post__api_Workspace_invoicePaidHook_{token}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Workspace/invoicePaidHook/string");
var request = new RestRequest(Method.POST);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"property1\":[[]],\"property2\":[[]]}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"property1\":[[]],\"property2\":[[]]}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("POST", "/api/Workspace/invoicePaidHook/string", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"property1\":[[]],\"property2\":[[]]}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("POST", "https://example.com/api/Workspace/invoicePaidHook/string");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
POST /api/Workspace/invoicePaidHook/string HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 35

{"property1":[[]],"property2":[[]]}
```

```java
HttpResponse<String> response = Unirest.post("https://example.com/api/Workspace/invoicePaidHook/string")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"property1\":[[]],\"property2\":[[]]}")
  .asString();
```

`POST /api/Workspace/invoicePaidHook/{token}`

> Body parameter

```json
{
  "property1": [
    []
  ],
  "property2": [
    []
  ]
}
```

<h3 id="post__api_workspace_invoicepaidhook_{token}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|token|path|string|true|none|
|body|body|object|false|none|
|» **additionalProperties**|body|[[JToken](#schemajtoken)]|false|none|

<h3 id="post__api_workspace_invoicepaidhook_{token}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## get__api_Workspace_{workspaceIdOrSlug}_features

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Workspace/string/features");
var request = new RestRequest(Method.GET);
request.AddHeader("Authorization", "API_KEY");
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

headers = { 'Authorization': "API_KEY" }

conn.request("GET", "/api/Workspace/string/features", headers=headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = null;

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("GET", "https://example.com/api/Workspace/string/features");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
GET /api/Workspace/string/features HTTP/1.1
Authorization: API_KEY
Host: example.com

```

```java
HttpResponse<String> response = Unirest.get("https://example.com/api/Workspace/string/features")
  .header("Authorization", "API_KEY")
  .asString();
```

`GET /api/Workspace/{workspaceIdOrSlug}/features`

<h3 id="get__api_workspace_{workspaceidorslug}_features-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|workspaceIdOrSlug|path|string|true|none|

<h3 id="get__api_workspace_{workspaceidorslug}_features-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

## put__api_Workspace_{workspaceIdOrSlug}_features_{type}

> Code samples

```csharp
var client = new RestClient("https://example.com/api/Workspace/string/features/0");
var request = new RestRequest(Method.PUT);
request.AddHeader("Content-Type", "application/json-patch+json");
request.AddHeader("Authorization", "API_KEY");
request.AddParameter("application/json-patch+json", "{\"isSupportEnabled\":true,\"isLobbyPageEnabled\":true,\"isChatEnabled\":true,\"isSpeakersEnabled\":true,\"isAgendaEnabled\":true,\"isRTMPStreamEnabled\":true,\"isSponsorsEnabled\":true,\"isClientsAffected\":true}", ParameterType.RequestBody);
IRestResponse response = client.Execute(request);
```

```python
import http.client

conn = http.client.HTTPSConnection("example.com")

payload = "{\"isSupportEnabled\":true,\"isLobbyPageEnabled\":true,\"isChatEnabled\":true,\"isSpeakersEnabled\":true,\"isAgendaEnabled\":true,\"isRTMPStreamEnabled\":true,\"isSponsorsEnabled\":true,\"isClientsAffected\":true}"

headers = {
    'Content-Type': "application/json-patch+json",
    'Authorization': "API_KEY"
    }

conn.request("PUT", "/api/Workspace/string/features/0", payload, headers)

res = conn.getresponse()
data = res.read()

print(data.decode("utf-8"))
```

```javascript
const data = "{\"isSupportEnabled\":true,\"isLobbyPageEnabled\":true,\"isChatEnabled\":true,\"isSpeakersEnabled\":true,\"isAgendaEnabled\":true,\"isRTMPStreamEnabled\":true,\"isSponsorsEnabled\":true,\"isClientsAffected\":true}";

const xhr = new XMLHttpRequest();
xhr.withCredentials = true;

xhr.addEventListener("readystatechange", function () {
  if (this.readyState === this.DONE) {
    console.log(this.responseText);
  }
});

xhr.open("PUT", "https://example.com/api/Workspace/string/features/0");
xhr.setRequestHeader("Content-Type", "application/json-patch+json");
xhr.setRequestHeader("Authorization", "API_KEY");

xhr.send(data);
```

```http
PUT /api/Workspace/string/features/0 HTTP/1.1
Content-Type: application/json-patch+json
Authorization: API_KEY
Host: example.com
Content-Length: 197

{"isSupportEnabled":true,"isLobbyPageEnabled":true,"isChatEnabled":true,"isSpeakersEnabled":true,"isAgendaEnabled":true,"isRTMPStreamEnabled":true,"isSponsorsEnabled":true,"isClientsAffected":true}
```

```java
HttpResponse<String> response = Unirest.put("https://example.com/api/Workspace/string/features/0")
  .header("Content-Type", "application/json-patch+json")
  .header("Authorization", "API_KEY")
  .body("{\"isSupportEnabled\":true,\"isLobbyPageEnabled\":true,\"isChatEnabled\":true,\"isSpeakersEnabled\":true,\"isAgendaEnabled\":true,\"isRTMPStreamEnabled\":true,\"isSponsorsEnabled\":true,\"isClientsAffected\":true}")
  .asString();
```

`PUT /api/Workspace/{workspaceIdOrSlug}/features/{type}`

> Body parameter

```json
{
  "isSupportEnabled": true,
  "isLobbyPageEnabled": true,
  "isChatEnabled": true,
  "isSpeakersEnabled": true,
  "isAgendaEnabled": true,
  "isRTMPStreamEnabled": true,
  "isSponsorsEnabled": true,
  "isClientsAffected": true
}
```

<h3 id="put__api_workspace_{workspaceidorslug}_features_{type}-parameters">Parameters</h3>

|Name|In|Type|Required|Description|
|---|---|---|---|---|
|workspaceIdOrSlug|path|string|true|none|
|type|path|[WorkspaceFeatureType](#schemaworkspacefeaturetype)|true|none|
|body|body|[WorkspaceFeatureSetDto](#schemaworkspacefeaturesetdto)|false|none|

#### Enumerated Values

|Parameter|Value|
|---|---|
|type|0|
|type|1|

<h3 id="put__api_workspace_{workspaceidorslug}_features_{type}-responses">Responses</h3>

|Status|Meaning|Description|Schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|Success|None|

<aside class="warning">
To perform this operation, you must be authenticated by means of one of the following methods:
Bearer
</aside>

# Schemas

<h2 id="tocS_AddPartnerWorkspaceUsersDto">AddPartnerWorkspaceUsersDto</h2>
<!-- backwards compatibility -->
<a id="schemaaddpartnerworkspaceusersdto"></a>
<a id="schema_AddPartnerWorkspaceUsersDto"></a>
<a id="tocSaddpartnerworkspaceusersdto"></a>
<a id="tocsaddpartnerworkspaceusersdto"></a>

```json
{
  "partnerId": "string",
  "users": [
    "string"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|partnerId|string|true|none|none|
|users|[string]¦null|false|none|none|

<h2 id="tocS_AddSessionRequest">AddSessionRequest</h2>
<!-- backwards compatibility -->
<a id="schemaaddsessionrequest"></a>
<a id="schema_AddSessionRequest"></a>
<a id="tocSaddsessionrequest"></a>
<a id="tocsaddsessionrequest"></a>

```json
{
  "title": "string",
  "startDate": "2019-08-24T14:15:22Z",
  "endDate": "2019-08-24T14:15:22Z",
  "trackId": "string",
  "description": "string",
  "speakerIds": [
    "string"
  ],
  "stageStream": {
    "type": 0,
    "url": "string",
    "hostUrl": "string",
    "additionalUrls": [
      {
        "type": 0,
        "url": "string"
      }
    ],
    "rtmpSettings": {
      "streamKey": "string",
      "channelArn": "string",
      "recordings": [
        "string"
      ]
    },
    "settings": {
      "host": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      },
      "stream": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      },
      "startDate": "2019-08-24T14:15:22Z",
      "endDate": "2019-08-24T14:15:22Z"
    }
  },
  "groupIds": [
    "string"
  ],
  "isStreamTypeChangeForced": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|title|string|true|none|none|
|startDate|string(date-time)|true|none|none|
|endDate|string(date-time)|true|none|none|
|trackId|string|true|none|none|
|description|string¦null|false|none|none|
|speakerIds|[string]¦null|false|none|none|
|stageStream|[StageStreamDtoBase](#schemastagestreamdtobase)|false|none|none|
|groupIds|[string]¦null|false|none|none|
|isStreamTypeChangeForced|boolean|false|none|none|

<h2 id="tocS_AddTrackRequest">AddTrackRequest</h2>
<!-- backwards compatibility -->
<a id="schemaaddtrackrequest"></a>
<a id="schema_AddTrackRequest"></a>
<a id="tocSaddtrackrequest"></a>
<a id="tocsaddtrackrequest"></a>

```json
{
  "title": "string",
  "headerBackgroundColor": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|title|string|true|none|none|
|headerBackgroundColor|string|true|none|none|

<h2 id="tocS_AddWorkspaceUsersDto">AddWorkspaceUsersDto</h2>
<!-- backwards compatibility -->
<a id="schemaaddworkspaceusersdto"></a>
<a id="schema_AddWorkspaceUsersDto"></a>
<a id="tocSaddworkspaceusersdto"></a>
<a id="tocsaddworkspaceusersdto"></a>

```json
{
  "workspaceId": "string",
  "users": [
    "string"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|workspaceId|string|true|none|none|
|users|[string]¦null|false|none|none|

<h2 id="tocS_AdminLiveDocumentDto">AdminLiveDocumentDto</h2>
<!-- backwards compatibility -->
<a id="schemaadminlivedocumentdto"></a>
<a id="schema_AdminLiveDocumentDto"></a>
<a id="tocSadminlivedocumentdto"></a>
<a id="tocsadminlivedocumentdto"></a>

```json
{
  "id": "string",
  "createdOn": "2019-08-24T14:15:22Z",
  "title": "string",
  "description": "string",
  "documentUrl": "string",
  "isHidden": true,
  "order": 0,
  "groupIds": [
    "string"
  ],
  "platformPages": [
    0
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string¦null|false|none|none|
|createdOn|string(date-time)¦null|false|none|none|
|title|string¦null|false|none|none|
|description|string¦null|false|none|none|
|documentUrl|string¦null|false|none|none|
|isHidden|boolean¦null|false|none|none|
|order|integer(int32)¦null|false|none|none|
|groupIds|[string]¦null|false|none|none|
|platformPages|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|

<h2 id="tocS_AdminPollVoteDto">AdminPollVoteDto</h2>
<!-- backwards compatibility -->
<a id="schemaadminpollvotedto"></a>
<a id="schema_AdminPollVoteDto"></a>
<a id="tocSadminpollvotedto"></a>
<a id="tocsadminpollvotedto"></a>

```json
{
  "label": "string",
  "pollId": "string",
  "answeredBy": "string",
  "createdOn": "2019-08-24T14:15:22Z"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|label|string¦null|false|none|none|
|pollId|string¦null|false|none|none|
|answeredBy|string¦null|false|none|none|
|createdOn|string(date-time)|false|none|none|

<h2 id="tocS_BatchRegistrationGroupDto">BatchRegistrationGroupDto</h2>
<!-- backwards compatibility -->
<a id="schemabatchregistrationgroupdto"></a>
<a id="schema_BatchRegistrationGroupDto"></a>
<a id="tocSbatchregistrationgroupdto"></a>
<a id="tocsbatchregistrationgroupdto"></a>

```json
{
  "items": [
    {
      "groupId": "string",
      "userId": "string"
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|items|[[BatchRegistrationGroupItemDto](#schemabatchregistrationgroupitemdto)]¦null|false|none|none|

<h2 id="tocS_BatchRegistrationGroupItemDto">BatchRegistrationGroupItemDto</h2>
<!-- backwards compatibility -->
<a id="schemabatchregistrationgroupitemdto"></a>
<a id="schema_BatchRegistrationGroupItemDto"></a>
<a id="tocSbatchregistrationgroupitemdto"></a>
<a id="tocsbatchregistrationgroupitemdto"></a>

```json
{
  "groupId": "string",
  "userId": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|groupId|string¦null|false|none|none|
|userId|string¦null|false|none|none|

<h2 id="tocS_BrandingDeleteDto">BrandingDeleteDto</h2>
<!-- backwards compatibility -->
<a id="schemabrandingdeletedto"></a>
<a id="schema_BrandingDeleteDto"></a>
<a id="tocSbrandingdeletedto"></a>
<a id="tocsbrandingdeletedto"></a>

```json
{
  "logoUrl": true,
  "faviconUrl": true,
  "primaryButtonBackgroundColor": true,
  "primaryButtonTextColor": true,
  "secondaryButtonBackgroundColor": true,
  "secondaryButtonTextColor": true,
  "socialEventImageUrl": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|logoUrl|boolean|false|none|none|
|faviconUrl|boolean|false|none|none|
|primaryButtonBackgroundColor|boolean|false|none|none|
|primaryButtonTextColor|boolean|false|none|none|
|secondaryButtonBackgroundColor|boolean|false|none|none|
|secondaryButtonTextColor|boolean|false|none|none|
|socialEventImageUrl|boolean|false|none|none|

<h2 id="tocS_BrandingUpdateDto">BrandingUpdateDto</h2>
<!-- backwards compatibility -->
<a id="schemabrandingupdatedto"></a>
<a id="schema_BrandingUpdateDto"></a>
<a id="tocSbrandingupdatedto"></a>
<a id="tocsbrandingupdatedto"></a>

```json
{
  "logoUrl": "string",
  "faviconUrl": "string",
  "primaryButtonBackgroundColor": "string",
  "primaryButtonTextColor": "string",
  "secondaryButtonBackgroundColor": "string",
  "secondaryButtonTextColor": "string",
  "socialEventImageUrl": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|logoUrl|string¦null|false|none|none|
|faviconUrl|string¦null|false|none|none|
|primaryButtonBackgroundColor|string¦null|false|none|none|
|primaryButtonTextColor|string¦null|false|none|none|
|secondaryButtonBackgroundColor|string¦null|false|none|none|
|secondaryButtonTextColor|string¦null|false|none|none|
|socialEventImageUrl|string¦null|false|none|none|

<h2 id="tocS_CancelSubscriptionDto">CancelSubscriptionDto</h2>
<!-- backwards compatibility -->
<a id="schemacancelsubscriptiondto"></a>
<a id="schema_CancelSubscriptionDto"></a>
<a id="tocScancelsubscriptiondto"></a>
<a id="tocscancelsubscriptiondto"></a>

```json
{
  "workspaceId": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|workspaceId|string¦null|false|none|none|

<h2 id="tocS_ChangeLogItemDto">ChangeLogItemDto</h2>
<!-- backwards compatibility -->
<a id="schemachangelogitemdto"></a>
<a id="schema_ChangeLogItemDto"></a>
<a id="tocSchangelogitemdto"></a>
<a id="tocschangelogitemdto"></a>

```json
{
  "id": "string",
  "title": "string",
  "description": "string",
  "notificationDate": "2019-08-24T14:15:22Z",
  "createdOn": "2019-08-24T14:15:22Z",
  "updatedOn": "2019-08-24T14:15:22Z"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string¦null|false|none|none|
|title|string¦null|false|none|none|
|description|string¦null|false|none|none|
|notificationDate|string(date-time)|false|none|none|
|createdOn|string(date-time)|false|none|none|
|updatedOn|string(date-time)¦null|false|none|none|

<h2 id="tocS_CreatableDropDownOption">CreatableDropDownOption</h2>
<!-- backwards compatibility -->
<a id="schemacreatabledropdownoption"></a>
<a id="schema_CreatableDropDownOption"></a>
<a id="tocScreatabledropdownoption"></a>
<a id="tocscreatabledropdownoption"></a>

```json
{
  "value": "string",
  "isNew": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|value|string¦null|false|none|none|
|isNew|boolean|false|none|none|

<h2 id="tocS_CreateChatRequest">CreateChatRequest</h2>
<!-- backwards compatibility -->
<a id="schemacreatechatrequest"></a>
<a id="schema_CreateChatRequest"></a>
<a id="tocScreatechatrequest"></a>
<a id="tocscreatechatrequest"></a>

```json
{
  "userId": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|userId|string¦null|false|none|none|

<h2 id="tocS_CreateEventDto">CreateEventDto</h2>
<!-- backwards compatibility -->
<a id="schemacreateeventdto"></a>
<a id="schema_CreateEventDto"></a>
<a id="tocScreateeventdto"></a>
<a id="tocscreateeventdto"></a>

```json
{
  "name": "string",
  "slug": "string",
  "description": "string",
  "venue": "string",
  "isPaymentEnabled": true,
  "price": 0,
  "paymentApiKey": "string",
  "paymentApiSecret": "string",
  "timezone": "string",
  "currency": "string",
  "language": "string",
  "dataControllerName": "string",
  "dataControllerEmail": "user@example.com",
  "dataProcessorName": "string",
  "dataProcessorEmail": "user@example.com",
  "isLiveEventEnabled": true,
  "isRegistrationEnabled": true,
  "isMinglEvent": true,
  "startDate": "2019-08-24T14:15:22Z",
  "endDate": "2019-08-24T14:15:22Z",
  "workspaceId": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|name|string|true|none|none|
|slug|string¦null|false|none|none|
|description|string¦null|false|none|none|
|venue|string¦null|false|none|none|
|isPaymentEnabled|boolean|false|none|none|
|price|number(double)¦null|false|none|none|
|paymentApiKey|string¦null|false|none|none|
|paymentApiSecret|string¦null|false|none|none|
|timezone|string|true|none|none|
|currency|string¦null|false|none|none|
|language|string|true|none|none|
|dataControllerName|string|true|none|none|
|dataControllerEmail|string(email)|true|none|none|
|dataProcessorName|string|true|none|none|
|dataProcessorEmail|string(email)|true|none|none|
|isLiveEventEnabled|boolean¦null|false|none|none|
|isRegistrationEnabled|boolean¦null|false|none|none|
|isMinglEvent|boolean¦null|false|none|none|
|startDate|string(date-time)|true|none|none|
|endDate|string(date-time)¦null|false|none|none|
|workspaceId|string¦null|false|none|none|

<h2 id="tocS_CreatePaymentIntentDto">CreatePaymentIntentDto</h2>
<!-- backwards compatibility -->
<a id="schemacreatepaymentintentdto"></a>
<a id="schema_CreatePaymentIntentDto"></a>
<a id="tocScreatepaymentintentdto"></a>
<a id="tocscreatepaymentintentdto"></a>

```json
{
  "eventId": "string",
  "formFields": {
    "property1": "string",
    "property2": "string"
  },
  "price": 0,
  "registrationAccessKey": "string",
  "reservations": [
    {
      "id": "string",
      "entityId": "string",
      "token": "string",
      "contextId": "string",
      "isUsed": true
    }
  ],
  "language": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|eventId|string¦null|false|none|none|
|formFields|object¦null|false|none|none|
|» **additionalProperties**|string|false|none|none|
|price|number(double)¦null|false|none|none|
|registrationAccessKey|string¦null|false|none|none|
|reservations|[[ReservedItemDto](#schemareserveditemdto)]¦null|false|none|none|
|language|string¦null|false|none|none|

<h2 id="tocS_CreateRegistrationDto">CreateRegistrationDto</h2>
<!-- backwards compatibility -->
<a id="schemacreateregistrationdto"></a>
<a id="schema_CreateRegistrationDto"></a>
<a id="tocScreateregistrationdto"></a>
<a id="tocscreateregistrationdto"></a>

```json
{
  "registrationId": "string",
  "eventId": "string",
  "values": {
    "property1": "string",
    "property2": "string"
  },
  "reservations": [
    {
      "id": "string",
      "entityId": "string",
      "token": "string",
      "contextId": "string",
      "isUsed": true
    }
  ],
  "ticket": {
    "url": "string",
    "barcode": "string"
  }
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|registrationId|string¦null|false|none|none|
|eventId|string¦null|false|none|none|
|values|object¦null|false|none|none|
|» **additionalProperties**|string|false|none|none|
|reservations|[[ReservedItemDto](#schemareserveditemdto)]¦null|false|none|none|
|ticket|[TicketDto](#schematicketdto)|false|none|none|

<h2 id="tocS_DeclineRegistrationDto">DeclineRegistrationDto</h2>
<!-- backwards compatibility -->
<a id="schemadeclineregistrationdto"></a>
<a id="schema_DeclineRegistrationDto"></a>
<a id="tocSdeclineregistrationdto"></a>
<a id="tocsdeclineregistrationdto"></a>

```json
{
  "eventId": "string",
  "registrationAccessKey": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|eventId|string¦null|false|none|none|
|registrationAccessKey|string¦null|false|none|none|

<h2 id="tocS_DeletePartnerWorkspaceUserDto">DeletePartnerWorkspaceUserDto</h2>
<!-- backwards compatibility -->
<a id="schemadeletepartnerworkspaceuserdto"></a>
<a id="schema_DeletePartnerWorkspaceUserDto"></a>
<a id="tocSdeletepartnerworkspaceuserdto"></a>
<a id="tocsdeletepartnerworkspaceuserdto"></a>

```json
{
  "partnerId": "string",
  "email": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|partnerId|string¦null|false|none|none|
|email|string¦null|false|none|none|

<h2 id="tocS_DeleteTimelineEntryRequest">DeleteTimelineEntryRequest</h2>
<!-- backwards compatibility -->
<a id="schemadeletetimelineentryrequest"></a>
<a id="schema_DeleteTimelineEntryRequest"></a>
<a id="tocSdeletetimelineentryrequest"></a>
<a id="tocsdeletetimelineentryrequest"></a>

```json
{
  "entryId": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|entryId|string¦null|false|none|none|

<h2 id="tocS_DeleteWorkspaceUserDto">DeleteWorkspaceUserDto</h2>
<!-- backwards compatibility -->
<a id="schemadeleteworkspaceuserdto"></a>
<a id="schema_DeleteWorkspaceUserDto"></a>
<a id="tocSdeleteworkspaceuserdto"></a>
<a id="tocsdeleteworkspaceuserdto"></a>

```json
{
  "workspaceId": "string",
  "email": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|workspaceId|string¦null|false|none|none|
|email|string¦null|false|none|none|

<h2 id="tocS_DestinationDto">DestinationDto</h2>
<!-- backwards compatibility -->
<a id="schemadestinationdto"></a>
<a id="schema_DestinationDto"></a>
<a id="tocSdestinationdto"></a>
<a id="tocsdestinationdto"></a>

```json
{
  "registrationId": "string",
  "phoneNumber": "string",
  "text": "string",
  "messageId": "string",
  "error": {
    "errorName": "string",
    "errorDescription": "string"
  }
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|registrationId|string¦null|false|none|none|
|phoneNumber|string¦null|false|none|none|
|text|string¦null|false|none|none|
|messageId|string¦null|false|none|none|
|error|[SmsAuditErrorDto](#schemasmsauditerrordto)|false|none|none|

<h2 id="tocS_ElementType">ElementType</h2>
<!-- backwards compatibility -->
<a id="schemaelementtype"></a>
<a id="schema_ElementType"></a>
<a id="tocSelementtype"></a>
<a id="tocselementtype"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|0|
|*anonymous*|1|
|*anonymous*|2|
|*anonymous*|3|
|*anonymous*|4|
|*anonymous*|5|
|*anonymous*|6|
|*anonymous*|7|
|*anonymous*|8|
|*anonymous*|9|
|*anonymous*|10|
|*anonymous*|99|
|*anonymous*|100|

<h2 id="tocS_ElementUpdateDto">ElementUpdateDto</h2>
<!-- backwards compatibility -->
<a id="schemaelementupdatedto"></a>
<a id="schema_ElementUpdateDto"></a>
<a id="tocSelementupdatedto"></a>
<a id="tocselementupdatedto"></a>

```json
{
  "id": "string",
  "type": 0,
  "options": null,
  "logic": {
    "isEnabled": true,
    "components": [
      {
        "id": "string",
        "action": 0,
        "fieldId": "string",
        "operator": 0,
        "value": "string"
      }
    ]
  },
  "mandatory": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string¦null|false|none|none|
|type|[ElementType](#schemaelementtype)|false|none|none|
|options|any|true|none|none|
|logic|[LogicDto](#schemalogicdto)|false|none|none|
|mandatory|boolean|false|none|none|

<h2 id="tocS_EmailDestinationDto">EmailDestinationDto</h2>
<!-- backwards compatibility -->
<a id="schemaemaildestinationdto"></a>
<a id="schema_EmailDestinationDto"></a>
<a id="tocSemaildestinationdto"></a>
<a id="tocsemaildestinationdto"></a>

```json
{
  "registrationId": "string",
  "email": "string",
  "replacementData": {
    "property1": null,
    "property2": null
  }
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|registrationId|string¦null|false|none|none|
|email|string¦null|false|none|none|
|replacementData|object¦null|false|none|none|
|» **additionalProperties**|any|false|none|none|

<h2 id="tocS_Error">Error</h2>
<!-- backwards compatibility -->
<a id="schemaerror"></a>
<a id="schema_Error"></a>
<a id="tocSerror"></a>
<a id="tocserror"></a>

```json
{
  "groupId": 0,
  "groupName": "string",
  "id": 0,
  "name": "string",
  "description": "string",
  "permanent": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|groupId|integer(int32)¦null|false|none|none|
|groupName|string¦null|false|none|none|
|id|integer(int32)¦null|false|none|none|
|name|string¦null|false|none|none|
|description|string¦null|false|none|none|
|permanent|boolean¦null|false|none|none|

<h2 id="tocS_ErrorDto">ErrorDto</h2>
<!-- backwards compatibility -->
<a id="schemaerrordto"></a>
<a id="schema_ErrorDto"></a>
<a id="tocSerrordto"></a>
<a id="tocserrordto"></a>

```json
{
  "text": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|text|string¦null|false|none|none|

<h2 id="tocS_EventFeatureDtoBase">EventFeatureDtoBase</h2>
<!-- backwards compatibility -->
<a id="schemaeventfeaturedtobase"></a>
<a id="schema_EventFeatureDtoBase"></a>
<a id="tocSeventfeaturedtobase"></a>
<a id="tocseventfeaturedtobase"></a>

```json
{
  "type": 0,
  "typeString": 0,
  "completedOn": "2019-08-24T14:15:22Z",
  "disabledOn": "2019-08-24T14:15:22Z",
  "order": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|type|[EventFeatureType](#schemaeventfeaturetype)|false|none|none|
|typeString|[EventFeatureType](#schemaeventfeaturetype)|false|none|none|
|completedOn|string(date-time)¦null|false|none|none|
|disabledOn|string(date-time)¦null|false|none|none|
|order|integer(int32)|false|none|none|

<h2 id="tocS_EventFeatureType">EventFeatureType</h2>
<!-- backwards compatibility -->
<a id="schemaeventfeaturetype"></a>
<a id="schema_EventFeatureType"></a>
<a id="tocSeventfeaturetype"></a>
<a id="tocseventfeaturetype"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|0|
|*anonymous*|100|
|*anonymous*|200|
|*anonymous*|210|
|*anonymous*|220|
|*anonymous*|230|
|*anonymous*|300|
|*anonymous*|400|
|*anonymous*|500|
|*anonymous*|600|
|*anonymous*|700|
|*anonymous*|800|
|*anonymous*|900|
|*anonymous*|1000|
|*anonymous*|1100|
|*anonymous*|1300|
|*anonymous*|1400|
|*anonymous*|1500|
|*anonymous*|1600|

<h2 id="tocS_EventFormMetadataDto">EventFormMetadataDto</h2>
<!-- backwards compatibility -->
<a id="schemaeventformmetadatadto"></a>
<a id="schema_EventFormMetadataDto"></a>
<a id="tocSeventformmetadatadto"></a>
<a id="tocseventformmetadatadto"></a>

```json
{
  "registrationStartDate": "2019-08-24T14:15:22Z",
  "registrationEndDate": "2019-08-24T14:15:22Z",
  "attendeeLimit": 0,
  "isDirty": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|registrationStartDate|string(date-time)¦null|false|none|none|
|registrationEndDate|string(date-time)¦null|false|none|none|
|attendeeLimit|integer(int32)|false|none|none|
|isDirty|boolean|false|none|none|

<h2 id="tocS_EventFormUpdateDto">EventFormUpdateDto</h2>
<!-- backwards compatibility -->
<a id="schemaeventformupdatedto"></a>
<a id="schema_EventFormUpdateDto"></a>
<a id="tocSeventformupdatedto"></a>
<a id="tocseventformupdatedto"></a>

```json
{
  "eventId": "string",
  "elements": [
    {
      "id": "string",
      "type": 0,
      "options": null,
      "logic": {
        "isEnabled": true,
        "components": [
          {
            "id": "string",
            "action": 0,
            "fieldId": "string",
            "operator": 0,
            "value": "string"
          }
        ]
      },
      "mandatory": true
    }
  ],
  "formMetadata": {
    "registrationStartDate": "2019-08-24T14:15:22Z",
    "registrationEndDate": "2019-08-24T14:15:22Z",
    "attendeeLimit": 0,
    "isDirty": true
  },
  "isDirty": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|eventId|string|true|none|none|
|elements|[[ElementUpdateDto](#schemaelementupdatedto)]|true|none|none|
|formMetadata|[EventFormMetadataDto](#schemaeventformmetadatadto)|false|none|none|
|isDirty|boolean|false|none|none|

<h2 id="tocS_EventLandingPageUpdateDto">EventLandingPageUpdateDto</h2>
<!-- backwards compatibility -->
<a id="schemaeventlandingpageupdatedto"></a>
<a id="schema_EventLandingPageUpdateDto"></a>
<a id="tocSeventlandingpageupdatedto"></a>
<a id="tocseventlandingpageupdatedto"></a>

```json
{
  "eventId": "string",
  "widgets": [
    {
      "id": "string",
      "type": 1,
      "options": null,
      "mandatory": true
    }
  ],
  "branding": {
    "showHeader": true,
    "headerBackgroundColor": "string",
    "headerBackgroundUrl": "string",
    "headerTextColor": "string",
    "headerHeight": 0,
    "headerSpacing": 0,
    "headerTitleSize": 0,
    "transparentHeader": true,
    "faviconUrl": "string",
    "backgroundColor": "string",
    "backgroundImageUrl": "string",
    "backgroundRepeat": "string",
    "backgroundPosition": "string",
    "fixedBackground": true
  },
  "templates": {
    "successfulRegistrationHtmlTemplate": "string",
    "isDirty": true
  },
  "isPreview": true,
  "isDirty": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|eventId|string|true|none|none|
|widgets|[[WidgetUpdateDto](#schemawidgetupdatedto)]|true|none|none|
|branding|[LandingPageBrandingDto](#schemalandingpagebrandingdto)|false|none|none|
|templates|[EventTemplateUpdateDto](#schemaeventtemplateupdatedto)|false|none|none|
|isPreview|boolean|false|none|none|
|isDirty|boolean|false|none|none|

<h2 id="tocS_EventLinkDto">EventLinkDto</h2>
<!-- backwards compatibility -->
<a id="schemaeventlinkdto"></a>
<a id="schema_EventLinkDto"></a>
<a id="tocSeventlinkdto"></a>
<a id="tocseventlinkdto"></a>

```json
{
  "destination": 0,
  "eventId": "string",
  "externalEventId": "string",
  "externalEventName": "string",
  "isUnlink": true,
  "message": "string",
  "stackTraceLines": [
    "string"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|destination|[IntegrationDestination](#schemaintegrationdestination)|false|none|none|
|eventId|string¦null|false|none|none|
|externalEventId|string¦null|false|none|none|
|externalEventName|string¦null|false|none|none|
|isUnlink|boolean|false|none|none|
|message|string¦null|false|none|none|
|stackTraceLines|[string]¦null|false|none|none|

<h2 id="tocS_EventLobbyPageUpdateDto">EventLobbyPageUpdateDto</h2>
<!-- backwards compatibility -->
<a id="schemaeventlobbypageupdatedto"></a>
<a id="schema_EventLobbyPageUpdateDto"></a>
<a id="tocSeventlobbypageupdatedto"></a>
<a id="tocseventlobbypageupdatedto"></a>

```json
{
  "eventId": "string",
  "elements": [
    {
      "id": "string",
      "category": 1,
      "type": 0,
      "options": null,
      "mandatory": true
    }
  ],
  "branding": {
    "backgroundColor": "string",
    "textColor": "string",
    "navigationBackgroundColor": "string",
    "primaryBackgroundColor": "string",
    "primaryTextColor": "string",
    "secondaryBackgroundColor": "string",
    "secondaryTextColor": "string"
  },
  "isPreview": true,
  "isDirty": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|eventId|string|true|none|none|
|elements|[[PageElementUpdateDto](#schemapageelementupdatedto)]|true|none|none|
|branding|[LobbyPageBrandingDto](#schemalobbypagebrandingdto)|false|none|none|
|isPreview|boolean|false|none|none|
|isDirty|boolean|false|none|none|

<h2 id="tocS_EventTemplatePageUpdateDto">EventTemplatePageUpdateDto</h2>
<!-- backwards compatibility -->
<a id="schemaeventtemplatepageupdatedto"></a>
<a id="schema_EventTemplatePageUpdateDto"></a>
<a id="tocSeventtemplatepageupdatedto"></a>
<a id="tocseventtemplatepageupdatedto"></a>

```json
{
  "successfulRegistrationHtmlTemplate": "string",
  "isDirty": true,
  "eventId": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|successfulRegistrationHtmlTemplate|string¦null|false|none|none|
|isDirty|boolean|false|none|none|
|eventId|string|true|none|none|

<h2 id="tocS_EventTemplateUpdateDto">EventTemplateUpdateDto</h2>
<!-- backwards compatibility -->
<a id="schemaeventtemplateupdatedto"></a>
<a id="schema_EventTemplateUpdateDto"></a>
<a id="tocSeventtemplateupdatedto"></a>
<a id="tocseventtemplateupdatedto"></a>

```json
{
  "successfulRegistrationHtmlTemplate": "string",
  "isDirty": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|successfulRegistrationHtmlTemplate|string¦null|false|none|none|
|isDirty|boolean|false|none|none|

<h2 id="tocS_ExportParticipantsRequest">ExportParticipantsRequest</h2>
<!-- backwards compatibility -->
<a id="schemaexportparticipantsrequest"></a>
<a id="schema_ExportParticipantsRequest"></a>
<a id="tocSexportparticipantsrequest"></a>
<a id="tocsexportparticipantsrequest"></a>

```json
{
  "selectedRows": [
    "string"
  ],
  "selectedColumns": [
    "string"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|selectedRows|[string]¦null|false|none|none|
|selectedColumns|[string]¦null|false|none|none|

<h2 id="tocS_GroupSubType">GroupSubType</h2>
<!-- backwards compatibility -->
<a id="schemagroupsubtype"></a>
<a id="schema_GroupSubType"></a>
<a id="tocSgroupsubtype"></a>
<a id="tocsgroupsubtype"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|0|
|*anonymous*|1|

<h2 id="tocS_GroupType">GroupType</h2>
<!-- backwards compatibility -->
<a id="schemagrouptype"></a>
<a id="schema_GroupType"></a>
<a id="tocSgrouptype"></a>
<a id="tocsgrouptype"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|0|
|*anonymous*|1|

<h2 id="tocS_HelpTextRequest">HelpTextRequest</h2>
<!-- backwards compatibility -->
<a id="schemahelptextrequest"></a>
<a id="schema_HelpTextRequest"></a>
<a id="tocShelptextrequest"></a>
<a id="tocshelptextrequest"></a>

```json
{
  "content": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|content|string¦null|false|none|none|

<h2 id="tocS_HelpTextType">HelpTextType</h2>
<!-- backwards compatibility -->
<a id="schemahelptexttype"></a>
<a id="schema_HelpTextType"></a>
<a id="tocShelptexttype"></a>
<a id="tocshelptexttype"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|0|
|*anonymous*|1|

<h2 id="tocS_InfoPageDto">InfoPageDto</h2>
<!-- backwards compatibility -->
<a id="schemainfopagedto"></a>
<a id="schema_InfoPageDto"></a>
<a id="tocSinfopagedto"></a>
<a id="tocsinfopagedto"></a>

```json
{
  "id": "string",
  "title": "string",
  "content": "string",
  "order": 0,
  "groupIds": [
    "string"
  ],
  "platformPages": [
    0
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string¦null|false|none|none|
|title|string¦null|false|none|none|
|content|string¦null|false|none|none|
|order|integer(int32)¦null|false|none|none|
|groupIds|[string]¦null|false|none|none|
|platformPages|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|

<h2 id="tocS_IntegrationDestination">IntegrationDestination</h2>
<!-- backwards compatibility -->
<a id="schemaintegrationdestination"></a>
<a id="schema_IntegrationDestination"></a>
<a id="tocSintegrationdestination"></a>
<a id="tocsintegrationdestination"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|0|
|*anonymous*|1|

<h2 id="tocS_InvoiceStatusDto">InvoiceStatusDto</h2>
<!-- backwards compatibility -->
<a id="schemainvoicestatusdto"></a>
<a id="schema_InvoiceStatusDto"></a>
<a id="tocSinvoicestatusdto"></a>
<a id="tocsinvoicestatusdto"></a>

```json
{
  "workspaceId": "string",
  "invoiceId": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|workspaceId|string¦null|false|none|none|
|invoiceId|string¦null|false|none|none|

<h2 id="tocS_IValueConverter">IValueConverter</h2>
<!-- backwards compatibility -->
<a id="schemaivalueconverter"></a>
<a id="schema_IValueConverter"></a>
<a id="tocSivalueconverter"></a>
<a id="tocsivalueconverter"></a>

```json
{}

```

### Properties

*None*

<h2 id="tocS_JToken">JToken</h2>
<!-- backwards compatibility -->
<a id="schemajtoken"></a>
<a id="schema_JToken"></a>
<a id="tocSjtoken"></a>
<a id="tocsjtoken"></a>

```json
[
  [
    []
  ]
]

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|[[JToken](#schemajtoken)]|false|none|none|

<h2 id="tocS_LandingPageBrandingDto">LandingPageBrandingDto</h2>
<!-- backwards compatibility -->
<a id="schemalandingpagebrandingdto"></a>
<a id="schema_LandingPageBrandingDto"></a>
<a id="tocSlandingpagebrandingdto"></a>
<a id="tocslandingpagebrandingdto"></a>

```json
{
  "showHeader": true,
  "headerBackgroundColor": "string",
  "headerBackgroundUrl": "string",
  "headerTextColor": "string",
  "headerHeight": 0,
  "headerSpacing": 0,
  "headerTitleSize": 0,
  "transparentHeader": true,
  "faviconUrl": "string",
  "backgroundColor": "string",
  "backgroundImageUrl": "string",
  "backgroundRepeat": "string",
  "backgroundPosition": "string",
  "fixedBackground": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|showHeader|boolean|false|none|none|
|headerBackgroundColor|string¦null|false|none|none|
|headerBackgroundUrl|string¦null|false|none|none|
|headerTextColor|string¦null|false|none|none|
|headerHeight|integer(int32)|false|none|none|
|headerSpacing|integer(int32)|false|none|none|
|headerTitleSize|integer(int32)|false|none|none|
|transparentHeader|boolean|false|none|none|
|faviconUrl|string¦null|false|none|none|
|backgroundColor|string¦null|false|none|none|
|backgroundImageUrl|string¦null|false|none|none|
|backgroundRepeat|string¦null|false|none|none|
|backgroundPosition|string¦null|false|none|none|
|fixedBackground|boolean|false|none|none|

<h2 id="tocS_LikeTimelineEntryRequest">LikeTimelineEntryRequest</h2>
<!-- backwards compatibility -->
<a id="schemaliketimelineentryrequest"></a>
<a id="schema_LikeTimelineEntryRequest"></a>
<a id="tocSliketimelineentryrequest"></a>
<a id="tocsliketimelineentryrequest"></a>

```json
{
  "entryId": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|entryId|string¦null|false|none|none|

<h2 id="tocS_LiveEventSettingsUpdateDto">LiveEventSettingsUpdateDto</h2>
<!-- backwards compatibility -->
<a id="schemaliveeventsettingsupdatedto"></a>
<a id="schema_LiveEventSettingsUpdateDto"></a>
<a id="tocSliveeventsettingsupdatedto"></a>
<a id="tocsliveeventsettingsupdatedto"></a>

```json
{
  "stageStream": {
    "type": 0,
    "url": "string",
    "settings": {
      "host": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      },
      "stream": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      }
    }
  },
  "isRegisterEnabled": true,
  "isLoginEnabled": true,
  "loginCaption": "string",
  "loginDisabledFrom": "2019-08-24T14:15:22Z",
  "loginDisabledTo": "2019-08-24T14:15:22Z",
  "isGamificationEnabled": true,
  "gamificationUrl": "string",
  "platformPages": [
    0
  ],
  "newsFeed": [
    0
  ],
  "newsFeedPosts": [
    0
  ],
  "newsFeedComments": [
    0
  ],
  "infoPages": [
    0
  ],
  "userSettings": [
    0
  ],
  "documents": [
    0
  ],
  "sponsors": [
    0
  ],
  "chat": [
    0
  ],
  "speakers": [
    0
  ],
  "agenda": [
    0
  ],
  "support": [
    0
  ],
  "participants": [
    0
  ],
  "isParticipantEmailEnabled": true,
  "isParticipantPhoneEnabled": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|stageStream|[StageStreamPatchDto](#schemastagestreampatchdto)|false|none|none|
|isRegisterEnabled|boolean¦null|false|none|none|
|isLoginEnabled|boolean¦null|false|none|none|
|loginCaption|string¦null|false|none|none|
|loginDisabledFrom|string(date-time)¦null|false|none|none|
|loginDisabledTo|string(date-time)¦null|false|none|none|
|isGamificationEnabled|boolean¦null|false|none|none|
|gamificationUrl|string¦null|false|none|none|
|platformPages|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|
|newsFeed|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|
|newsFeedPosts|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|
|newsFeedComments|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|
|infoPages|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|
|userSettings|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|
|documents|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|
|sponsors|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|
|chat|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|
|speakers|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|
|agenda|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|
|support|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|
|participants|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|
|isParticipantEmailEnabled|boolean¦null|false|none|none|
|isParticipantPhoneEnabled|boolean¦null|false|none|none|

<h2 id="tocS_LobbyPageBrandingDto">LobbyPageBrandingDto</h2>
<!-- backwards compatibility -->
<a id="schemalobbypagebrandingdto"></a>
<a id="schema_LobbyPageBrandingDto"></a>
<a id="tocSlobbypagebrandingdto"></a>
<a id="tocslobbypagebrandingdto"></a>

```json
{
  "backgroundColor": "string",
  "textColor": "string",
  "navigationBackgroundColor": "string",
  "primaryBackgroundColor": "string",
  "primaryTextColor": "string",
  "secondaryBackgroundColor": "string",
  "secondaryTextColor": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|backgroundColor|string¦null|false|none|none|
|textColor|string¦null|false|none|none|
|navigationBackgroundColor|string¦null|false|none|none|
|primaryBackgroundColor|string¦null|false|none|none|
|primaryTextColor|string¦null|false|none|none|
|secondaryBackgroundColor|string¦null|false|none|none|
|secondaryTextColor|string¦null|false|none|none|

<h2 id="tocS_LogicAction">LogicAction</h2>
<!-- backwards compatibility -->
<a id="schemalogicaction"></a>
<a id="schema_LogicAction"></a>
<a id="tocSlogicaction"></a>
<a id="tocslogicaction"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|0|
|*anonymous*|1|

<h2 id="tocS_LogicComponentDto">LogicComponentDto</h2>
<!-- backwards compatibility -->
<a id="schemalogiccomponentdto"></a>
<a id="schema_LogicComponentDto"></a>
<a id="tocSlogiccomponentdto"></a>
<a id="tocslogiccomponentdto"></a>

```json
{
  "id": "string",
  "action": 0,
  "fieldId": "string",
  "operator": 0,
  "value": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string¦null|false|none|none|
|action|[LogicAction](#schemalogicaction)|false|none|none|
|fieldId|string¦null|false|none|none|
|operator|[LogicOperator](#schemalogicoperator)|false|none|none|
|value|string¦null|false|none|none|

<h2 id="tocS_LogicDto">LogicDto</h2>
<!-- backwards compatibility -->
<a id="schemalogicdto"></a>
<a id="schema_LogicDto"></a>
<a id="tocSlogicdto"></a>
<a id="tocslogicdto"></a>

```json
{
  "isEnabled": true,
  "components": [
    {
      "id": "string",
      "action": 0,
      "fieldId": "string",
      "operator": 0,
      "value": "string"
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|isEnabled|boolean|false|none|none|
|components|[[LogicComponentDto](#schemalogiccomponentdto)]¦null|false|none|none|

<h2 id="tocS_LogicOperator">LogicOperator</h2>
<!-- backwards compatibility -->
<a id="schemalogicoperator"></a>
<a id="schema_LogicOperator"></a>
<a id="tocSlogicoperator"></a>
<a id="tocslogicoperator"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|0|
|*anonymous*|1|
|*anonymous*|2|

<h2 id="tocS_LoginUserDto">LoginUserDto</h2>
<!-- backwards compatibility -->
<a id="schemaloginuserdto"></a>
<a id="schema_LoginUserDto"></a>
<a id="tocSloginuserdto"></a>
<a id="tocsloginuserdto"></a>

```json
{
  "userName": "string",
  "password": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|userName|string¦null|false|none|none|
|password|string¦null|false|none|none|

<h2 id="tocS_PageElementCategory">PageElementCategory</h2>
<!-- backwards compatibility -->
<a id="schemapageelementcategory"></a>
<a id="schema_PageElementCategory"></a>
<a id="tocSpageelementcategory"></a>
<a id="tocspageelementcategory"></a>

```json
1

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|1|
|*anonymous*|2|

<h2 id="tocS_PageElementUpdateDto">PageElementUpdateDto</h2>
<!-- backwards compatibility -->
<a id="schemapageelementupdatedto"></a>
<a id="schema_PageElementUpdateDto"></a>
<a id="tocSpageelementupdatedto"></a>
<a id="tocspageelementupdatedto"></a>

```json
{
  "id": "string",
  "category": 1,
  "type": 0,
  "options": null,
  "mandatory": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string¦null|false|none|none|
|category|[PageElementCategory](#schemapageelementcategory)|false|none|none|
|type|integer(int32)|false|none|none|
|options|any|true|none|none|
|mandatory|boolean|false|none|none|

<h2 id="tocS_PartialInfoPageDto">PartialInfoPageDto</h2>
<!-- backwards compatibility -->
<a id="schemapartialinfopagedto"></a>
<a id="schema_PartialInfoPageDto"></a>
<a id="tocSpartialinfopagedto"></a>
<a id="tocspartialinfopagedto"></a>

```json
{
  "title": "string",
  "content": "string",
  "order": 0,
  "groupIds": [
    "string"
  ],
  "platformPages": [
    0
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|title|string¦null|false|none|none|
|content|string¦null|false|none|none|
|order|integer(int32)¦null|false|none|none|
|groupIds|[string]¦null|false|none|none|
|platformPages|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|

<h2 id="tocS_PartialLiveDocumentDto">PartialLiveDocumentDto</h2>
<!-- backwards compatibility -->
<a id="schemapartiallivedocumentdto"></a>
<a id="schema_PartialLiveDocumentDto"></a>
<a id="tocSpartiallivedocumentdto"></a>
<a id="tocspartiallivedocumentdto"></a>

```json
{
  "title": "string",
  "description": "string",
  "documentUrl": "string",
  "isHidden": true,
  "order": 0,
  "groupIds": [
    "string"
  ],
  "platformPages": [
    0
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|title|string¦null|false|none|none|
|description|string¦null|false|none|none|
|documentUrl|string¦null|false|none|none|
|isHidden|boolean¦null|false|none|none|
|order|integer(int32)¦null|false|none|none|
|groupIds|[string]¦null|false|none|none|
|platformPages|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|

<h2 id="tocS_PartialPollDto">PartialPollDto</h2>
<!-- backwards compatibility -->
<a id="schemapartialpolldto"></a>
<a id="schema_PartialPollDto"></a>
<a id="tocSpartialpolldto"></a>
<a id="tocspartialpolldto"></a>

```json
{}

```

### Properties

*None*

<h2 id="tocS_PartialPromotedMessageDto">PartialPromotedMessageDto</h2>
<!-- backwards compatibility -->
<a id="schemapartialpromotedmessagedto"></a>
<a id="schema_PartialPromotedMessageDto"></a>
<a id="tocSpartialpromotedmessagedto"></a>
<a id="tocspartialpromotedmessagedto"></a>

```json
{
  "fromDate": "2019-08-24T14:15:22Z",
  "toDate": "2019-08-24T14:15:22Z",
  "message": "string",
  "isHidden": true,
  "isVisibleOnTop": true,
  "groupIds": [
    "string"
  ],
  "platformPages": [
    0
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|fromDate|string(date-time)¦null|false|none|none|
|toDate|string(date-time)¦null|false|none|none|
|message|string¦null|false|none|none|
|isHidden|boolean¦null|false|none|none|
|isVisibleOnTop|boolean¦null|false|none|none|
|groupIds|[string]¦null|false|none|none|
|platformPages|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|

<h2 id="tocS_PartialRegistrationGroupDto">PartialRegistrationGroupDto</h2>
<!-- backwards compatibility -->
<a id="schemapartialregistrationgroupdto"></a>
<a id="schema_PartialRegistrationGroupDto"></a>
<a id="tocSpartialregistrationgroupdto"></a>
<a id="tocspartialregistrationgroupdto"></a>

```json
{
  "name": "string",
  "userIds": [
    "string"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|name|string¦null|false|none|none|
|userIds|[string]¦null|false|none|none|

<h2 id="tocS_PartialSpeakerDto">PartialSpeakerDto</h2>
<!-- backwards compatibility -->
<a id="schemapartialspeakerdto"></a>
<a id="schema_PartialSpeakerDto"></a>
<a id="tocSpartialspeakerdto"></a>
<a id="tocspartialspeakerdto"></a>

```json
{}

```

### Properties

*None*

<h2 id="tocS_PartialSponsorDto">PartialSponsorDto</h2>
<!-- backwards compatibility -->
<a id="schemapartialsponsordto"></a>
<a id="schema_PartialSponsorDto"></a>
<a id="tocSpartialsponsordto"></a>
<a id="tocspartialsponsordto"></a>

```json
{
  "name": "string",
  "logoUrl": "string",
  "description": "string",
  "email": "string",
  "phoneNumber": "string",
  "website": "string",
  "address": "string",
  "links": [
    {
      "url": "string"
    }
  ],
  "order": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|name|string¦null|false|none|none|
|logoUrl|string¦null|false|none|none|
|description|string¦null|false|none|none|
|email|string¦null|false|none|none|
|phoneNumber|string¦null|false|none|none|
|website|string¦null|false|none|none|
|address|string¦null|false|none|none|
|links|[[SocialLinkDto](#schemasociallinkdto)]¦null|false|none|none|
|order|integer(int32)|false|none|none|

<h2 id="tocS_PlatformPage">PlatformPage</h2>
<!-- backwards compatibility -->
<a id="schemaplatformpage"></a>
<a id="schema_PlatformPage"></a>
<a id="tocSplatformpage"></a>
<a id="tocsplatformpage"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|0|
|*anonymous*|1|
|*anonymous*|2|

<h2 id="tocS_PollDto">PollDto</h2>
<!-- backwards compatibility -->
<a id="schemapolldto"></a>
<a id="schema_PollDto"></a>
<a id="tocSpolldto"></a>
<a id="tocspolldto"></a>

```json
{
  "id": "string",
  "title": "string",
  "description": "string",
  "isPublicResults": true,
  "order": 0,
  "pollType": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string¦null|false|none|none|
|title|string¦null|false|none|none|
|description|string¦null|false|none|none|
|isPublicResults|boolean¦null|false|none|none|
|order|integer(int32)¦null|false|none|none|
|pollType|[PollType](#schemapolltype)|false|none|none|

<h2 id="tocS_PollType">PollType</h2>
<!-- backwards compatibility -->
<a id="schemapolltype"></a>
<a id="schema_PollType"></a>
<a id="tocSpolltype"></a>
<a id="tocspolltype"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|0|
|*anonymous*|1|
|*anonymous*|2|

<h2 id="tocS_PortalCheckoutRequest">PortalCheckoutRequest</h2>
<!-- backwards compatibility -->
<a id="schemaportalcheckoutrequest"></a>
<a id="schema_PortalCheckoutRequest"></a>
<a id="tocSportalcheckoutrequest"></a>
<a id="tocsportalcheckoutrequest"></a>

```json
{
  "addressLine1": "string",
  "addressLine2": "string",
  "zipCode": "string",
  "state": "string",
  "stateCode": "string",
  "country": "string",
  "city": "string",
  "firstName": "string",
  "lastName": "string",
  "company": "string",
  "planPriceId": "string",
  "workspaceId": "string",
  "paymentIntentId": "string",
  "companyName": "string",
  "cardHolderFirstName": "string",
  "cardHolderLastName": "string",
  "vatId": "string",
  "invoiceEmail": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|addressLine1|string¦null|false|none|none|
|addressLine2|string¦null|false|none|none|
|zipCode|string¦null|false|none|none|
|state|string¦null|false|none|none|
|stateCode|string¦null|false|none|none|
|country|string¦null|false|none|none|
|city|string¦null|false|none|none|
|firstName|string¦null|false|none|none|
|lastName|string¦null|false|none|none|
|company|string¦null|false|none|none|
|planPriceId|string¦null|false|none|none|
|workspaceId|string¦null|false|none|none|
|paymentIntentId|string¦null|false|none|none|
|companyName|string¦null|false|none|none|
|cardHolderFirstName|string¦null|false|none|none|
|cardHolderLastName|string¦null|false|none|none|
|vatId|string¦null|false|none|none|
|invoiceEmail|string¦null|false|none|none|

<h2 id="tocS_PortalConfirmPaymentIntentRequest">PortalConfirmPaymentIntentRequest</h2>
<!-- backwards compatibility -->
<a id="schemaportalconfirmpaymentintentrequest"></a>
<a id="schema_PortalConfirmPaymentIntentRequest"></a>
<a id="tocSportalconfirmpaymentintentrequest"></a>
<a id="tocsportalconfirmpaymentintentrequest"></a>

```json
{
  "paymentIntentId": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|paymentIntentId|string¦null|false|none|none|

<h2 id="tocS_PortalCreatePaymentIntentRequest">PortalCreatePaymentIntentRequest</h2>
<!-- backwards compatibility -->
<a id="schemaportalcreatepaymentintentrequest"></a>
<a id="schema_PortalCreatePaymentIntentRequest"></a>
<a id="tocSportalcreatepaymentintentrequest"></a>
<a id="tocsportalcreatepaymentintentrequest"></a>

```json
{
  "addressLine1": "string",
  "addressLine2": "string",
  "zipCode": "string",
  "state": "string",
  "stateCode": "string",
  "country": "string",
  "city": "string",
  "firstName": "string",
  "lastName": "string",
  "company": "string",
  "paymentMethodId": "string",
  "planName": "string",
  "planPriceId": "string",
  "totalPrice": 0,
  "companyName": "string",
  "invoiceEmail": "string",
  "vatId": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|addressLine1|string¦null|false|none|none|
|addressLine2|string¦null|false|none|none|
|zipCode|string¦null|false|none|none|
|state|string¦null|false|none|none|
|stateCode|string¦null|false|none|none|
|country|string¦null|false|none|none|
|city|string¦null|false|none|none|
|firstName|string¦null|false|none|none|
|lastName|string¦null|false|none|none|
|company|string¦null|false|none|none|
|paymentMethodId|string¦null|false|none|none|
|planName|string¦null|false|none|none|
|planPriceId|string¦null|false|none|none|
|totalPrice|integer(int32)|false|none|none|
|companyName|string¦null|false|none|none|
|invoiceEmail|string¦null|false|none|none|
|vatId|string¦null|false|none|none|

<h2 id="tocS_PresentType">PresentType</h2>
<!-- backwards compatibility -->
<a id="schemapresenttype"></a>
<a id="schema_PresentType"></a>
<a id="tocSpresenttype"></a>
<a id="tocspresenttype"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|0|
|*anonymous*|1|
|*anonymous*|2|
|*anonymous*|3|

<h2 id="tocS_Price">Price</h2>
<!-- backwards compatibility -->
<a id="schemaprice"></a>
<a id="schema_Price"></a>
<a id="tocSprice"></a>
<a id="tocsprice"></a>

```json
{
  "pricePerMessage": 0,
  "pricePerLookup": 0,
  "currency": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|pricePerMessage|number(double)¦null|false|none|none|
|pricePerLookup|number(double)¦null|false|none|none|
|currency|string¦null|false|none|none|

<h2 id="tocS_PromotedMessageDto">PromotedMessageDto</h2>
<!-- backwards compatibility -->
<a id="schemapromotedmessagedto"></a>
<a id="schema_PromotedMessageDto"></a>
<a id="tocSpromotedmessagedto"></a>
<a id="tocspromotedmessagedto"></a>

```json
{
  "id": "string",
  "fromDate": "2019-08-24T14:15:22Z",
  "toDate": "2019-08-24T14:15:22Z",
  "message": "string",
  "isHidden": true,
  "isVisibleOnTop": true,
  "groupIds": [
    "string"
  ],
  "platformPages": [
    0
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string¦null|false|none|none|
|fromDate|string(date-time)¦null|false|none|none|
|toDate|string(date-time)¦null|false|none|none|
|message|string¦null|false|none|none|
|isHidden|boolean¦null|false|none|none|
|isVisibleOnTop|boolean¦null|false|none|none|
|groupIds|[string]¦null|false|none|none|
|platformPages|[[PlatformPage](#schemaplatformpage)]¦null|false|none|none|

<h2 id="tocS_PublishEventDto">PublishEventDto</h2>
<!-- backwards compatibility -->
<a id="schemapublisheventdto"></a>
<a id="schema_PublishEventDto"></a>
<a id="tocSpublisheventdto"></a>
<a id="tocspublisheventdto"></a>

```json
{
  "eventId": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|eventId|string¦null|false|none|none|

<h2 id="tocS_PurchaseAddonDto">PurchaseAddonDto</h2>
<!-- backwards compatibility -->
<a id="schemapurchaseaddondto"></a>
<a id="schema_PurchaseAddonDto"></a>
<a id="tocSpurchaseaddondto"></a>
<a id="tocspurchaseaddondto"></a>

```json
{
  "workspaceId": "string",
  "addonId": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|workspaceId|string¦null|false|none|none|
|addonId|string¦null|false|none|none|

<h2 id="tocS_RegisterEventDto">RegisterEventDto</h2>
<!-- backwards compatibility -->
<a id="schemaregistereventdto"></a>
<a id="schema_RegisterEventDto"></a>
<a id="tocSregistereventdto"></a>
<a id="tocsregistereventdto"></a>

```json
{
  "eventId": "string",
  "formFields": {
    "property1": "string",
    "property2": "string"
  },
  "paymentIntentId": "string",
  "paymentIntentClientSecret": "string",
  "registrationAccessKey": "string",
  "reservations": [
    {
      "id": "string",
      "entityId": "string",
      "token": "string",
      "contextId": "string",
      "isUsed": true
    }
  ],
  "language": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|eventId|string¦null|false|none|none|
|formFields|object¦null|false|none|none|
|» **additionalProperties**|string|false|none|none|
|paymentIntentId|string¦null|false|none|none|
|paymentIntentClientSecret|string¦null|false|none|none|
|registrationAccessKey|string¦null|false|none|none|
|reservations|[[ReservedItemDto](#schemareserveditemdto)]¦null|false|none|none|
|language|string¦null|false|none|none|

<h2 id="tocS_RegisterUserDto">RegisterUserDto</h2>
<!-- backwards compatibility -->
<a id="schemaregisteruserdto"></a>
<a id="schema_RegisterUserDto"></a>
<a id="tocSregisteruserdto"></a>
<a id="tocsregisteruserdto"></a>

```json
{
  "email": "user@example.com",
  "password": "string",
  "name": "string",
  "lastName": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|email|string(email)|true|none|none|
|password|string|true|none|none|
|name|string|true|none|none|
|lastName|string|true|none|none|

<h2 id="tocS_RegistrationBulkEditDto">RegistrationBulkEditDto</h2>
<!-- backwards compatibility -->
<a id="schemaregistrationbulkeditdto"></a>
<a id="schema_RegistrationBulkEditDto"></a>
<a id="tocSregistrationbulkeditdto"></a>
<a id="tocsregistrationbulkeditdto"></a>

```json
{
  "eventId": "string",
  "registrationIds": [
    "string"
  ],
  "status": 0,
  "clearReservations": true,
  "addToGroups": [
    {
      "value": "string",
      "isNew": true
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|eventId|string¦null|false|none|none|
|registrationIds|[string]¦null|false|none|none|
|status|[RegistrationType](#schemaregistrationtype)|false|none|none|
|clearReservations|boolean|false|none|none|
|addToGroups|[[CreatableDropDownOption](#schemacreatabledropdownoption)]¦null|false|none|none|

<h2 id="tocS_RegistrationDeleteDto">RegistrationDeleteDto</h2>
<!-- backwards compatibility -->
<a id="schemaregistrationdeletedto"></a>
<a id="schema_RegistrationDeleteDto"></a>
<a id="tocSregistrationdeletedto"></a>
<a id="tocsregistrationdeletedto"></a>

```json
{
  "registrationIds": [
    "string"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|registrationIds|[string]¦null|false|none|none|

<h2 id="tocS_RegistrationGroupDto">RegistrationGroupDto</h2>
<!-- backwards compatibility -->
<a id="schemaregistrationgroupdto"></a>
<a id="schema_RegistrationGroupDto"></a>
<a id="tocSregistrationgroupdto"></a>
<a id="tocsregistrationgroupdto"></a>

```json
{
  "id": "string",
  "eventId": "string",
  "type": 0,
  "subType": 0,
  "name": "string",
  "userIds": [
    "string"
  ],
  "elementId": "string",
  "elementLabel": "string",
  "elementChoiceId": "string",
  "elementChoiceLabel": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string¦null|false|none|none|
|eventId|string¦null|false|none|none|
|type|[GroupType](#schemagrouptype)|false|none|none|
|subType|[GroupSubType](#schemagroupsubtype)|false|none|none|
|name|string|true|none|none|
|userIds|[string]¦null|false|none|none|
|elementId|string¦null|false|none|none|
|elementLabel|string¦null|false|none|none|
|elementChoiceId|string¦null|false|none|none|
|elementChoiceLabel|string¦null|false|none|none|

<h2 id="tocS_RegistrationLinkRequest">RegistrationLinkRequest</h2>
<!-- backwards compatibility -->
<a id="schemaregistrationlinkrequest"></a>
<a id="schema_RegistrationLinkRequest"></a>
<a id="tocSregistrationlinkrequest"></a>
<a id="tocsregistrationlinkrequest"></a>

```json
{
  "eventId": "string",
  "registrationId": "string",
  "parentId": "string",
  "userId": "string",
  "isUnlink": true,
  "message": "string",
  "stackTraceLines": [
    "string"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|eventId|string¦null|false|none|none|
|registrationId|string¦null|false|none|none|
|parentId|string¦null|false|none|none|
|userId|string¦null|false|none|none|
|isUnlink|boolean|false|none|none|
|message|string¦null|false|none|none|
|stackTraceLines|[string]¦null|false|none|none|

<h2 id="tocS_RegistrationsLinkDto">RegistrationsLinkDto</h2>
<!-- backwards compatibility -->
<a id="schemaregistrationslinkdto"></a>
<a id="schema_RegistrationsLinkDto"></a>
<a id="tocSregistrationslinkdto"></a>
<a id="tocsregistrationslinkdto"></a>

```json
{
  "eventId": "string",
  "registrationIds": [
    "string"
  ],
  "userId": "string",
  "parentId": "string",
  "isUnlink": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|eventId|string¦null|false|none|none|
|registrationIds|[string]¦null|false|none|none|
|userId|string¦null|false|none|none|
|parentId|string¦null|false|none|none|
|isUnlink|boolean|false|none|none|

<h2 id="tocS_RegistrationType">RegistrationType</h2>
<!-- backwards compatibility -->
<a id="schemaregistrationtype"></a>
<a id="schema_RegistrationType"></a>
<a id="tocSregistrationtype"></a>
<a id="tocsregistrationtype"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|0|
|*anonymous*|1|
|*anonymous*|2|
|*anonymous*|3|
|*anonymous*|4|

<h2 id="tocS_ReleaseReservationsDto">ReleaseReservationsDto</h2>
<!-- backwards compatibility -->
<a id="schemareleasereservationsdto"></a>
<a id="schema_ReleaseReservationsDto"></a>
<a id="tocSreleasereservationsdto"></a>
<a id="tocsreleasereservationsdto"></a>

```json
{
  "eventId": "string",
  "ids": [
    "string"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|eventId|string¦null|false|none|none|
|ids|[string]¦null|false|none|none|

<h2 id="tocS_ReorderInfoPageDto">ReorderInfoPageDto</h2>
<!-- backwards compatibility -->
<a id="schemareorderinfopagedto"></a>
<a id="schema_ReorderInfoPageDto"></a>
<a id="tocSreorderinfopagedto"></a>
<a id="tocsreorderinfopagedto"></a>

```json
{
  "infoPageIds": [
    "string"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|infoPageIds|[string]¦null|false|none|none|

<h2 id="tocS_ReorderLiveDocumentDto">ReorderLiveDocumentDto</h2>
<!-- backwards compatibility -->
<a id="schemareorderlivedocumentdto"></a>
<a id="schema_ReorderLiveDocumentDto"></a>
<a id="tocSreorderlivedocumentdto"></a>
<a id="tocsreorderlivedocumentdto"></a>

```json
{
  "documentIds": [
    "string"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|documentIds|[string]¦null|false|none|none|

<h2 id="tocS_ReorderPollDto">ReorderPollDto</h2>
<!-- backwards compatibility -->
<a id="schemareorderpolldto"></a>
<a id="schema_ReorderPollDto"></a>
<a id="tocSreorderpolldto"></a>
<a id="tocsreorderpolldto"></a>

```json
{
  "pollIds": [
    "string"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|pollIds|[string]¦null|false|none|none|

<h2 id="tocS_ReorderSpeakerDto">ReorderSpeakerDto</h2>
<!-- backwards compatibility -->
<a id="schemareorderspeakerdto"></a>
<a id="schema_ReorderSpeakerDto"></a>
<a id="tocSreorderspeakerdto"></a>
<a id="tocsreorderspeakerdto"></a>

```json
{
  "speakerIds": [
    "string"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|speakerIds|[string]¦null|false|none|none|

<h2 id="tocS_ReorderSponsorDto">ReorderSponsorDto</h2>
<!-- backwards compatibility -->
<a id="schemareordersponsordto"></a>
<a id="schema_ReorderSponsorDto"></a>
<a id="tocSreordersponsordto"></a>
<a id="tocsreordersponsordto"></a>

```json
{
  "sponsorIds": [
    "string"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|sponsorIds|[string]¦null|false|none|none|

<h2 id="tocS_ReorderTemplateDto">ReorderTemplateDto</h2>
<!-- backwards compatibility -->
<a id="schemareordertemplatedto"></a>
<a id="schema_ReorderTemplateDto"></a>
<a id="tocSreordertemplatedto"></a>
<a id="tocsreordertemplatedto"></a>

```json
{
  "templateIds": [
    "string"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|templateIds|[string]¦null|false|none|none|

<h2 id="tocS_ResendEmailDto">ResendEmailDto</h2>
<!-- backwards compatibility -->
<a id="schemaresendemaildto"></a>
<a id="schema_ResendEmailDto"></a>
<a id="tocSresendemaildto"></a>
<a id="tocsresendemaildto"></a>

```json
{
  "username": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|username|string¦null|false|none|none|

<h2 id="tocS_ReservationRequest">ReservationRequest</h2>
<!-- backwards compatibility -->
<a id="schemareservationrequest"></a>
<a id="schema_ReservationRequest"></a>
<a id="tocSreservationrequest"></a>
<a id="tocsreservationrequest"></a>

```json
{
  "topParentReferenceId": "string",
  "contextId": "string",
  "entityId": "string",
  "previousEntityId": "string",
  "language": "string",
  "isRegistrationPage": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|topParentReferenceId|string¦null|false|none|none|
|contextId|string¦null|false|none|none|
|entityId|string¦null|false|none|none|
|previousEntityId|string¦null|false|none|none|
|language|string¦null|false|none|none|
|isRegistrationPage|boolean|false|none|none|

<h2 id="tocS_ReservedItemDto">ReservedItemDto</h2>
<!-- backwards compatibility -->
<a id="schemareserveditemdto"></a>
<a id="schema_ReservedItemDto"></a>
<a id="tocSreserveditemdto"></a>
<a id="tocsreserveditemdto"></a>

```json
{
  "id": "string",
  "entityId": "string",
  "token": "string",
  "contextId": "string",
  "isUsed": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string¦null|false|none|none|
|entityId|string¦null|false|none|none|
|token|string¦null|false|none|none|
|contextId|string¦null|false|none|none|
|isUsed|boolean|false|none|none|

<h2 id="tocS_ResetPasswordDto">ResetPasswordDto</h2>
<!-- backwards compatibility -->
<a id="schemaresetpassworddto"></a>
<a id="schema_ResetPasswordDto"></a>
<a id="tocSresetpassworddto"></a>
<a id="tocsresetpassworddto"></a>

```json
{
  "userId": "string",
  "token": "string",
  "newPassword": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|userId|string¦null|false|none|none|
|token|string¦null|false|none|none|
|newPassword|string¦null|false|none|none|

<h2 id="tocS_SaveGuestDto">SaveGuestDto</h2>
<!-- backwards compatibility -->
<a id="schemasaveguestdto"></a>
<a id="schema_SaveGuestDto"></a>
<a id="tocSsaveguestdto"></a>
<a id="tocssaveguestdto"></a>

```json
{
  "parentRegistrationId": "string",
  "registrationId": "string",
  "values": {
    "property1": "string",
    "property2": "string"
  },
  "eventId": "string",
  "reservations": [
    {
      "id": "string",
      "entityId": "string",
      "token": "string",
      "contextId": "string",
      "isUsed": true
    }
  ],
  "contextId": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|parentRegistrationId|string¦null|false|none|none|
|registrationId|string¦null|false|none|none|
|values|object¦null|false|none|none|
|» **additionalProperties**|string|false|none|none|
|eventId|string¦null|false|none|none|
|reservations|[[ReservedItemDto](#schemareserveditemdto)]¦null|false|none|none|
|contextId|string¦null|false|none|none|

<h2 id="tocS_SavePartnerWorkspaceDto">SavePartnerWorkspaceDto</h2>
<!-- backwards compatibility -->
<a id="schemasavepartnerworkspacedto"></a>
<a id="schema_SavePartnerWorkspaceDto"></a>
<a id="tocSsavepartnerworkspacedto"></a>
<a id="tocssavepartnerworkspacedto"></a>

```json
{
  "name": "string",
  "companyId": "string",
  "addressLine1": "string",
  "addressLine2": "string",
  "city": "string",
  "country": "string",
  "email": "string",
  "contactName": "string",
  "contactLastName": "string",
  "contactEmail": "string",
  "contactPhone": "string",
  "phone": "string",
  "invoiceEmail": "string",
  "users": [
    {
      "userId": "string",
      "name": "string",
      "lastName": "string",
      "email": "string",
      "role": "string"
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|name|string¦null|false|none|none|
|companyId|string¦null|false|none|none|
|addressLine1|string¦null|false|none|none|
|addressLine2|string¦null|false|none|none|
|city|string¦null|false|none|none|
|country|string¦null|false|none|none|
|email|string¦null|false|none|none|
|contactName|string¦null|false|none|none|
|contactLastName|string¦null|false|none|none|
|contactEmail|string¦null|false|none|none|
|contactPhone|string¦null|false|none|none|
|phone|string¦null|false|none|none|
|invoiceEmail|string¦null|false|none|none|
|users|[[WorkspaceUserDto](#schemaworkspaceuserdto)]¦null|false|none|none|

<h2 id="tocS_SaveSponsorDto">SaveSponsorDto</h2>
<!-- backwards compatibility -->
<a id="schemasavesponsordto"></a>
<a id="schema_SaveSponsorDto"></a>
<a id="tocSsavesponsordto"></a>
<a id="tocssavesponsordto"></a>

```json
{
  "id": "string",
  "name": "string",
  "logoUrl": "string",
  "description": "string",
  "email": "string",
  "phoneNumber": "string",
  "website": "string",
  "address": "string",
  "links": [
    {
      "url": "string"
    }
  ],
  "stageStream": {
    "type": 0,
    "url": "string",
    "hostUrl": "string",
    "additionalUrls": [
      {
        "type": 0,
        "url": "string"
      }
    ],
    "rtmpSettings": {
      "streamKey": "string",
      "channelArn": "string",
      "recordings": [
        "string"
      ]
    },
    "settings": {
      "host": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      },
      "stream": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      },
      "startDate": "2019-08-24T14:15:22Z",
      "endDate": "2019-08-24T14:15:22Z"
    }
  },
  "order": 0,
  "isStreamTypeChangeForced": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string¦null|false|none|none|
|name|string¦null|false|none|none|
|logoUrl|string¦null|false|none|none|
|description|string¦null|false|none|none|
|email|string¦null|false|none|none|
|phoneNumber|string¦null|false|none|none|
|website|string¦null|false|none|none|
|address|string¦null|false|none|none|
|links|[[SocialLinkDto](#schemasociallinkdto)]¦null|false|none|none|
|stageStream|[StageStreamDtoBase](#schemastagestreamdtobase)|false|none|none|
|order|integer(int32)|false|none|none|
|isStreamTypeChangeForced|boolean|false|none|none|

<h2 id="tocS_SaveWorkspaceDto">SaveWorkspaceDto</h2>
<!-- backwards compatibility -->
<a id="schemasaveworkspacedto"></a>
<a id="schema_SaveWorkspaceDto"></a>
<a id="tocSsaveworkspacedto"></a>
<a id="tocssaveworkspacedto"></a>

```json
{
  "name": "string",
  "companyId": "string",
  "addressLine1": "string",
  "addressLine2": "string",
  "contactName": "string",
  "zipCode": "string",
  "city": "string",
  "state": "string",
  "country": "string",
  "contactLastName": "string",
  "phone": "string",
  "invoiceEmail": "user@example.com",
  "partnerWorkspaceId": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|name|string|true|none|none|
|companyId|string¦null|false|none|none|
|addressLine1|string¦null|false|none|none|
|addressLine2|string¦null|false|none|none|
|contactName|string¦null|false|none|none|
|zipCode|string¦null|false|none|none|
|city|string¦null|false|none|none|
|state|string¦null|false|none|none|
|country|string¦null|false|none|none|
|contactLastName|string¦null|false|none|none|
|phone|string(tel)¦null|false|none|none|
|invoiceEmail|string(email)¦null|false|none|none|
|partnerWorkspaceId|string¦null|false|none|none|

<h2 id="tocS_SelectListGroup">SelectListGroup</h2>
<!-- backwards compatibility -->
<a id="schemaselectlistgroup"></a>
<a id="schema_SelectListGroup"></a>
<a id="tocSselectlistgroup"></a>
<a id="tocsselectlistgroup"></a>

```json
{
  "disabled": true,
  "name": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|disabled|boolean|false|none|none|
|name|string¦null|false|none|none|

<h2 id="tocS_SelectListItem">SelectListItem</h2>
<!-- backwards compatibility -->
<a id="schemaselectlistitem"></a>
<a id="schema_SelectListItem"></a>
<a id="tocSselectlistitem"></a>
<a id="tocsselectlistitem"></a>

```json
{
  "disabled": true,
  "group": {
    "disabled": true,
    "name": "string"
  },
  "selected": true,
  "text": "string",
  "value": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|disabled|boolean|false|none|none|
|group|[SelectListGroup](#schemaselectlistgroup)|false|none|none|
|selected|boolean|false|none|none|
|text|string¦null|false|none|none|
|value|string¦null|false|none|none|

<h2 id="tocS_SendContactRequest">SendContactRequest</h2>
<!-- backwards compatibility -->
<a id="schemasendcontactrequest"></a>
<a id="schema_SendContactRequest"></a>
<a id="tocSsendcontactrequest"></a>
<a id="tocssendcontactrequest"></a>

```json
{
  "sponsorId": "string",
  "message": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|sponsorId|string¦null|false|none|none|
|message|string¦null|false|none|none|

<h2 id="tocS_SendEmailDto">SendEmailDto</h2>
<!-- backwards compatibility -->
<a id="schemasendemaildto"></a>
<a id="schema_SendEmailDto"></a>
<a id="tocSsendemaildto"></a>
<a id="tocssendemaildto"></a>

```json
{
  "eventId": "string",
  "senderIdentityId": "string",
  "subject": "string",
  "template": "string",
  "destinations": [
    {
      "registrationId": "string",
      "email": "string",
      "replacementData": {
        "property1": null,
        "property2": null
      }
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|eventId|string¦null|false|none|none|
|senderIdentityId|string¦null|false|none|none|
|subject|string¦null|false|none|none|
|template|string¦null|false|none|none|
|destinations|[[EmailDestinationDto](#schemaemaildestinationdto)]¦null|false|none|none|

<h2 id="tocS_SendMessageRequest">SendMessageRequest</h2>
<!-- backwards compatibility -->
<a id="schemasendmessagerequest"></a>
<a id="schema_SendMessageRequest"></a>
<a id="tocSsendmessagerequest"></a>
<a id="tocssendmessagerequest"></a>

```json
{
  "message": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|message|string¦null|false|none|none|

<h2 id="tocS_SendResetPasswordDto">SendResetPasswordDto</h2>
<!-- backwards compatibility -->
<a id="schemasendresetpassworddto"></a>
<a id="schema_SendResetPasswordDto"></a>
<a id="tocSsendresetpassworddto"></a>
<a id="tocssendresetpassworddto"></a>

```json
{
  "email": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|email|string¦null|false|none|none|

<h2 id="tocS_SendSmsDto">SendSmsDto</h2>
<!-- backwards compatibility -->
<a id="schemasendsmsdto"></a>
<a id="schema_SendSmsDto"></a>
<a id="tocSsendsmsdto"></a>
<a id="tocssendsmsdto"></a>

```json
{
  "eventId": "string",
  "sender": "string",
  "template": "string",
  "destinations": [
    {
      "registrationId": "string",
      "phoneNumber": "string",
      "text": "string",
      "messageId": "string",
      "error": {
        "errorName": "string",
        "errorDescription": "string"
      }
    }
  ],
  "sendDateTime": "2019-08-24T14:15:22Z"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|eventId|string¦null|false|none|none|
|sender|string¦null|false|none|none|
|template|string¦null|false|none|none|
|destinations|[[DestinationDto](#schemadestinationdto)]¦null|false|none|none|
|sendDateTime|string(date-time)¦null|false|none|none|

<h2 id="tocS_SignUpDto">SignUpDto</h2>
<!-- backwards compatibility -->
<a id="schemasignupdto"></a>
<a id="schema_SignUpDto"></a>
<a id="tocSsignupdto"></a>
<a id="tocssignupdto"></a>

```json
{
  "username": "user@example.com",
  "password": "string",
  "conditionsAccepted": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|username|string(email)|true|none|none|
|password|string|true|none|none|
|conditionsAccepted|boolean|false|none|none|

<h2 id="tocS_SlugAvailabilityRequest">SlugAvailabilityRequest</h2>
<!-- backwards compatibility -->
<a id="schemaslugavailabilityrequest"></a>
<a id="schema_SlugAvailabilityRequest"></a>
<a id="tocSslugavailabilityrequest"></a>
<a id="tocsslugavailabilityrequest"></a>

```json
{
  "eventId": "string",
  "slug": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|eventId|string¦null|false|none|none|
|slug|string¦null|false|none|none|

<h2 id="tocS_SmsAuditErrorDto">SmsAuditErrorDto</h2>
<!-- backwards compatibility -->
<a id="schemasmsauditerrordto"></a>
<a id="schema_SmsAuditErrorDto"></a>
<a id="tocSsmsauditerrordto"></a>
<a id="tocssmsauditerrordto"></a>

```json
{
  "errorName": "string",
  "errorDescription": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|errorName|string¦null|false|none|none|
|errorDescription|string¦null|false|none|none|

<h2 id="tocS_SMSReport">SMSReport</h2>
<!-- backwards compatibility -->
<a id="schemasmsreport"></a>
<a id="schema_SMSReport"></a>
<a id="tocSsmsreport"></a>
<a id="tocssmsreport"></a>

```json
{
  "bulkId": "string",
  "messageId": "string",
  "to": "string",
  "from": "string",
  "text": "string",
  "sentAt": "2019-08-24T14:15:22Z",
  "doneAt": "2019-08-24T14:15:22Z",
  "smsCount": 0,
  "mccMnc": "string",
  "price": {
    "pricePerMessage": 0,
    "pricePerLookup": 0,
    "currency": "string"
  },
  "status": {
    "groupId": 0,
    "groupName": "string",
    "id": 0,
    "name": "string",
    "description": "string",
    "action": "string"
  },
  "error": {
    "groupId": 0,
    "groupName": "string",
    "id": 0,
    "name": "string",
    "description": "string",
    "permanent": true
  },
  "callbackData": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|bulkId|string¦null|false|none|none|
|messageId|string¦null|false|none|none|
|to|string¦null|false|none|none|
|from|string¦null|false|none|none|
|text|string¦null|false|none|none|
|sentAt|string(date-time)¦null|false|none|none|
|doneAt|string(date-time)¦null|false|none|none|
|smsCount|integer(int32)¦null|false|none|none|
|mccMnc|string¦null|false|none|none|
|price|[Price](#schemaprice)|false|none|none|
|status|[Status](#schemastatus)|false|none|none|
|error|[Error](#schemaerror)|false|none|none|
|callbackData|string¦null|false|none|none|

<h2 id="tocS_SMSReportResponse">SMSReportResponse</h2>
<!-- backwards compatibility -->
<a id="schemasmsreportresponse"></a>
<a id="schema_SMSReportResponse"></a>
<a id="tocSsmsreportresponse"></a>
<a id="tocssmsreportresponse"></a>

```json
{
  "results": [
    {
      "bulkId": "string",
      "messageId": "string",
      "to": "string",
      "from": "string",
      "text": "string",
      "sentAt": "2019-08-24T14:15:22Z",
      "doneAt": "2019-08-24T14:15:22Z",
      "smsCount": 0,
      "mccMnc": "string",
      "price": {
        "pricePerMessage": 0,
        "pricePerLookup": 0,
        "currency": "string"
      },
      "status": {
        "groupId": 0,
        "groupName": "string",
        "id": 0,
        "name": "string",
        "description": "string",
        "action": "string"
      },
      "error": {
        "groupId": 0,
        "groupName": "string",
        "id": 0,
        "name": "string",
        "description": "string",
        "permanent": true
      },
      "callbackData": "string"
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|results|[[SMSReport](#schemasmsreport)]¦null|false|none|none|

<h2 id="tocS_SocialLinkDto">SocialLinkDto</h2>
<!-- backwards compatibility -->
<a id="schemasociallinkdto"></a>
<a id="schema_SocialLinkDto"></a>
<a id="tocSsociallinkdto"></a>
<a id="tocssociallinkdto"></a>

```json
{
  "url": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|url|string¦null|false|none|none|

<h2 id="tocS_SpeakerDto">SpeakerDto</h2>
<!-- backwards compatibility -->
<a id="schemaspeakerdto"></a>
<a id="schema_SpeakerDto"></a>
<a id="tocSspeakerdto"></a>
<a id="tocsspeakerdto"></a>

```json
{
  "id": "string",
  "eventId": "string",
  "name": "string",
  "lastName": "string",
  "company": "string",
  "jobTitle": "string",
  "email": "string",
  "phoneNumber": "string",
  "description": "string",
  "profileImageUrl": "string",
  "order": 0,
  "links": [
    {
      "url": "string"
    }
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string¦null|false|none|none|
|eventId|string¦null|false|none|none|
|name|string¦null|false|none|none|
|lastName|string¦null|false|none|none|
|company|string¦null|false|none|none|
|jobTitle|string¦null|false|none|none|
|email|string¦null|false|none|none|
|phoneNumber|string¦null|false|none|none|
|description|string¦null|false|none|none|
|profileImageUrl|string¦null|false|none|none|
|order|integer(int32)|false|none|none|
|links|[[SocialLinkDto](#schemasociallinkdto)]¦null|false|none|none|

<h2 id="tocS_StageRTMPStreamSettingsDto">StageRTMPStreamSettingsDto</h2>
<!-- backwards compatibility -->
<a id="schemastagertmpstreamsettingsdto"></a>
<a id="schema_StageRTMPStreamSettingsDto"></a>
<a id="tocSstagertmpstreamsettingsdto"></a>
<a id="tocsstagertmpstreamsettingsdto"></a>

```json
{
  "streamKey": "string",
  "channelArn": "string",
  "recordings": [
    "string"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|streamKey|string¦null|false|none|none|
|channelArn|string¦null|false|none|none|
|recordings|[string]¦null|false|none|none|

<h2 id="tocS_StageStreamDtoBase">StageStreamDtoBase</h2>
<!-- backwards compatibility -->
<a id="schemastagestreamdtobase"></a>
<a id="schema_StageStreamDtoBase"></a>
<a id="tocSstagestreamdtobase"></a>
<a id="tocsstagestreamdtobase"></a>

```json
{
  "type": 0,
  "url": "string",
  "hostUrl": "string",
  "additionalUrls": [
    {
      "type": 0,
      "url": "string"
    }
  ],
  "rtmpSettings": {
    "streamKey": "string",
    "channelArn": "string",
    "recordings": [
      "string"
    ]
  },
  "settings": {
    "host": {
      "isChatEnabled": true,
      "isPeopleEnabled": true,
      "isLeaveButtonEnabled": true,
      "isRecordingEnabled": true,
      "isScreenShareEnabled": true,
      "isBackgroundEnabled": true,
      "isVideoEnabled": true,
      "isAudioEnabled": true,
      "isBreakoutEnabled": true
    },
    "stream": {
      "isChatEnabled": true,
      "isPeopleEnabled": true,
      "isLeaveButtonEnabled": true,
      "isRecordingEnabled": true,
      "isScreenShareEnabled": true,
      "isBackgroundEnabled": true,
      "isVideoEnabled": true,
      "isAudioEnabled": true,
      "isBreakoutEnabled": true
    },
    "startDate": "2019-08-24T14:15:22Z",
    "endDate": "2019-08-24T14:15:22Z"
  }
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|type|[StageStreamType](#schemastagestreamtype)|false|none|none|
|url|string¦null|false|none|none|
|hostUrl|string¦null|false|none|none|
|additionalUrls|[[StageStreamUrlDto](#schemastagestreamurldto)]¦null|false|none|none|
|rtmpSettings|[StageRTMPStreamSettingsDto](#schemastagertmpstreamsettingsdto)|false|none|none|
|settings|[StageStreamSettingsDto](#schemastagestreamsettingsdto)|false|none|none|

<h2 id="tocS_StageStreamPatchDto">StageStreamPatchDto</h2>
<!-- backwards compatibility -->
<a id="schemastagestreampatchdto"></a>
<a id="schema_StageStreamPatchDto"></a>
<a id="tocSstagestreampatchdto"></a>
<a id="tocsstagestreampatchdto"></a>

```json
{
  "type": 0,
  "url": "string",
  "settings": {
    "host": {
      "isChatEnabled": true,
      "isPeopleEnabled": true,
      "isLeaveButtonEnabled": true,
      "isRecordingEnabled": true,
      "isScreenShareEnabled": true,
      "isBackgroundEnabled": true,
      "isVideoEnabled": true,
      "isAudioEnabled": true,
      "isBreakoutEnabled": true
    },
    "stream": {
      "isChatEnabled": true,
      "isPeopleEnabled": true,
      "isLeaveButtonEnabled": true,
      "isRecordingEnabled": true,
      "isScreenShareEnabled": true,
      "isBackgroundEnabled": true,
      "isVideoEnabled": true,
      "isAudioEnabled": true,
      "isBreakoutEnabled": true
    }
  }
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|type|[StageStreamType](#schemastagestreamtype)|false|none|none|
|url|string¦null|false|none|none|
|settings|[StageStreamSettingsPatchDto](#schemastagestreamsettingspatchdto)|false|none|none|

<h2 id="tocS_StageStreamSettingsDto">StageStreamSettingsDto</h2>
<!-- backwards compatibility -->
<a id="schemastagestreamsettingsdto"></a>
<a id="schema_StageStreamSettingsDto"></a>
<a id="tocSstagestreamsettingsdto"></a>
<a id="tocsstagestreamsettingsdto"></a>

```json
{
  "host": {
    "isChatEnabled": true,
    "isPeopleEnabled": true,
    "isLeaveButtonEnabled": true,
    "isRecordingEnabled": true,
    "isScreenShareEnabled": true,
    "isBackgroundEnabled": true,
    "isVideoEnabled": true,
    "isAudioEnabled": true,
    "isBreakoutEnabled": true
  },
  "stream": {
    "isChatEnabled": true,
    "isPeopleEnabled": true,
    "isLeaveButtonEnabled": true,
    "isRecordingEnabled": true,
    "isScreenShareEnabled": true,
    "isBackgroundEnabled": true,
    "isVideoEnabled": true,
    "isAudioEnabled": true,
    "isBreakoutEnabled": true
  },
  "startDate": "2019-08-24T14:15:22Z",
  "endDate": "2019-08-24T14:15:22Z"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|host|[StreamSettingsDto](#schemastreamsettingsdto)|false|none|none|
|stream|[StreamSettingsDto](#schemastreamsettingsdto)|false|none|none|
|startDate|string(date-time)|false|none|none|
|endDate|string(date-time)|false|none|none|

<h2 id="tocS_StageStreamSettingsPatchDto">StageStreamSettingsPatchDto</h2>
<!-- backwards compatibility -->
<a id="schemastagestreamsettingspatchdto"></a>
<a id="schema_StageStreamSettingsPatchDto"></a>
<a id="tocSstagestreamsettingspatchdto"></a>
<a id="tocsstagestreamsettingspatchdto"></a>

```json
{
  "host": {
    "isChatEnabled": true,
    "isPeopleEnabled": true,
    "isLeaveButtonEnabled": true,
    "isRecordingEnabled": true,
    "isScreenShareEnabled": true,
    "isBackgroundEnabled": true,
    "isVideoEnabled": true,
    "isAudioEnabled": true,
    "isBreakoutEnabled": true
  },
  "stream": {
    "isChatEnabled": true,
    "isPeopleEnabled": true,
    "isLeaveButtonEnabled": true,
    "isRecordingEnabled": true,
    "isScreenShareEnabled": true,
    "isBackgroundEnabled": true,
    "isVideoEnabled": true,
    "isAudioEnabled": true,
    "isBreakoutEnabled": true
  }
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|host|[StreamSettingsPatchDto](#schemastreamsettingspatchdto)|false|none|none|
|stream|[StreamSettingsPatchDto](#schemastreamsettingspatchdto)|false|none|none|

<h2 id="tocS_StageStreamType">StageStreamType</h2>
<!-- backwards compatibility -->
<a id="schemastagestreamtype"></a>
<a id="schema_StageStreamType"></a>
<a id="tocSstagestreamtype"></a>
<a id="tocsstagestreamtype"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|0|
|*anonymous*|1|
|*anonymous*|2|
|*anonymous*|3|

<h2 id="tocS_StageStreamUrlDto">StageStreamUrlDto</h2>
<!-- backwards compatibility -->
<a id="schemastagestreamurldto"></a>
<a id="schema_StageStreamUrlDto"></a>
<a id="tocSstagestreamurldto"></a>
<a id="tocsstagestreamurldto"></a>

```json
{
  "type": 0,
  "url": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|type|[StageStreamUrlType](#schemastagestreamurltype)|false|none|none|
|url|string¦null|false|none|none|

<h2 id="tocS_StageStreamUrlType">StageStreamUrlType</h2>
<!-- backwards compatibility -->
<a id="schemastagestreamurltype"></a>
<a id="schema_StageStreamUrlType"></a>
<a id="tocSstagestreamurltype"></a>
<a id="tocsstagestreamurltype"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|0|

<h2 id="tocS_Status">Status</h2>
<!-- backwards compatibility -->
<a id="schemastatus"></a>
<a id="schema_Status"></a>
<a id="tocSstatus"></a>
<a id="tocsstatus"></a>

```json
{
  "groupId": 0,
  "groupName": "string",
  "id": 0,
  "name": "string",
  "description": "string",
  "action": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|groupId|integer(int32)¦null|false|none|none|
|groupName|string¦null|false|none|none|
|id|integer(int32)¦null|false|none|none|
|name|string¦null|false|none|none|
|description|string¦null|false|none|none|
|action|string¦null|false|none|none|

<h2 id="tocS_StorePollAnswerRequest">StorePollAnswerRequest</h2>
<!-- backwards compatibility -->
<a id="schemastorepollanswerrequest"></a>
<a id="schema_StorePollAnswerRequest"></a>
<a id="tocSstorepollanswerrequest"></a>
<a id="tocsstorepollanswerrequest"></a>

```json
{
  "pollId": "string",
  "questionType": "string",
  "alternatives": [
    "string"
  ]
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|pollId|string¦null|false|none|none|
|questionType|string¦null|false|none|none|
|alternatives|[string]¦null|false|none|none|

<h2 id="tocS_StorePollOpenTextAnswerRequest">StorePollOpenTextAnswerRequest</h2>
<!-- backwards compatibility -->
<a id="schemastorepollopentextanswerrequest"></a>
<a id="schema_StorePollOpenTextAnswerRequest"></a>
<a id="tocSstorepollopentextanswerrequest"></a>
<a id="tocsstorepollopentextanswerrequest"></a>

```json
{
  "pollId": "string",
  "label": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|pollId|string¦null|false|none|none|
|label|string¦null|false|none|none|

<h2 id="tocS_StreamSettingsDto">StreamSettingsDto</h2>
<!-- backwards compatibility -->
<a id="schemastreamsettingsdto"></a>
<a id="schema_StreamSettingsDto"></a>
<a id="tocSstreamsettingsdto"></a>
<a id="tocsstreamsettingsdto"></a>

```json
{
  "isChatEnabled": true,
  "isPeopleEnabled": true,
  "isLeaveButtonEnabled": true,
  "isRecordingEnabled": true,
  "isScreenShareEnabled": true,
  "isBackgroundEnabled": true,
  "isVideoEnabled": true,
  "isAudioEnabled": true,
  "isBreakoutEnabled": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|isChatEnabled|boolean|false|none|none|
|isPeopleEnabled|boolean|false|none|none|
|isLeaveButtonEnabled|boolean|false|none|none|
|isRecordingEnabled|boolean|false|none|none|
|isScreenShareEnabled|boolean|false|none|none|
|isBackgroundEnabled|boolean|false|none|none|
|isVideoEnabled|boolean|false|none|none|
|isAudioEnabled|boolean|false|none|none|
|isBreakoutEnabled|boolean|false|none|none|

<h2 id="tocS_StreamSettingsPatchDto">StreamSettingsPatchDto</h2>
<!-- backwards compatibility -->
<a id="schemastreamsettingspatchdto"></a>
<a id="schema_StreamSettingsPatchDto"></a>
<a id="tocSstreamsettingspatchdto"></a>
<a id="tocsstreamsettingspatchdto"></a>

```json
{
  "isChatEnabled": true,
  "isPeopleEnabled": true,
  "isLeaveButtonEnabled": true,
  "isRecordingEnabled": true,
  "isScreenShareEnabled": true,
  "isBackgroundEnabled": true,
  "isVideoEnabled": true,
  "isAudioEnabled": true,
  "isBreakoutEnabled": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|isChatEnabled|boolean|false|none|none|
|isPeopleEnabled|boolean|false|none|none|
|isLeaveButtonEnabled|boolean|false|none|none|
|isRecordingEnabled|boolean|false|none|none|
|isScreenShareEnabled|boolean|false|none|none|
|isBackgroundEnabled|boolean|false|none|none|
|isVideoEnabled|boolean|false|none|none|
|isAudioEnabled|boolean|false|none|none|
|isBreakoutEnabled|boolean|false|none|none|

<h2 id="tocS_TemplateDto">TemplateDto</h2>
<!-- backwards compatibility -->
<a id="schematemplatedto"></a>
<a id="schema_TemplateDto"></a>
<a id="tocStemplatedto"></a>
<a id="tocstemplatedto"></a>

```json
{
  "id": "string",
  "createdOn": "2019-08-24T14:15:22Z",
  "code": "string",
  "name": "string",
  "description": "string",
  "content": "string",
  "subject": "string",
  "emailSenderIdentityId": "string",
  "type": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string¦null|false|none|none|
|createdOn|string(date-time)¦null|false|none|none|
|code|string¦null|false|none|none|
|name|string¦null|false|none|none|
|description|string¦null|false|none|none|
|content|string¦null|false|none|none|
|subject|string¦null|false|none|none|
|emailSenderIdentityId|string¦null|false|none|none|
|type|[TemplateType](#schematemplatetype)|false|none|none|

<h2 id="tocS_TemplateType">TemplateType</h2>
<!-- backwards compatibility -->
<a id="schematemplatetype"></a>
<a id="schema_TemplateType"></a>
<a id="tocStemplatetype"></a>
<a id="tocstemplatetype"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|0|
|*anonymous*|1|

<h2 id="tocS_TermsAcceptanceRequest">TermsAcceptanceRequest</h2>
<!-- backwards compatibility -->
<a id="schematermsacceptancerequest"></a>
<a id="schema_TermsAcceptanceRequest"></a>
<a id="tocStermsacceptancerequest"></a>
<a id="tocstermsacceptancerequest"></a>

```json
{
  "termsText": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|termsText|string¦null|false|none|none|

<h2 id="tocS_TicketDto">TicketDto</h2>
<!-- backwards compatibility -->
<a id="schematicketdto"></a>
<a id="schema_TicketDto"></a>
<a id="tocSticketdto"></a>
<a id="tocsticketdto"></a>

```json
{
  "url": "string",
  "barcode": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|url|string¦null|false|none|none|
|barcode|string¦null|false|none|none|

<h2 id="tocS_TogglePollAnswerPresentationRequest">TogglePollAnswerPresentationRequest</h2>
<!-- backwards compatibility -->
<a id="schematogglepollanswerpresentationrequest"></a>
<a id="schema_TogglePollAnswerPresentationRequest"></a>
<a id="tocStogglepollanswerpresentationrequest"></a>
<a id="tocstogglepollanswerpresentationrequest"></a>

```json
{
  "label": "string",
  "presentType": 0
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|label|string¦null|false|none|none|
|presentType|[PresentType](#schemapresenttype)|false|none|none|

<h2 id="tocS_UnlikeTimelineEntryRequest">UnlikeTimelineEntryRequest</h2>
<!-- backwards compatibility -->
<a id="schemaunliketimelineentryrequest"></a>
<a id="schema_UnlikeTimelineEntryRequest"></a>
<a id="tocSunliketimelineentryrequest"></a>
<a id="tocsunliketimelineentryrequest"></a>

```json
{
  "entryId": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|entryId|string¦null|false|none|none|

<h2 id="tocS_UpdateEmailAddressRequest">UpdateEmailAddressRequest</h2>
<!-- backwards compatibility -->
<a id="schemaupdateemailaddressrequest"></a>
<a id="schema_UpdateEmailAddressRequest"></a>
<a id="tocSupdateemailaddressrequest"></a>
<a id="tocsupdateemailaddressrequest"></a>

```json
{
  "email": "string",
  "friendlyName": "string",
  "isDefault": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|email|string¦null|false|none|none|
|friendlyName|string¦null|false|none|none|
|isDefault|boolean|false|none|none|

<h2 id="tocS_UpdateEventDto">UpdateEventDto</h2>
<!-- backwards compatibility -->
<a id="schemaupdateeventdto"></a>
<a id="schema_UpdateEventDto"></a>
<a id="tocSupdateeventdto"></a>
<a id="tocsupdateeventdto"></a>

```json
{
  "name": "string",
  "slug": "string",
  "description": "string",
  "venue": "string",
  "isPaymentEnabled": true,
  "price": 0,
  "paymentApiKey": "string",
  "paymentApiSecret": "string",
  "timezone": "string",
  "currency": "string",
  "language": "string",
  "dataControllerName": "string",
  "dataControllerEmail": "user@example.com",
  "dataProcessorName": "string",
  "dataProcessorEmail": "user@example.com",
  "isLiveEventEnabled": true,
  "isRegistrationEnabled": true,
  "isMinglEvent": true,
  "startDate": "2019-08-24T14:15:22Z",
  "endDate": "2019-08-24T14:15:22Z",
  "isDirty": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|name|string|true|none|none|
|slug|string¦null|false|none|none|
|description|string¦null|false|none|none|
|venue|string¦null|false|none|none|
|isPaymentEnabled|boolean|false|none|none|
|price|number(double)¦null|false|none|none|
|paymentApiKey|string¦null|false|none|none|
|paymentApiSecret|string¦null|false|none|none|
|timezone|string|true|none|none|
|currency|string¦null|false|none|none|
|language|string|true|none|none|
|dataControllerName|string|true|none|none|
|dataControllerEmail|string(email)|true|none|none|
|dataProcessorName|string|true|none|none|
|dataProcessorEmail|string(email)|true|none|none|
|isLiveEventEnabled|boolean¦null|false|none|none|
|isRegistrationEnabled|boolean¦null|false|none|none|
|isMinglEvent|boolean¦null|false|none|none|
|startDate|string(date-time)|true|none|none|
|endDate|string(date-time)¦null|false|none|none|
|isDirty|boolean|false|none|none|

<h2 id="tocS_UpdatePaymentMethodDto">UpdatePaymentMethodDto</h2>
<!-- backwards compatibility -->
<a id="schemaupdatepaymentmethoddto"></a>
<a id="schema_UpdatePaymentMethodDto"></a>
<a id="tocSupdatepaymentmethoddto"></a>
<a id="tocsupdatepaymentmethoddto"></a>

```json
{
  "workspaceId": "string",
  "temporaryToken": "string",
  "firstName": "string",
  "lastName": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|workspaceId|string¦null|false|none|none|
|temporaryToken|string¦null|false|none|none|
|firstName|string¦null|false|none|none|
|lastName|string¦null|false|none|none|

<h2 id="tocS_UpdateRegistrationDto">UpdateRegistrationDto</h2>
<!-- backwards compatibility -->
<a id="schemaupdateregistrationdto"></a>
<a id="schema_UpdateRegistrationDto"></a>
<a id="tocSupdateregistrationdto"></a>
<a id="tocsupdateregistrationdto"></a>

```json
{
  "eventId": "string",
  "registrationId": "string",
  "values": {
    "property1": "string",
    "property2": "string"
  },
  "reservations": [
    {
      "id": "string",
      "entityId": "string",
      "token": "string",
      "contextId": "string",
      "isUsed": true
    }
  ],
  "ticket": {
    "url": "string",
    "barcode": "string"
  }
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|eventId|string¦null|false|none|none|
|registrationId|string¦null|false|none|none|
|values|object¦null|false|none|none|
|» **additionalProperties**|string|false|none|none|
|reservations|[[ReservedItemDto](#schemareserveditemdto)]¦null|false|none|none|
|ticket|[TicketDto](#schematicketdto)|false|none|none|

<h2 id="tocS_UpdateSessionRequest">UpdateSessionRequest</h2>
<!-- backwards compatibility -->
<a id="schemaupdatesessionrequest"></a>
<a id="schema_UpdateSessionRequest"></a>
<a id="tocSupdatesessionrequest"></a>
<a id="tocsupdatesessionrequest"></a>

```json
{
  "title": "string",
  "startDate": "2019-08-24T14:15:22Z",
  "endDate": "2019-08-24T14:15:22Z",
  "trackId": "string",
  "description": "string",
  "speakerIds": [
    "string"
  ],
  "stageStream": {
    "type": 0,
    "url": "string",
    "hostUrl": "string",
    "additionalUrls": [
      {
        "type": 0,
        "url": "string"
      }
    ],
    "rtmpSettings": {
      "streamKey": "string",
      "channelArn": "string",
      "recordings": [
        "string"
      ]
    },
    "settings": {
      "host": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      },
      "stream": {
        "isChatEnabled": true,
        "isPeopleEnabled": true,
        "isLeaveButtonEnabled": true,
        "isRecordingEnabled": true,
        "isScreenShareEnabled": true,
        "isBackgroundEnabled": true,
        "isVideoEnabled": true,
        "isAudioEnabled": true,
        "isBreakoutEnabled": true
      },
      "startDate": "2019-08-24T14:15:22Z",
      "endDate": "2019-08-24T14:15:22Z"
    }
  },
  "groupIds": [
    "string"
  ],
  "isStreamTypeChangeForced": true,
  "id": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|title|string|true|none|none|
|startDate|string(date-time)|true|none|none|
|endDate|string(date-time)|true|none|none|
|trackId|string|true|none|none|
|description|string¦null|false|none|none|
|speakerIds|[string]¦null|false|none|none|
|stageStream|[StageStreamDtoBase](#schemastagestreamdtobase)|false|none|none|
|groupIds|[string]¦null|false|none|none|
|isStreamTypeChangeForced|boolean|false|none|none|
|id|string¦null|false|none|none|

<h2 id="tocS_UpdateTrackRequest">UpdateTrackRequest</h2>
<!-- backwards compatibility -->
<a id="schemaupdatetrackrequest"></a>
<a id="schema_UpdateTrackRequest"></a>
<a id="tocSupdatetrackrequest"></a>
<a id="tocsupdatetrackrequest"></a>

```json
{
  "title": "string",
  "headerBackgroundColor": "string",
  "id": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|title|string|true|none|none|
|headerBackgroundColor|string|true|none|none|
|id|string¦null|false|none|none|

<h2 id="tocS_UpdateUserDto">UpdateUserDto</h2>
<!-- backwards compatibility -->
<a id="schemaupdateuserdto"></a>
<a id="schema_UpdateUserDto"></a>
<a id="tocSupdateuserdto"></a>
<a id="tocsupdateuserdto"></a>

```json
{
  "name": "string",
  "lastName": "string",
  "phoneNumber": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|name|string¦null|false|none|none|
|lastName|string¦null|false|none|none|
|phoneNumber|string¦null|false|none|none|

<h2 id="tocS_UpdateUserPictureRequest">UpdateUserPictureRequest</h2>
<!-- backwards compatibility -->
<a id="schemaupdateuserpicturerequest"></a>
<a id="schema_UpdateUserPictureRequest"></a>
<a id="tocSupdateuserpicturerequest"></a>
<a id="tocsupdateuserpicturerequest"></a>

```json
{
  "imageBase64WithContext": "string",
  "fileName": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|imageBase64WithContext|string¦null|false|none|none|
|fileName|string¦null|false|none|none|

<h2 id="tocS_UpdateUserRequest">UpdateUserRequest</h2>
<!-- backwards compatibility -->
<a id="schemaupdateuserrequest"></a>
<a id="schema_UpdateUserRequest"></a>
<a id="tocSupdateuserrequest"></a>
<a id="tocsupdateuserrequest"></a>

```json
{
  "userId": "string",
  "name": "string",
  "lastName": "string",
  "email": "string",
  "description": "string",
  "company": "string",
  "jobTitle": "string",
  "fullName": "string",
  "phoneNumber": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|userId|string¦null|false|none|none|
|name|string¦null|false|none|none|
|lastName|string¦null|false|none|none|
|email|string¦null|false|none|none|
|description|string¦null|false|none|none|
|company|string¦null|false|none|none|
|jobTitle|string¦null|false|none|none|
|fullName|string¦null|false|none|none|
|phoneNumber|string¦null|false|none|none|

<h2 id="tocS_UpdateUserWorkspaceDto">UpdateUserWorkspaceDto</h2>
<!-- backwards compatibility -->
<a id="schemaupdateuserworkspacedto"></a>
<a id="schema_UpdateUserWorkspaceDto"></a>
<a id="tocSupdateuserworkspacedto"></a>
<a id="tocsupdateuserworkspacedto"></a>

```json
{
  "workspaceId": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|workspaceId|string¦null|false|none|none|

<h2 id="tocS_ValidateResetPasswordTokenRequest">ValidateResetPasswordTokenRequest</h2>
<!-- backwards compatibility -->
<a id="schemavalidateresetpasswordtokenrequest"></a>
<a id="schema_ValidateResetPasswordTokenRequest"></a>
<a id="tocSvalidateresetpasswordtokenrequest"></a>
<a id="tocsvalidateresetpasswordtokenrequest"></a>

```json
{
  "userId": "string",
  "token": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|userId|string¦null|false|none|none|
|token|string¦null|false|none|none|

<h2 id="tocS_VerifyEmailAddressRequest">VerifyEmailAddressRequest</h2>
<!-- backwards compatibility -->
<a id="schemaverifyemailaddressrequest"></a>
<a id="schema_VerifyEmailAddressRequest"></a>
<a id="tocSverifyemailaddressrequest"></a>
<a id="tocsverifyemailaddressrequest"></a>

```json
{
  "email": "string",
  "friendlyName": "string",
  "isDefault": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|email|string¦null|false|none|none|
|friendlyName|string¦null|false|none|none|
|isDefault|boolean|false|none|none|

<h2 id="tocS_WidgetType">WidgetType</h2>
<!-- backwards compatibility -->
<a id="schemawidgettype"></a>
<a id="schema_WidgetType"></a>
<a id="tocSwidgettype"></a>
<a id="tocswidgettype"></a>

```json
1

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|1|
|*anonymous*|2|
|*anonymous*|3|
|*anonymous*|4|
|*anonymous*|5|
|*anonymous*|6|
|*anonymous*|7|

<h2 id="tocS_WidgetUpdateDto">WidgetUpdateDto</h2>
<!-- backwards compatibility -->
<a id="schemawidgetupdatedto"></a>
<a id="schema_WidgetUpdateDto"></a>
<a id="tocSwidgetupdatedto"></a>
<a id="tocswidgetupdatedto"></a>

```json
{
  "id": "string",
  "type": 1,
  "options": null,
  "mandatory": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|id|string¦null|false|none|none|
|type|[WidgetType](#schemawidgettype)|false|none|none|
|options|any|true|none|none|
|mandatory|boolean|false|none|none|

<h2 id="tocS_WorkspaceClientLinkDto">WorkspaceClientLinkDto</h2>
<!-- backwards compatibility -->
<a id="schemaworkspaceclientlinkdto"></a>
<a id="schema_WorkspaceClientLinkDto"></a>
<a id="tocSworkspaceclientlinkdto"></a>
<a id="tocsworkspaceclientlinkdto"></a>

```json
{
  "clientId": "string",
  "workspaceId": "string",
  "name": "string",
  "eventCount": 0,
  "isUnlink": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|clientId|string¦null|false|none|none|
|workspaceId|string¦null|false|none|none|
|name|string¦null|false|none|none|
|eventCount|integer(int32)|false|none|none|
|isUnlink|boolean|false|none|none|

<h2 id="tocS_WorkspaceFeatureSetDto">WorkspaceFeatureSetDto</h2>
<!-- backwards compatibility -->
<a id="schemaworkspacefeaturesetdto"></a>
<a id="schema_WorkspaceFeatureSetDto"></a>
<a id="tocSworkspacefeaturesetdto"></a>
<a id="tocsworkspacefeaturesetdto"></a>

```json
{
  "isSupportEnabled": true,
  "isLobbyPageEnabled": true,
  "isChatEnabled": true,
  "isSpeakersEnabled": true,
  "isAgendaEnabled": true,
  "isRTMPStreamEnabled": true,
  "isSponsorsEnabled": true,
  "isClientsAffected": true
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|isSupportEnabled|boolean|false|none|none|
|isLobbyPageEnabled|boolean|false|none|none|
|isChatEnabled|boolean|false|none|none|
|isSpeakersEnabled|boolean|false|none|none|
|isAgendaEnabled|boolean|false|none|none|
|isRTMPStreamEnabled|boolean|false|none|none|
|isSponsorsEnabled|boolean|false|none|none|
|isClientsAffected|boolean|false|none|none|

<h2 id="tocS_WorkspaceFeatureType">WorkspaceFeatureType</h2>
<!-- backwards compatibility -->
<a id="schemaworkspacefeaturetype"></a>
<a id="schema_WorkspaceFeatureType"></a>
<a id="tocSworkspacefeaturetype"></a>
<a id="tocsworkspacefeaturetype"></a>

```json
0

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|*anonymous*|integer(int32)|false|none|none|

#### Enumerated Values

|Property|Value|
|---|---|
|*anonymous*|0|
|*anonymous*|1|

<h2 id="tocS_WorkspaceUserDto">WorkspaceUserDto</h2>
<!-- backwards compatibility -->
<a id="schemaworkspaceuserdto"></a>
<a id="schema_WorkspaceUserDto"></a>
<a id="tocSworkspaceuserdto"></a>
<a id="tocsworkspaceuserdto"></a>

```json
{
  "userId": "string",
  "name": "string",
  "lastName": "string",
  "email": "string",
  "role": "string"
}

```

### Properties

|Name|Type|Required|Restrictions|Description|
|---|---|---|---|---|
|userId|string¦null|false|none|none|
|name|string¦null|false|none|none|
|lastName|string¦null|false|none|none|
|email|string¦null|false|none|none|
|role|string¦null|false|none|none|

