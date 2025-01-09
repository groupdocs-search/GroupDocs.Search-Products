---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: fa
product: "Search"
product_tag: "search"
platform: "Net"
platform_tag: "net"

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
head_title: "کتابخانه جستجو و نمایه‌سازی اسناد .NET برای PDF ها، فایل‌های آفیس و بیشتر"
head_description: "راهکار قدرتمند .NET برای جستجو و نمایه‌سازی متن در اسناد مانند PDF، Word، Excel، ارائه‌ها، ایمیل‌ها و فرمت‌های وب."

############################# Header ############################
title: "جستجو و نمایه‌سازی پیشرفته اسناد با API .NET"
description: "برنامه‌های .NET را با قابلیت‌های پیشرفته جستجوی متن در فرمت‌های محبوب رفع ویرایش کنید."
words:
  for: "برای"

actions:
  main: "دانلود Nuget به صورت رایگان"
  main_link: "https://www.nuget.org/packages/GroupDocs.Search"
  alt: "مجوز دهی"
  alt_link: "https://purchase.groupdocs.com/pricing/search/net/"
  title: "سفر خود را امروز آغاز کنید!"
  description: "قابلیت‌های GroupDocs.Search را به صورت رایگان کشف کنید یا یک مجوز برای باز کردن پتانسیل کامل آن دریافت کنید."

release:
  title: "نسخه {0} منتشر شد"
  notes: "ببینید چه چیز جدیدی است"
  downloads: "بارگیری‌ها"

