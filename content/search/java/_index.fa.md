---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: fa
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

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
head_title: "راهکار جستجو و نمایه‌سازی اسناد Java برای PDF ها، فایل‌های آفیس و محتوای وب"
head_description: "قدرت جستجو و نمایه‌سازی متن برای برنامه‌های Java. به آسانی داده‌ها را در PDF، Word، Excel، ارائه‌ها، ایمیل‌ها و فرمت‌های وب جستجو و سازمان‌دهی کنید."

############################# Header ############################
title: "جستجو و نمایه‌سازی مؤثر اسناد با API Java"
description: "برنامه‌های Java را با ویژگی‌های قدرتمند جستجوی متن در تمام فرمت‌های محبوب اسناد تقویت کنید."
words:
  for: "برای"

actions:
  main: "دانلود Maven به صورت رایگان"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-search/"
  alt: "مجوز دهی"
  alt_link: "https://purchase.groupdocs.com/pricing/search/java/"
  title: "سفر خود را امروز آغاز کنید!"
  description: "قابلیت‌های GroupDocs.Search را به صورت رایگان کشف کنید یا یک مجوز برای باز کردن پتانسیل کامل آن دریافت کنید."

release:
  title: "نسخه {0} منتشر شد"
  notes: "ببینید چه چیز جدیدی است"
  downloads: "بارگیری‌ها"

code:
  title: "یافتن متن در فایل‌ها با استفاده از Java"
  more: "نمونه‌های بیشتر"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-search</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // یک نمایه برای اسناد خود ایجاد کنید
    Index index = new Index("c:/MyIndex");

    // اسناد را به نمایه اضافه کنید تا جستاری مؤثر انجام دهید
    index.add("c:/MyDocuments");
    
    // برای جستجوی کلمات یا عبارات خاص، مانند
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "بررسی اجمالی GroupDocs.Search"
  description: "قابلیت‌های قدرتمند جستجوی متن کتابخانه Java Java را کشف کنید."
  features:
    # feature loop
    - title: "عملیات نمایه‌سازی و جستجو در Java"
      content: "با GroupDocs.Search for Java می‌توانید داده‌ها را به طور مؤثر جمع‌آوری، ذخیره و تجزیه و تحلیل کنید تا نمایه‌های دقیقی برای جستجوهای سریعتر و دقیق‌تر ایجاد کنید."

    # feature loop
    - title: "بهینه‌سازی جستجو با ادغام نمایه‌ها"
      content: "با GroupDocs.Search for Java به آسانی چندین نمایه را ترکیب کنید تا جستجوها را ساده کنید. تأثیر نمایه‌های دلتا را با ادغام آنها به یک نمایه با عملکرد بالا کاهش دهید."

    # feature loop
    - title: "پشتیبانی از چیدمان‌های چند زبانه"
      content: "با GroupDocs.Search for Java در زبان‌ها و چیدمان‌های مختلف جستجو کنید. این کتابخانه از 88 زبان و 164 پیکربندی صفحه کلید برای انعطاف‌پذیری بی‌نظیر پشتیبانی می‌کند."

    # feature loop
    - title: "قابلیت‌های جستجوی مورفولوژیکی"
      content: "با GroupDocs.Search for Java به جستجو بر اساس اشکال مختلف کلام مانند اسم‌های مفرد و جمع یا تغییرات فعل بپردازید. گزینه‌های جستجو را برای زبان‌های مختلف سفارشی کنید."

