
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:46
draft: false
lang: fa
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "جستجوی بولی TXT از طریق Node.js"
head_description: "با استفاده از API GroupDocs.Search for Node.js via Java به اجرای جستجوهای پیشرفته در محتوای اسناد با استفاده از عملگرهای بولی مانند AND، OR و NOT بپردازید، که برای توسعه‌دهندگان JavaScript بهینه‌سازی شده است."

############################# Header ############################
title: "انجام جستجوهای منطقی بولی" 
description: "با GroupDocs.Search for Node.js via Java می‌توانید به سادگی جستجوهای پیشرفته‌ای را با استفاده از عملگرهای بولی (AND، OR، NOT) در محیط Node.js خود ایجاد کنید."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "هم‌اکنون دانلود کنید"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search چیست؟"
    link: "/search/nodejs-java/"
    link_title: "بیشتر بیاموزید"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) ابزاری قدرتمند برای جستجو و نمایه‌سازی متن درون اسناد است. این ابزار از بیش از 70 فرمت مانند PDF، Word، Excel، PowerPoint، تصاویر و فایل‌های ZIP پشتیبانی می‌کند و به طور مؤثر پردازش اطلاعات زیاد را تسهیل می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه در اسناد TXT جستجو کنیم با استفاده از عملگرهای بولی"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) به شما اجازه می‌دهد به طور موثر در فایل‌های TXT جستجو کنید. با منطق بولی، می‌توانید جستجوهای خود را در برنامه‌های Node.js via Java برای دقت بهتر تنظیم کنید.
      
      1. پوشه‌ای را برای ذخیره نمایه جستجو تنظیم کنید.
      2. پوشه حاوی فایل‌های TXT برای جستجو را انتخاب کنید.
      3. پرسش جستجو را اجرا کرده و نتایج را بازیابی کنید.
      4. نتایج جستجو را پردازش و تحلیل کنید.
   
    code:
      platform: "nodejs-java"
      copy_title: "کپی"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "نتیجه جستجو"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "برای کپی کلیک کنید"
        copy_done: "کپی شد"
      links:
        #  loop
        - title: "مثال‌های بیشتر"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "مستندات"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // محل ذخیره‌سازی پوشه نمایه را تنظیم کنید
        const index = new searchLib.Index("c:/MyIndex");

        // پوشه‌ای که شامل اسنادی برای جستجو است را مشخص کنید
        index.add("c:/MyDocuments");

        // یک جستجوی پیشرفته را با منطق ایجاد کنید
        const result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ابزارهای قدرتمند برای جستجو و نمایه‌سازی اسناد"
  description: "GroupDocs.Search for Node.js via Java جستجو و نمایه‌سازی متن را برای بیش از 70 نوع پرونده ساده می‌کند و به شما کمک می‌کند اطلاعات را سریع‌تر و با دقت بیشتری پیدا و مدیریت کنید."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Search"
  features:
    # feature loop
    - title: "جستجوی متن پیشرفته"
      content: "متن را به سرعت در فرمت‌های مختلف مانند PDF، اسناد Word، ارائه‌ها و صفحات گسترده پیدا کنید. از ویژگی‌هایی همچون تطبیق دقیق، جستجوهای wildcard، و جستجوی نادقیق برای نتایج دقیق استفاده کنید."

    # feature loop
    - title: "نمایه‌سازی کارآمد داده‌ها"
      content: "شاخص‌ها را بسازید و مدیریت کنید تا جستجوها در مجموعه‌های بزرگ اسناد سریع‌تر انجام شود. نمایه‌سازی دسترسی سریع و ساختار یافته به داده‌های شما را تضمین می‌کند."

    # feature loop
    - title: "پشتیبانی چند زبانه"
      content: "در اسنادی که به بیش از 80 زبان نوشته شده‌اند جستجو کنید. پشتیبانی از شکل‌های دستوری و سازگاری با چیدمان کیبورد، نتایج جستجو را در زبان‌های مختلف بهبود می‌بخشد."

    # feature loop
    - title: "تنظیمات جستجوی انعطاف‌پذیر"
      content: "جستجوی خود را با فعال‌سازی حساسیت به حروف بزرگ و کوچک، اعمال فیلترهای تاریخ، یا نادیده‌گرفتن کلمات و داده‌های خاص در طول نمایه‌سازی سفارشی کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "مثالی از جستجوی بولی پیشرفته"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توان پرسش‌های مبتنی بر بولی را برای جستجوی محتوا در اسناد TXT ایجاد کرد.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // پوشه‌ای را برای نمایه جستجو تعریف کنید
          const index = new searchLib.Index("c:/MyIndex");
              
          // محل اسناد برای جستجو را مشخص کنید
          index.add("c:/MyDocuments");

          // یک پرسش را با استفاده از عملگرهای بولی بسازید
          const wordQuery1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wordQuery2 = searchLib.SearchQuery.createWordQuery("ipsum");
          const booleanQuery = searchLib.SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // نتایج جستجو را بازیابی کنید
          const result = index.search(booleanQuery);
          
          // نتایج جستجو را پردازش و استفاده کنید
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "کپی"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "برای کپی کلیک کنید"
          copy_done: "کپی شد"
        top_links:
          #  loop
          - title: "دانلود نتیجه"
            icon: "download"
            link: "/examples/search/formats/searchboolean.txt"
        links:
          #  loop
          - title: "مثال‌های بیشتر"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "مستندات"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "آماده شروع هستید؟"
  description: "ویژگی‌های GroupDocs.Search را رایگان امتحان کنید یا درخواست مجوز دهید"
  items:
    #  loop
    - title: "دانلود NPM"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "مجوزدهی"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "قابلیت‌های کلیدی GroupDocs.Search"
    exclude: "boolean"
    description: "ویژگی‌های جستجوی پیشرفته، کارآمد و قابل تنظیم را باز کنید."
    items: 
          
        # operation loop 1
        - name: "جستجو با شرط"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "یافتن اطلاعات در اسناد با استفاده از شرایط بولی"

        # operation loop 2
        - name: "جستجوی حساس به حروف بزرگ و کوچک"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "دقت جستجو را با در نظر گرفتن حساسیت حروف افزایش دهید"

        # operation loop 3
        - name: "شاخص‌گذاری اسناد"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "اسناد را یک‌بار شاخص‌گذاری کنید و از شاخص برای جستجوهای متعدد استفاده کنید"

        # operation loop 4
        - name: "فیلترهای جستجو"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "از فیلترها برای محدود کردن داده‌های پردازش‌شده استفاده کنید"

        # operation loop 5
        - name: "عبارت دقیق"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "جستجو برای یک جمله یا عبارت خاص"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "جستجوی فرمت‌های محبوب اسناد"
    exclude: "TXT"
    description: "GroupDocs.Search از بیش از 70 فرمت فایل پشتیبانی می‌کند و قوانین جستجوی انعطاف‌پذیر و نمایه‌سازی کارآمد را برای صرفه‌جویی در زمان و تلاش فراهم می‌کند."
    items: 
        # format loop 1
        - name: "جستجوی بولی در DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/boolean/docx/"
          description: "سند XML باز مایکروسافت ورد"
          
        # format loop 2
        - name: "جستجوی بولی در PDF"
          format: "PDF"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 3
        - name: "جستجوی بولی در PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "ارائه XML باز پاورپوینت"

        # format loop 4
        - name: "جستجوی بولی در TXT"
          format: "TXT"
          link: "/search/nodejs-java/boolean/txt/"
          description: "سند متنی"
          
        # format loop 5
        - name: "جستجوی بولی در XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "برگه XML باز مایکروسافت اکسل"
  

---