code:
  title: "جستجوی متن در پرونده‌های دایرکتوری"
  more: "نمونه‌های بیشتر"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
  install: "dotnet add package GroupDocs.Search"
  content: |
    ```csharp {style=abap}   
    // یک نمایه برای اسناد خود ایجاد کنید
    Index index = new Index("c:/MyIndex");

    // اسناد را به نمایه اضافه کنید تا جستاری مؤثر انجام دهید
    index.Add("c:/MyDocuments");
    
    // برای جستجوی کلمات یا عبارات خاص، مانند
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.Search("'"?ffect & princip?(2~4)"'");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "بررسی اجمالی GroupDocs.Search"
  description: "کتابخانه .NET C# برای جستجوی مؤثر متن و نمایه‌سازی."
  features:
    # feature loop
    - title: "ویژگی‌های نمایه‌سازی و جستجو در .NET"
      content: "با GroupDocs.Search for .NET داده‌های اسنادی را به شکل مؤثر نمایه‌سازی، ذخیره و پردازش کنید تا عملیات جست‌وجو با دقت و سرعت بالا داشته باشید."

    # feature loop
    - title: "ترکیب نمایه‌ها برای بهبود سرعت جستجو"
      content: "GroupDocs.Search for .NET به شما اجازه می‌دهد چندین نمایه را ادغام کنید تا عملکرد بهینه‌تری داشته باشید. تأثیر نمایه‌های دلتا را با ادغام آنها به یک نمایه جامع کاهش دهید تا جستجوها بهبود یابند."

    # feature loop
    - title: "جستجو در میان چیدمان‌های صفحه کلید مختلف"
      content: "سوالات جستجو را در 88 زبان و 164 چیدمان صفحه کلید به آسانی با تشخیص هوشمند GroupDocs.Search for .NET مدیریت کنید."

    # feature loop
    - title: "جستجوهای کلامی مورفولوژیکی"
      content: "GroupDocs.Search for .NET از جستجوی تغییرات کلامی مانند اسم‌های مفرد/جمع و اشکال مختلف فعل پشتیبانی می‌کند که قابل شخصی‌سازی برای زبان‌های مختلف هستند."

############################# Platforms ############################
platforms:
  enable: true
  title: "استقلال از پلتفرم"
  description: "GroupDocs.Search for .NET به طور یکپارچه در سیستم‌عامل‌ها و مدیران بسته اصلی کار می‌کند."
  items:
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
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "فرمت‌های فایل پشتیبانی شده"
  description: |
    با GroupDocs.Search for .NET دامنه وسیعی از فرمت‌های فایل را پردازش کنید. [تمام فرمت‌های پشتیبانی شده را مشاهده کنید](https://docs.groupdocs.com/search/net/supported-document-formats/).
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
  title: "ویژگی‌های کلیدی GroupDocs.Search for .NET"
  description: "مدیریت سند را با قابلیت‌های پیشرفته جستجو در فرمت‌های محبوب مانند PDF، DOCX، XLSX، PPTX و بیشتر ساده کنید."

  items:
    # feature loop
    - icon: "document_info"
      title: "پارامترهای جستجوی قابل تنظیم"
      content: "از فیلترهایی مانند بازه‌های زمانی و حساسیت به حروف برای تصحیح جستجو استفاده کنید."

    # feature loop
    - icon: "detect"
      title: "از بررسی املایی هوشمند بهره‌مند شوید"
      content: "عبارات جستجو را با تصحیح املایی، کاراکترهای عمومی و کاراکترهای خاص نادیده گرفته شده جستجو کنید."

    # feature loop
    - icon: "collect"
      title: "نتایج جستجوی فیلتر شده"
      content: "نتایج جستجو را با توجه به نوع سند یا معیارهای مشخص شده فیلتر کرده و سفارشی کنید."

    # feature loop
    - icon: "get"
      title: "واردات و صادرات نمایه"
      content: "داده‌ها را وارد، تنظیمات نمایه‌گذاری را اصلاح کرده و نتایج نمایه‌گذاری شده را صادر کنید."

    # feature loop
    - icon: "remove"
      title: "داده‌های نامربوط را نادیده بگیرید"
      content: "با نادیده گرفتن فایل‌ها یا کلمات خاص، نمایه‌سازی را بهینه کنید."

    # feature loop
    - icon: "style"
      title: "استخراج URL"
      content: "متن فرمت HTML را به فایل تبدیل کرده و لینک‌هایی برای نتایج جستجو ایجاد کنید."

    # feature loop
    - icon: "detect"
      title: "جستجویی با سرعت بالا"
      content: "نمایه‌های بزرگ را به بخش‌های کوچک‌تر تقسیم کنید تا پردازش سریع‌تری داشته باشید."

    # feature loop
    - icon: "manipulate"
      title: "مدیریت داده‌های ساده‌سازی شده"
      content: "اسناد را به طور مستقیم از جریان‌های داده و ساختارها نمایه‌سازی کنید."

    # feature loop
    - icon: "compare"
      title: "تشخیص اشتباهات املایی"
      content: "برای بهبود دقت پیشنهادهایی برای کلمات جایگزین و پیگیری رخدادها ارائه دهید."

    # feature loop
    - icon: "unreadable_characters"
      title: "پشتیبانی از آرشیو"
      content: "نزدیک‌ترین فایل‌ها درون آرشیوهای ZIP تو در تو را نمایه‌سازی کنید و جزئیات فایل‌ها درون آن‌ها را بازیابی کنید."

    # feature loop
    - icon: "hidden_print"
      title: "نمایه‌سازی مؤثر"
      content: "با نمایه‌سازی فشرده، فضای دیسک را صرفه‌جویی کنید و اسناد محافظت‌شده با کلمه عبور را پردازش کنید."

    # feature loop
    - icon: "style"
      title: "مترادف‌های سفارشی"
      content: "مترادف‌ها را اضافه و مدیریت کنید تا نتایج جستجوی سفارشی‌سازی‌شده‌ای ارائه دهید."

############################# Code samples ############################
code_samples:
  enable: true
  title: "نمونه‌های کد"
  description: "قابلیت‌های قدرتمند GroupDocs.Search for .NET را با نمونه‌های عملی کشف کنید."
  items:
    # code sample loop
    - title: "افزایش بهره‌وری با جستجوی نزدیک"
      content: |
        از GroupDocs.Search for .NET برای کنترل محتوای انعطاف‌پذیر و دقیق از طریق الگوریتم‌های جستجوی پیشرفته استفاده کنید. [بیشتر بیاموزید](https://docs.groupdocs.com/search/net/search-results/).
        {{< landing/code title="چگونه نتیجه جستجو را پردازش کنیم">}}
        ```csharp {style=abap}
        // یک نمایه ایجاد کنید
        Index index = new Index("C:/IndexFolder");
        index.Add("C:/DocumentFolder");

        // گزینه‌های جستجو را تنظیم کنید
        SearchOptions options = new SearchOptions();
        options.FuzzySearch.Enabled = true;
        options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3);

        // به دنبال اسنادی باشید که شامل کلمه 'آب' یا عبارت 'لورم ایپسوم' هستند
        string query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.Search(query, options);
        
        // نتیجه جستجو را پردازش کنید
        Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
        Console.WriteLine("Occurrences: " + document.OccurrenceCount);
        for (int i = 0; i < result.DocumentCount; i++) {
            FoundDocument document = result.GetFoundDocument(i);
            Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
            Console.WriteLine("Occurrences: " + document.OccurrenceCount);
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "جستجوی پیشرفته با استفاده از عبارات منظم"
      content: |
        GroupDocs.Search for .NET از عبارات منظم برای جستجوهای دقیق پشتیبانی می‌کند. [تکنیک‌های پیشرفته را بیاموزید](https://docs.groupdocs.com/search/net/regular-expression-search/).
        {{< landing/code title="چگونه با استفاده از عبارات منظم جستجو کنیم">}}
        ```csharp {style=abap}   
        // یک نمایه ایجاد کنید
        Index index = new Index("c:/IndexFolder");
        index.Add("c:/DocumentFolder");
 
        // عبارت را در فرم متنی جستجو کنید

        // کاراکتر اولیه در ابتدای متن نشان می‌دهد که این یک جستجوی منظم است
        string query = "^^(.)\\1{1,}";
        // به دنبال دو یا چند کاراکتر یکسان در ابتدای یک کلمه جستجو کنید
        SearchResult result = index.Search(query);
 
        ```
        {{< /landing/code >}}

---
