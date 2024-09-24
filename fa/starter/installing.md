---
layout: page
title: Installing Express
menu: starter
lang: fa
redirect_from: '/starter/installing.html'
---

# Installing

با فرض اینکه شما از قبل [Node.js](https://nodejs.org/) را نصب کردید، یک دایرکتوری برای اپلیکیشن خود ایجاد کنید و آن را به عنوان دایرکتوری فعلی خود قرار دهید.

- [Express 4.x](/{{ page.lang }}/4x/api.html) نیاز به Node.js ۰.۱۰ یا بالاتر دارد.
- [Express 5.x](/{{ page.lang }}/5x/api.html) نیاز به Node.js ۱۸ یا بالاتر دارد.

```console
$ mkdir myapp
$ cd myapp
```

از کامند `npm init` برای ایجاد کردن `package.json` برای اپلیکیشن خود استفاده کنید.
برای اطلاعات بیشتر درباره اینکه چگونه `package.json` کار می‌کند، [جزئیات تنظیمات package.json در NPM](https://docs.npmjs.com/files/package.json).

```console
$ npm init
```

این کامند به شما برای چیز‌هایی مانند اسم و ورژن اپلیکیشن شما پیام می‌دهد.
فعلا شما می‌توانید با زدن دکمه RETURN بیش‌تر پیش‌فرض‌ها را قبول کنید، غیر از این‌ها:

```
entry point: (index.js)
```

`app.js` یا هرچیزی که به عنوان اسم فایل اصلی شما باشد را وارد کنید. اگر می‌خواهید اسم فایل اصلی شما `index.js` باشد، RETURN را فشار دهید تا پیش‌فرض های پیشنهادی را قبول کنید

حالا اکسپرس را در دایرکتوری `myapp` نصب کنید و آن را در لیست dependency‌ها ذخیره کنید. برای مثال:

```console
$ npm install express
```

برای نصب کردن موقتی اکسپرس و اضافه نکردن آن به لیست dependency‌ها:

```console
$ npm install express --no-save
```

<div class="doc-box doc-info" markdown="1">

به طور پیش‌فرض، با ورژن بالاتر از ۵.۰، `npm install` ماژول را در لیست ‌`dependency`های `package.json` اضافه می‌کند. با ورژن های قبلی NPM، شما باید گزینه `--save` را صریحا وارد کنید. بعد از آن، اجرا کردن `npm install` در دایرکتوری اپلیکیشن به طور خودکار ماژول‌ها را در لیست dependency نصب می‌کند.

</div>

### [بعدی: سلام جهان ](/{{ page.lang }}/starter/hello-world.html)
