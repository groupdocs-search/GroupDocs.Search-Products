
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:48
draft: false
lang: fa
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "جستجوی حساس به حروف بزرگ در XLSX با Node.js"
head_description: "API GroupDocs.Search for Node.js via Java به توسعه‌دهندگان JavaScript اجازه می‌دهد تا جستجوهای حساس به حروف بزرگ را در انواع مختلف اسناد انجام دهند."

############################# Header ############################
title: "جستجوی حساس به حروف بزرگ" 
description: "GroupDocs.Search for Node.js via Java به شما اجازه می‌دهد تا قابلیت‌های جستجو حساس به حروف بزرگ را به راحتی در برنامه‌های Node.js خود پیاده‌سازی کنید."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود رایگان"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "چیست GroupDocs.Search؟"
    link: "/search/nodejs-java/"
    link_title: "بیشتر بیاموزید"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) یک کتابخانه قدرتمند برای جستجو و نمایه‌سازی متن در اسناد است. این کتابخانه از بیش از 70 فرمت پشتیبانی می‌کند، از جمله PDF، Word، Excel، PowerPoint، تصاویر و فایل‌های ZIP، که مدیریت بخش‌های بزرگ داده‌ای را آسان می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "مراحل انجام جستجوهای حساس به حروف بزرگ در فایل‌های XLSX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) جستجوهای حساس به حروف بزرگ را در فایل‌های XLSX تسهیل می‌کند و روندهای Node.js via Java شما را بهبود می‌بخشد.
      
      1. یک پوشه برای ذخیره نمایه جستجو ایجاد کنید.
      2. پوشه‌ای که فایل‌های XLSX در آن قرار دارد را انتخاب کنید.
      3. جستجو را اجرا کرده و نتایج را دریافت کنید.
      4. نتایج را پردازش و استفاده کنید.
   
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

        // مسیر پوشه نمایه را مشخص کنید
        const index = new searchLib.Index("c:/MyIndex");

        // پوشه‌ای که اسناد در آن قرار دارد را تعیین کنید
        index.add("c:/MyDocuments");

        // جستجوی حساس به حروف بزرگ را در تنظیمات فعال کنید
        const options = new groupdocs.search.SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // عمل جستجو را انجام دهید
        const result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ویژگی‌های کلیدی برای جستجو و نمایه‌سازی اسناد"
  description: "با GroupDocs.Search for Node.js via Java، می‌توانید به آسانی متن را در بیش از 70 فرمت فایل جستجو و نمایه‌سازی کنید. اطلاعات را با استفاده از ابزارهای جستجوی پیشرفته به‌راحتی دسترسی و سازماندهی کنید."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "ویژگی‌های اصلی GroupDocs.Search"
  features:
    # feature loop
    - title: "جستجوی جامع متن"
      content: "متن را در انواع مختلف اسناد مانند PDF، فایل‌های Word، جداول و ارائه‌ها پیدا کنید. از گزینه‌های مانند تطابق دقیق، جستجوی تقریبی و کاراکترهای جایگزین برای دستیابی به نتایج دقیق استفاده کنید."

    # feature loop
    - title: "نمایه‌سازی کارآمد داده‌ها"
      content: "شاخص‌ها را ایجاد و مدیریت کنید تا جستجوها سریع‌تر شوند. نمایه‌سازی به شما کمک می‌کند داده‌ها را در مجموعه‌های بزرگ اسناد سازماندهی و به‌سرعت پیدا کنید."

    # feature loop
    - title: "پشتیبانی از چندین زبان"
      content: "اسناد را به بیش از 80 زبان جستجو کنید با پشتیبانی از چیدمان‌های مختلف صفحه‌کلید و تنوع‌های کلمه، که دقت نتایج جستجو را تضمین می‌کند."

    # feature loop
    - title: "تنظیمات جستجوی قابل تنظیم"
      content: "تنظیمات جستجو، از جمله حساسیت به حروف بزرگ، فیلترهای تاریخ و حذف اصطلاحات یا داده‌های خاص در هنگام نمایه‌سازی را تنظیم کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "مثال: پیاده‌سازی جستجوی حساس به حروف بزرگ"
      content: |
        این مثال نشان می‌دهد که چگونه جستجوهای حساس به حروف بزرگ را برای اسناد XLSX انجام دهید.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // پوشه‌ای برای نمایه جستجو تعریف کنید
          const index = new searchLib.Index("c:/MyIndex");
              
          // مسیر پوشه اسناد را ارائه دهید
          index.add("c:/MyDocuments");

          // یک پرس و جو جستجو تنظیم کنید
          const wordQuery = searchLib.SearchQuery.createWordQuery("Lorem");

          // تنظیمات جستجوی حساس به حروف بزرگ را فعال کنید
          const options = new groupdocs.search.SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // به دنبال متن در اسناد بگردید
          const result = index.search(wordQuery, options);
          
          // نتایج را پردازش و مدیریت کنید
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
            link: "/examples/search/formats/searchcase-sensitive.xlsx"
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
    title: "عملکردهای کلیدی"
    exclude: "case-sensitive"
    description: "ویژگی‌های پیشرفته برای جستجوی سریع و دقیق اسناد را بررسی کنید."
    items: 
          
        # operation loop 1
        - name: "جستجو با شرط"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "یافتن اطلاعات در اسناد با استفاده از شرایط بولی"

        # operation loop 2
        - name: "جستجوی حساس به حروف بزرگ و کوچک"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "دقت جستجو را با در نظر گرفتن حساسیت حروف افزایش دهید"

        # operation loop 3
        - name: "شاخص‌گذاری اسناد"
          operation: "document"
          link: "/search/nodejs-java/document/xlsx/"
          description: "اسناد را یک‌بار شاخص‌گذاری کنید و از شاخص برای جستجوهای متعدد استفاده کنید"

        # operation loop 4
        - name: "فیلترهای جستجو"
          operation: "filters"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "از فیلترها برای محدود کردن داده‌های پردازش‌شده استفاده کنید"

        # operation loop 5
        - name: "عبارت دقیق"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "جستجو برای یک جمله یا عبارت خاص"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "فرمت‌های اسناد سازگار"
    exclude: "XLSX"
    description: "GroupDocs.Search از بیش از 70 فرمت سند پشتیبانی می‌کند. گزینه‌های جستجوی خود را سفارشی کنید و زمان خود را با نمایه‌سازی صرفه‌جویی کنید."
    items: 
        # format loop 1
        - name: "جستجوی حساس به حروف بزرگ و کوچک DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "سند XML باز مایکروسافت ورد"
          
        # format loop 2
        - name: "جستجوی حساس به حروف بزرگ و کوچک PDF"
          format: "PDF"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 3
        - name: "جستجوی حساس به حروف بزرگ و کوچک PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "ارائه XML باز پاورپوینت"

        # format loop 4
        - name: "جستجوی حساس به حروف بزرگ و کوچک TXT"
          format: "TXT"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "سند متنی"
          
        # format loop 5
        - name: "جستجوی حساس به حروف بزرگ و کوچک XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "برگه XML باز مایکروسافت اکسل"
  

---