---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: fa
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "کتابخانه جستجو و نمایه‌سازی متن Node.js برای اسناد، PDF، آفیس و وب"
head_description: "راه‌حل پیشرفته جستجوی متن برای برنامه‌های Node.js برای جستجو، نمایه‌سازی و جمع آوری داده‌ها از اسناد: PDF، Word، Excel، ارائه‌ها، ایمیل و فرمت‌های فایل وب."

############################# Header ############################
title: "جستجو و نمایه‌سازی اسناد با استفاده از API Node.js"
description: "برنامه‌های Node.js را با پیاده‌سازی جستجوی متن در تمامی فرمت‌های محبوب اسناد تقویت کنید."
words:
  for: "برای"

actions:
  main: "دانلود رایگان NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "مجوز دهی"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "سفر خود را امروز آغاز کنید!"
  description: "قابلیت‌های GroupDocs.Search را به صورت رایگان کشف کنید یا یک مجوز برای باز کردن پتانسیل کامل آن دریافت کنید."

release:
  title: "نسخه {0} منتشر شد"
  notes: "ببینید چه چیز جدیدی است"
  downloads: "بارگیری‌ها"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "جستجوی متن در یک پوشه با JavaScript"
  more: "نمونه‌های بیشتر"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    const searchLib = require('@groupdocs/groupdocs.search');

    // یک نمایه برای اسناد خود ایجاد کنید
    const index = new searchLib.Index('c:/MyIndex');

    // اسناد را به نمایه اضافه کنید تا جستاری مؤثر انجام دهید
    index.add('c:/MyDocuments');
    
    // برای جستجوی کلمات یا عبارات خاص، مانند
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "بررسی اجمالی GroupDocs.Search"
  description: "کتابخانه Node.js JavaScript برای جستجوی متن"
  features:
    # feature loop
    - title: "Node.js عملیات نمایه‌سازی و جستجو"
      content: "نمایه‌سازی در GroupDocs.Search for Node.js via Java داده‌ها را برای عملیات جستجوی دقیق و مؤثر جمع‌آوری، ذخیره و تجزیه و تحلیل می‌کند. این نمایه‌ها معمولاً برای انجام جستجوها استفاده می‌شوند."

    # feature loop
    - title: "ادغام نمایه‌ها برای افزایش کارآیی جستجو"
      content: "GroupDocs.Search for Node.js via Java API اجازه می‌دهد تا چندین نمایه را به یک نمایه ادغام کنید. اصلاحات مکرر نمایه‌های دلتا ایجاد می‌کند که می‌تواند عملکرد جستجو را کند کند. راه‌حل ما این نمایه‌های دلتا را به یک نمایه عمومی ادغام می‌کند که تمام اطلاعات از نمایه‌های دلتا ادغام شده را در بر می‌گیرد و کارآیی جستجو را بهبود می‌بخشد در حالی که نمایه‌های دلتا بدون تغییر باقی می‌مانند. قابلیت‌های مختلفی می‌توانند برای تنظیم این فرآیند پیکربندی شوند."

    # feature loop
    - title: "تشخیص جستجو از چیدمان‌های مختلف صفحه کلید"
      content: "GroupDocs.Search for Node.js via Java پرسش‌های جستجو را که با چیدمان صفحه کلید مطابقت ندارد، تشخیص می‌دهد. در حال حاضر، 88 زبان و 164 چیدمان صفحه کلید مختلف پشتیبانی می‌شوند."

    # feature loop
    - title: "جستجو با استفاده از اشکال کلامی مورفولوژیکی"
      content: "با GroupDocs.Search for Node.js via Java می‌توانید به جستجوی اشکال مختلف کلمه، مانند اسم‌های مفرد و جمع، یا تمام اشکال یک فعل بپردازید. زبان‌های انگلیسی و غیر انگلیسی می‌توانند برای اشکال خاص کلمه تنظیم شوند."

