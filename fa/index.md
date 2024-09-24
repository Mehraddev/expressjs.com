---
layout: home
title: Express - Node.js web application framework
menu: home
lang: fa
redirect_from: '/en/index.html'
---

<section id="home-content">
  {% include header/header-{{ page.lang }}.html %}
  <div id="overlay"></div>
  <div id="homepage-leftpane" class="pane">
    <section id="description">
        <div class="express"><a href="/">Express</a><a href="{{ page.lang }}/changelog/4x.html#{{ site.data.express.current_version }}" id="express-version">{{ site.data.express.current_version }}</a></div>
        <span class="description">فریمورک سریع، انعطاف‌پذیر و مینیمالیست برای<a href='https://nodejs.org/en/'>Node.js</a></span>
    </section>
    <div id="install-command">$ npm install express --save</div>
  </div>
</section>
<section id="announcements">
  {% include announcement/announcement-en.md %}
</section>

<section id="intro">

  <div id="boxes" class="clearfix">
    <div id="web-applications">
      <h3>وب اپلیکیشن‌ها</h3> اکسپرس یک فریمورک مینیمال و انعطاف‌پذیر اپلیکیشن‌های وب است که مجموعه‌ای از ویژگی‌های قدرتمند برای اپلیکیشن‌های وب ارائه می‌دهد.
    </div>

    <div id="apis">
      <h3>API‌ها</h3>  با تعداد بسیار زیاد متد های HTTP و middleware در دسترس شما، ایجاد کردن APIهای قدرتمند سریع و راحت است.
    </div>

    <div id="performance">
      <h3>عملکرد</h3> اکسپرس لایه نازکی از ویژگی‌های اساسی اپلیکیشن‌های وب را بدون از بین بردن ویژگی‌های Node.js که شما می‌دانید و دوست دارید ارئه می‌دهد.
    </div>

    <div id="middleware">
      <h3>Middleware</h3>
      اکسپرس فریمورک یک فریمورک routing سبک و انعطاف‌پذیر است با ویژگی‌های سبک و اساسی‌ که برای تکمیل کردن استفاده از اکسپرس تعبیه شده است. <a href="{{ page.lang }}/resources/middleware.html">middleware</a> modules.
    </div>

  </div>

</section>
