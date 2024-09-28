---
layout: page
title: Express application generator
menu: starter
lang: fa
redirect_from: '/starter/generator.html'
---

# [جنریتور اپلیکیشن Express]

از جنریتور اپلیکیشن اکسپرس، `express-generator`، برای ساختن سریع اسکلت یک اپلیکیشن استفاده کنید.

شما می‌توانید با دستور `npx`، جنریتور اپلیشکیشن را اجرا کنید (در دسترس در ورژن ۸.۲.۰ Node.js)

```console
$ npx express-generator
```

برای ورژن های قبلی Node، جنریتور اپلیکیشن را به عنوان پکیج گلوبال `npm` نصب کنید.

```console
$ npm install -g express-generator
$ express
```

با گزینه `-h`، گزینه‌های(آپشن‌های) دستور را نمایش دهید:

```console
$ express -h

  Usage: express [options] [dir]

  Options:

    -h, --help          output usage information
        --version       output the version number
    -e, --ejs           add ejs engine support
        --hbs           add handlebars engine support
        --pug           add pug engine support
    -H, --hogan         add hogan.js engine support
        --no-view       generate without view engine
    -v, --view <engine> add view <engine> support (ejs|hbs|hjs|jade|pug|twig|vash) (defaults to jade)
    -c, --css <engine>  add stylesheet <engine> support (less|stylus|compass|sass) (defaults to plain css)
        --git           add .gitignore
    -f, --force         force on non-empty directory
```

برای مثال، کد پایین یک اپلیکیشن اکسپرس با نام _myapp_ می‌سازد. این اپلیشکین در فولدری با نام _myapp_ در دایرکتوری فعلی ساخته خواهد شد و <a href="https://pugjs.org/" target="_blank" title="Pug documentation">Pug</a>، view engine خواهد بود.

```console
$ express --view=pug myapp

   create : myapp
   create : myapp/package.json
   create : myapp/app.js
   create : myapp/public
   create : myapp/public/javascripts
   create : myapp/public/images
   create : myapp/routes
   create : myapp/routes/index.js
   create : myapp/routes/users.js
   create : myapp/public/stylesheets
   create : myapp/public/stylesheets/style.css
   create : myapp/views
   create : myapp/views/index.pug
   create : myapp/views/layout.pug
   create : myapp/views/error.pug
   create : myapp/bin
   create : myapp/bin/www
```

سپس dependency ها را نصب کنید:

```console
$ cd myapp
$ npm install
```

در MacOS یا Linux اپلیکیشن را با این دستور اجرا کنید:

```console
$ DEBUG=myapp:* npm start
```

در کامند پرامت ویندوز، از این کامند استفاده کنید:

```console
> set DEBUG=myapp:* & npm start
```

در PowerShell ویندوز، از این دستور استفاده کنید:

```console
PS> $env:DEBUG='myapp:*'; npm start
```

سپس `http://localhost:3000/` را در مرورگرتان باز کنید تا به اپلیکیشن دسترسی پیدا کنید:

اپلیکیشن ایجاد شده ساختار دایرکتوری‌ای به این شکل خواهد داشت:

```console
.
├── app.js
├── bin
│   └── www
├── package.json
├── public
│   ├── images
│   ├── javascripts
│   └── stylesheets
│       └── style.css
├── routes
│   ├── index.js
│   └── users.js
└── views
    ├── error.pug
    ├── index.pug
    └── layout.pug

7 directories, 9 files
```

<div class="doc-box doc-info" markdown="1">
ساختار اپلیکیشن ایجاد شده توسط جنریتور، یک نمونه از نمونه‌های زیادی است که برای ساختار دادن به پروژه‌ها استفاده میشود. در صورت تمایل می‌توانید این ساختار را تغییر دهید تا به بهترین حالت ممکن نیاز‌های پروژه‌تان را رفع کنید.
</div>

### [قبلی: سلام جهان ](/{{ page.lang }}/starter/hello-world.html)&nbsp;&nbsp;&nbsp;&nbsp;[بعدی: مسیریابی ساده](/{{ page.lang }}/starter/basic-routing.html)