############################# Platforms ############################
platforms:
  enable: true
  title: "استقلال از پلتفرم"
  description: "GroupDocs.Search for Node.js via Java همه سیستم‌عامل‌های محبوب و مدیران بسته‌ها را پشتیبانی می‌کند."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "فرمت‌های فایل پشتیبانی شده"
  description: |
    GroupDocs.Search for Node.js via Java برای پردازش دامنه وسیعی از فرمت‌های فایل ارائه می‌شود. [لیست کامل را مشاهده کنید](https://docs.groupdocs.com/search/nodejs-java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### فرمت‌های محبوب آفیس
        * **قابل حمل:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **متن:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### فرمت‌های رسانه‌ای
        * **فرمت‌های تصویر محبوب:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **تصاویر چند صفحه‌ای:** GIF, WEBP, TIFF
        * **صوتی:** MP3, WAV
        * **ویدئو:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### سایر
        * **ایمیل:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **وب:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **سایر:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "ویژگی‌های GroupDocs.Search for Node.js via Java"
  description: "محتوای اسناد تجاری را با استفاده از موتور جستجوی پیشرفته ما کنترل کنید که از فرمت‌های محبوب شامل PDF، DOCX، XLSX، PPTX و بیشتر پشتیبانی می‌کند."

  items:
    # feature loop
    - icon: "document_info"
      title: "پارامترهای قابل تنظیم"
      content: "از محدوده تاریخ و حساسیت به حروف به عنوان پارامترهای جستجو استفاده کنید."

    # feature loop
    - icon: "detect"
      title: "جستجوی املایی"
      content: "عبارت‌های جستجو را با تصحیح املایی و کاراکترهای نادیده و کاراکترهای خاص در حفظ جستجو استفاده کنید."

    # feature loop
    - icon: "collect"
      title: "فیلتر کردن نتایج"
      content: "فقط نتایج مورد نظر را با تنظیم فیلتر اسناد در نتایج جستجو مشخص کنید."

    # feature loop
    - icon: "get"
      title: "واردات و صادرات"
      content: "وارد کردن یا استفاده از لیست برای تغییر کارکترها در طول نمایه‌سازی و صادرات به یک فایل."

    # feature loop
    - icon: "remove"
      title: "نادیده گرفتن داده‌های غیرضروری"
      content: "به طور انتخابی نمایه‌سازی را برای فایل‌های خاص نادیده گرفته و کلمات خاص را برای نمایه‌سازی سریع‌تر جا بیندازید."

    # feature loop
    - icon: "style"
      title: "پردازشURL"
      content: "محتوای HTML را به یک فایل استخراج کنید و URL‌ها را برای ناوبری از نتایج جستجو ایجاد کنید."

    # feature loop
    - icon: "detect"
      title: "جستجوی سریع"
      content: "عملیات جستجو را با تقسیم بر روی قسمت‌های کوچکتر، سرعت جستجوی بزرگ را افزایش دهید."

    # feature loop
    - icon: "manipulate"
      title: "پردازش جریانی"
      content: "اسناد را از جریانات و ساختار داده‌ها نمایه‌سازی کنید."

    # feature loop
    - icon: "compare"
      title: "مدیریت خطاهای املایی"
      content: "تعداد دقیق وقوع هر کلمه‌ی یافت شده را فعال کنید تا پیشنهاد کلمات جایگزین در صورت اشتباه املایی ارائه دهد."

    # feature loop
    - icon: "unreadable_characters"
      title: "پشتیبانی آرشیو"
      content: "آرشیوهای فشرده را در آرشیوهای ZIP نمایه‌سازی کنید و فهرست فایل‌های نمایه‌گذاری شده در یک آرشیو را بازیابی کنید."

    # feature loop
    - icon: "hidden_print"
      title: "صرفه‌جویی در فضای دیسک"
      content: "با نمایه‌سازی فشرده، فضای ذخیره‌سازی را ذخیره کنید و فایل‌های محافظت‌شده با کلمه عبور را نمایه‌سازی کنید."

    # feature loop
    - icon: "style"
      title: "مترادف‌های سفارشی"
      content: "مترادف‌های انگلیسی را به دیکشنری مترادف پیش‌فرض اضافه کنید."

############################# Code samples ############################
code_samples:
  enable: true
  title: "نمونه‌های کد"
  description: "ویژگی‌های GroupDocs.Search for Node.js via Java را با این مثال‌های کدی امتحان کنید."
  items:
    # code sample loop
    - title: "افزایش دقت جستجو با استفاده از تطابق نزدیک"
      content: |
        از عملکرد انعطاف‌پذیر GroupDocs.Search for Node.js via Java برای کنترل محتوای اسناد با قابلیت‌های پیشرفته جستجوی نزدیک بهره‌مند شوید. [بیشتر بیاموزید](https://docs.groupdocs.com/search/nodejs-java/search-results/).
        {{< landing/code title="چگونه نتیجه جستجو را پردازش کنیم">}}
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search');

        // یک نمایه ایجاد کنید
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // گزینه‌های جستجو را تنظیم کنید
        const options = new searchLib.SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // به دنبال اسنادی باشید که شامل کلمه 'آب' یا عبارت 'لورم ایپسوم' هستند
        const query = 'water OR "Lorem ipsum"';
        const result = index.search(query, options);
        
        // نتیجه جستجو را پردازش کنید
        console.log('Documents: ' + result.getDocumentCount());
        console.log('Total occurrences: ' + result.getOccurrenceCount());
        for (let i = 0; i < result.getDocumentCount(); i++) {
            const document = result.getFoundDocument(i);
            console.log('Document: ' + document.getDocumentInfo().getFilePath());
            console.log('Occurrences:  + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "از عبارات منظم برای جستجوهای دقیق و جزئی استفاده کنید"
      content: |
        GroupDocs.Search for Node.js via Java امکان استفاده از عبارات منظم را برای دقیق‌تر کردن جستجوها فراهم می‌کند. [تکنیک‌های پیشرفته را کشف کنید](https://docs.groupdocs.com/search/nodejs-java/regular-expression-search/).
        {{< landing/code title="چگونه با استفاده از عبارات منظم جستجو کنیم">}}
        ```javascript {style=abap}   
        const searchLib = require('@groupdocs/groupdocs.search');

        // یک نمایه ایجاد کنید
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // عبارت را در فرم متنی جستجو کنید

        // کاراکتر اولیه در ابتدای متن نشان می‌دهد که این یک جستجوی منظم است
        const query = '^^(.)\\1{1,}';
        // به دنبال دو یا چند کاراکتر یکسان در ابتدای یک کلمه جستجو کنید
        const result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
