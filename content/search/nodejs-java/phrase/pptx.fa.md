
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:40
draft: false
lang: fa
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "جستجوی عبارات در PPTX با استفاده از Node.js"
head_description: "GroupDocs.Search for Node.js via Java قابلیت جستجوی قوی عبارات را به برنامه‌های JavaScript اضافه می‌کند تا جستجوی اسناد به شکلی کارآمد انجام شود."

############################# Header ############################
title: "پیدا کردن عبارات در اسناد" 
description: "با GroupDocs.Search for Node.js via Java عبارات خاص را به سرعت پیدا کنید. قابلیت‌های جستجوی سریع و دقیق را به برنامه‌های Node.js خود ادغام کنید."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "ویژگی‌های GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "بیشتر بدانید"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) یک کتابخانه با کارایی بالا برای ایندکس‌گذاری و جستجوی متن در اسناد است. این کتابخانه از بیش از 70 فرمت فایل شامل PDF، اسناد Word، صفحات Excel، تصاویر و آرشیوهای ZIP پشتیبانی می‌کند و اطمینان حاصل می‌کند که نتایج جستجو دقیق و سریع هستند.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه عبارات را در اسناد PPTX پیدا کنیم"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) جستجوی عبارات در اسناد PPTX را آسان می‌کند. از گزینه‌های مختلف جستجو برای بهبود نتایج در برنامه‌های Node.js via Java استفاده کنید.
      
      1. یک پوشه برای ایندکس جستجو راه‌اندازی کنید.
      2. پوشه حاوی فایل‌های PPTX را تعیین کنید.
      3. پارامترهای جستجو را پیکربندی کنید.
      4. نتایج جستجو را بازیابی و پردازش کنید.
   
    code:
      platform: "nodejs-java"
      copy_title: "کپی"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
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

        // مسیر ذخیره ایندکس جستجو را مشخص کنید
        const index = new searchLib.Index("c:/MyIndex");

        // پوشه حاوی اسناد را تعیین کنید
        index.add("c:/MyDocuments");

        // تنظیمات جستجو را پیکربندی کنید
        const word1 = searchLib.SearchQuery.createWordQuery("lorem");
        const word2 = searchLib.SearchQuery.createWordQuery("ipsum");
        const word3 = searchLib.SearchQuery.createWordQuery("dolor");

        const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, word2, word3);

        // پرسش جستجو را اجرا کنید
        const result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "کشف موتور جستجوی اسناد Node.js"
  description: "GroupDocs.Search for Node.js via Java امکان جستجوی عبارات در بیش از 70 فرمت فایل را فراهم می‌کند و به راحتی داده‌ها را با ویژگی‌های جستجوی پیشرفته پیدا و سازماندهی کنید."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "قابلیت‌های کلیدی GroupDocs.Search"
  features:
    # feature loop
    - title: "جستجوی عبارات"
      content: "عبارات دقیق را در اسناد تجاری مانند PDF، فایل‌های Word، ارائه‌ها و صفحات گسترده پیدا کنید. از کاراکترهای جایگزین و گزینه‌های جستجوی انعطاف‌پذیر استفاده کنید زمانی که عبارت کامل مشخص نیست."

    # feature loop
    - title: "ایندکس‌گذاری بهینه داده‌ها"
      content: "عملکرد جستجو را با ایجاد ایندکس‌های قابل استفاده مجدد افزایش دهید. ایندکس‌گذاری ساختاری سرعت جستجوی اسناد را افزایش داده و دقت را بهبود می‌بخشد."

    # feature loop
    - title: "سازگاری چند زبانه"
      content: "در بیش از 80 زبان اسناد را جستجو کنید و از پشتیبانی از چیدمان‌های صفحه‌کلید مختلف و تغییرات مورفولوژیکی کلمات بهره‌مند شوید، تا نتایج دقیقی به دست آورید."

    # feature loop
    - title: "گزینه‌های جستجوی پیشرفته"
      content: "جستجوها را با حساسیت به حروف، تطابق تقریباً، تشخیص هم‌صدا، فیلتر کردن اسناد و سایر ویژگی‌های قدرتمند سفارشی کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "استفاده از تکنیک‌های جستجوی پیشرفته"
      content: |
        یاد بگیرید که چگونه برای جستجو در PPTX سوال‌ها را بسازید.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // دایرکتوری ایندکس جستجو را تعریف کنید
          const index = new searchLib.Index("c:/MyIndex");
              
          // مسیر سندهای هدف را تعیین کنید
          index.add("c:/MyDocuments");

          // یک پرسش برای عبارت مورد نظر بسازید
          const word1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wildcard = searchLib.SearchQuery.createWildcardQuery(1, 7);
          const word2 = searchLib.SearchQuery.createWordQuery("dolor");

          const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // نتایج جستجو را بازیابی کنید
          const result = index.search(query);
          
          // نتایج را پردازش و استفاده کنید
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
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchphrase.pptx"
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
  description: "امکانات GroupDocs.Search را به صورت رایگان امتحان کنید یا درخواست مجوز دهید"
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
    title: "قابلیت‌های جستجوی پیشرفته"
    exclude: "phrase"
    description: "از ویژگی‌های قوی جستجو برای دریافت نتایج سریع‌تر و دقیق‌تر بهره ببرید."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "جستجوی عبارات در اسناد تجاری"
    exclude: "PPTX"
    description: "GroupDocs.Search از جستجوی عبارات در بیش از 70 فرمت سند پشتیبانی می کند. از گزینه‌های پیشرفته و ایندکس‌گذاری برای تسهیل فرایند جستجو استفاده کنید."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/phrase/docx/"
          description: "مدرک مایکروسافت ورد Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "فرمت مدرک قابل حمل Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "ارائه PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/phrase/txt/"
          description: "مدرک متنی"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "جدول محتوای Open XML مایکروسافت اکسل"
  

---