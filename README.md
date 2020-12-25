# Cookify.js
A simple, extreme light weight javascript cookie library. Cookify JS is a simple script which lets you manage cookies in an easy way. Adding cookify JS to your project is super easy! To add and use cookify js, read our documentation or see the steps below. This is for the latest version 1.0.0

## ⚙️ Installation

#### Using CDN

Cookify JS can be added to your project by our CDN. To add cookify JS CDN to your project, just add the code below to the footer in your `.html` document
<br>Note: You should load this script before other scripts
```
<script src='https://cdn.jsdelivr.net/gh/Harry260/cookify.js/app.js' ></script>
```
#### Using File
You can download the file `app.js` and link it to your `.html` document using:<br>
```
<script src='PATH-TO-FILE' ></script>
```
Note: Here path refers to the path to the file `app.js`
<br>
## 🤔 How to Use it?
Using cookify JS is super-easy once after adding the CCDN to you footer. With cookief JS, you can `set`, `get`, `delete`, `clear` (all cookie at once),  `obj` (Get all cookies as object).

#### Setting cookie
To set cookie, you only need one line
```
Cookie.set(cookie name, cookie value, expiry date)
```

Here cookie name and cookie value can be null, but not recommended. But if cookie expiry date is null, the date will be set to `365` days automatically. You can also update a cookie with the same method `set()`

###### Example
```
var cookie_name = 'My_Cookie';
var cookie_value = 'Hello World';
var cookie_ex = 29; //Cookie expiry date in days
console.log(Cookie.set(cookie_name, cookie_value, cookie_ex)); // Return { name:My_Cookie, value:Hello World  }
```

#### Getting cookie
To get saved cookie, we use `get()` Method
```
Cookie.set(cookie name, cookie value, expiry date)
```

To get a cookie value, we only need the name of the cookie. So, we use `get()` method to get the cookie value.

###### Example
```
var cookie_name = 'My_Cookie';
console.log(Cookie.get(cookie_name)); // Return Hello_World
```

#### Deleting cookie
Parameters for Deleting cookie is almost same as getting a cookie.
To delete cookie, we only need the name of the cookie as parameter. 

```
  Cookie.delete(cookie name)
```

###### Example
```
var cookie_name = 'My_Cookie';
console.log(Cookie.delete(cookie name)) //Return 'success'
```

#### Clear all cookies
To clear all cookie, we dont use any parameter. This `clear()` method can be used to clear all the cookies.
```
Cookie.clear()
```

###### Example
```
var cookie_name = 'My_Cookie';
console.log(Cookie.get(cookie_name)); // Return Hello_World
```


#### Get all cookies as Object
With cookify JS, You can extract an object with `key` (Name of cookie) and `value` (Value of cookie) of the cookis saved in your domain.<br>

```
Cookie.obj()
```

The return will be in this format:
```
//This is am example
{
   username:'harto',
   profilepic:'harrytom.ml/assets/me.jpg',
   rep:236,
}
```

```
Cookie.clear()
```
