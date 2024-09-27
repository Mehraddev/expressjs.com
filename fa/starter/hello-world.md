---
layout: page
title: Express "Hello World" example
menu: starter
lang: fa
redirect_from: '/starter/hello-world.html'
---

# Hello world example

<div class="doc-box doc-info" markdown="1">
کد زیر اساسا ساده‌ترین اپلیکیشن Express است که می‌توانید بسازید. این یک اپلیکیشن تک فایلی است &mdash; نه چیزی که از Express generator می‌گیرید که یک اپلیکیشن کامل با فایل‌های بی‌شمار جاوااسکریپت، Jade template ها، و ساب دایرکتوری‌ها با هدف های مختلف می‌سازد.
</div>

<script src="https://embed.runkit.com" data-element-id="hello-example" data-mode="endpoint" async defer></script>
<div id="hello-example"><pre><code class="language-js">
const express = require('express')
const app = express()
const port = 3000

app.get('/', (req, res) => {
res.send('Hello World!')
})

app.listen(port, () => {
console.log(`Example app listening on port ${port}`)
})
</code></pre></div>

ین اپلیکیشن با یک سرور استارت می‌شود و برای اتصالات به پورت ۳۰۰۰ گوش می‌دهد. این اپلیکیشن به ریکوئست‌های آدرس (`/`) یا روت با "Hello World!" پاسخ می‌دهد. برای بقیه ریکوئست‌ها با ارور **404 Not Found** پاسخ می‌دهد.

مثال بالا درواقع یک سرور در حال کار است: روی آدرس نشان داده شده کلیک کنید. یک پاسخ با لاگ‌های لحظه‌ای می‌گیرید، و هر تغییری که ایجاد می‌کنید در لحظه نمایش داده می‌شود. این قابلیت به وسیله [RunKit](https://runkit.com) ارائه شده است که یک playground جاوااسکریپت ارائه می‌دهد که به یک محیط کامل Node که روی مرورگر شما اجرا می‌شود، متصل شده است.
پایین، راهنمایی است برای اجرا کردن همین اپلیکیشن روی کامپیوتر خودتان.

<div class="doc-box doc-info" markdown="1">
RunKit یک سرویس ثالث است که به پروژه Express ربطی ندارد.</div>

### Running Locally

اول، یک دایرکتوری با نام `myapp` ایجاد کنید، وارد آن شوید و `npm init` را اجرا کنید. سپس، `express` را به عنوان dependency نصب کنید، همانطور که در [راهنمای نصب](/{{ page.lang }}/starter/installing.html) اشاره شده است.

در دایرکتوری `myapp` یک فایل با نام `app.js` ایجاد کنید و سپس کد مثال بالا را در آن کپی کنید.

<div class="doc-box doc-notice" markdown="1">
`req` (درخواست) و `res` (پاسخ) دقیقاا همان آبجکت‌هایی هستند که Node ارائه می‌دهد، پس شما می‌توانید `req.pipe()`, `req.on('data', callback)` و هرچیز دیگر که بدون Express انجام می‌داید را فراخوانی کنید.
</div>

اپلیکیشن را با دستور زیر اجرا کنید:

```console
$ node app.js
```

سپس `http://localhost:3000/` را در مرورگر باز کنید تا نتایج را ببینید.

### [قبلی: نصب کردن ](/{{ page.lang }}/starter/installing.html)&nbsp;&nbsp;&nbsp;&nbsp;[بعدی: Express generator ](/{{ page.lang }}/starter/generator.html)