############################# Platforms ############################
platforms:
  enable: true
  title: "استقلال از پلتفرم"
  description: "GroupDocs.Search for Java با سیستم‌عامل‌ها و مدیران بسته اصلی سازگار است."
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "فرمت‌های فایل پشتیبانی شده"
  description: |
    با GroupDocs.Search for Java دامنه وسیعی از فرمت‌های فایل را پردازش کنید. [لیست کامل را مشاهده کنید](https://docs.groupdocs.com/search/java/supported-document-formats/).
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
  title: "ویژگی‌های GroupDocs.Search for Java"
  description: "مدیریت محتویات اسناد را به‌طور مؤثر با قابلیت‌های جستجوی پیشرفته در فرمت‌های PDF، DOCX، XLSX، PPTX و بیشتر انجام دهید."

  items:
    # feature loop
    - icon: "document_info"
      title: "پارامترهای جستجوی قابل تنظیم"
      content: "با استفاده از فیلترهایی مانند بازه‌های تاریخ و حساسیت به حروف، جستجو را محدودتر کنید."

    # feature loop
    - icon: "detect"
      title: "بررسی املایی بهبود یافته"
      content: "با بررسی املایی، کاراکترهای عمومی و با نادیده گرفتن کاراکترهای خاص به‌طور مؤثر جستجو کنید."

    # feature loop
    - icon: "collect"
      title: "نتایج جستجوی فیلتر شده"
      content: "نتایج جستجو را با تمرکز بر روی نوع سند یا معیارهای خاص فیلتر کنید."

    # feature loop
    - icon: "get"
      title: "واردات و صادرات داده‌های نمایه"
      content: "به راحتی داده‌ها را برای نمایه‌سازی وارد کنید یا نتایج را به فایل‌های قابل استفاده صادر کنید."

    # feature loop
    - icon: "remove"
      title: "نادیده گرفتن فایل‌های غیرضروری"
      content: "با نادیده گرفتن فایل‌ها یا کلمات خاص، نمایه‌سازی را بهینه کنید."

    # feature loop
    - icon: "style"
      title: "پردازش HTML و URL"
      content: "محتوای HTML را استخراج کرده و URL هایی برای ناوبری از طریق نتایج جستجو ایجاد کنید."

    # feature loop
    - icon: "detect"
      title: "جستجوی سریع در نمایه‌های بزرگ"
      content: "عملیات جستجو را با تقسیم نمایه‌های بزرگ به بخش‌های قابل مدیریت تسریع کنید."

    # feature loop
    - icon: "manipulate"
      title: "نمایه‌سازی مبتنی بر جریان"
      content: "اطلاعات را به‌طور مستقیم از جریان‌ها یا ساختارهای داده نمایه‌سازی کنید."

    # feature loop
    - icon: "compare"
      title: "مدیریت پرسش‌های اشتباه املایی"
      content: "اشتباهات املایی را تشخیص دهید و برای بهبود دقت جستجو کلمات جایگزین پیشنهاد دهید."

    # feature loop
    - icon: "unreadable_characters"
      title: "پشتیبانی جامع از آرشیو"
      content: "آرشیوهای تو در تو را نمایه‌گذاری کرده و فهرست دقیقی از فایل‌های آن داخل ZIP را بازیابی کنید."

    # feature loop
    - icon: "hidden_print"
      title: "نمایه‌سازی بهینه‌ی فضای دیسک"
      content: "نمایه‌ها را به صورت فشرده حفظ کنید تا فضای دیسک را صرفه‌جویی کرده و فایل‌های محافظت‌شده با کلمه عبور را پردازش کنید."

    # feature loop
    - icon: "style"
      title: "پشتیبانی از مترادف‌های سفارشی"
      content: "دیکشنری مترادف‌ها را گسترش دهید تا دقت جستجو با گزینه‌های سفارشی‌شده افزایش یابد."

############################# Code samples ############################
code_samples:
  enable: true
  title: "نمونه‌های کد"
  description: "به ویژگی‌های GroupDocs.Search for Java با این نمونه‌های کد بپردازید."
  items:
    # code sample loop
    - title: "افزایش دقت جستجو با تطابق نزدیک"
      content: |
        انعطاف‌پذیری GroupDocs.Search for Java را برای مدیریت محتوا با قابلیت‌های پیشرفته جستجوی نزدیک کشف کنید. [بیشتر بیاموزید](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="چگونه نتیجه جستجو را پردازش کنیم">}}
        ```java {style=abap}
        // یک نمایه ایجاد کنید
        Index index = new Index("C:/IndexFolder");
        index.add("C:/DocumentFolder");

        // گزینه‌های جستجو را تنظیم کنید
        SearchOptions options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // به دنبال اسنادی باشید که شامل کلمه 'آب' یا عبارت 'لورم ایپسوم' هستند
        String query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.search(query, options);
        
        // نتیجه جستجو را پردازش کنید
        System.out.println("Documents: " + result.getDocumentCount());
        System.out.println("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            System.out.println("Document: " + document.getDocumentInfo().getFilePath());
            System.out.println("Occurrences " + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "نتایج را با استفاده از عبارات منظم بهبود دهید"
      content: |
        از عبارات منظم در GroupDocs.Search for Java برای ایجاد نتایج دقیق و جزئی استفاده کنید. [تکنیک‌های پیشرفته را کشف کنید](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="چگونه با استفاده از عبارات منظم جستجو کنیم">}}
        ```java {style=abap}   
        // یک نمایه ایجاد کنید
        Index index = new Index("C:/IndexFolder");
        index.add("c:/DocumentFolder");
 
        // عبارت را در فرم متنی جستجو کنید

        // کاراکتر اولیه در ابتدای متن نشان می‌دهد که این یک جستجوی منظم است
        String query = "^^(.)\\1{1,}";
        // به دنبال دو یا چند کاراکتر یکسان در ابتدای یک کلمه جستجو کنید
        SearchResult result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
