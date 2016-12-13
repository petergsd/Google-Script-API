# Google-Script-API
This is one example that use **Google Apps Script** implemented as **executable API** to send emails through **Gmail API**.

Send emails with Google Script API is much easier than a classic method.

####How to:
To use it, simply:

* Create a project on **[Google Developers Console](https://console.developers.google.com/)** enabling the **Gmail** and **Google Script Execution API**. Then extract the client ID and paste it on:

```js
var CLIENT_ID = 'XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX';
```

* Create a Google Script file on **[Google Apps Script](https://script.google.com/)**. The Google Script code used is:

```js
function myFunction(email, subject, text) {  
    GmailApp.sendEmail(email, subject, text);
    return ['Email sent'];  
}
```

* Then, implement it as a executable API, extract the script ID and paste it on:

```js
var scriptId = "XXXXXXXXXXXXXXXXXXXXXXXXXXXX";
```
####Run
To run, use your favorite server or simply type:
```
python -m SimpleHTTPServer
```

All rights reserved to **[Google](http://www.google.com)**.

*Sorry if my English had mistakes, isn't my first language.*