
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: fa
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "جستجو در اسناد TXT با استفاده از Node.js"
head_description: "GroupDocs.Search for Node.js via Java قابلیت‌های جستجوی متن سریع و دقیقی را به برنامه‌های JavaScript اضافه می‌کند و از چندین قالب سند پشتیبانی می‌کند."

############################# Header ############################
title: "یافتن متن در اسناد تجاری" 
description: "GroupDocs.Search for Node.js via Java قابلیت جستجوی قدرتمند و منعطفی را برای اسناد فراهم می‌کند. جستجوی متن را به راحتی در برنامه‌های Node.js یکپارچه کنید."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "رایگان دانلود کنید"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search چیست؟"
    link: "/search/nodejs-java/"
    link_title: "بیشتر بیاموزید"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) یک کتابخانه جستجو و ایندکس‌گذاری قوی است که امکان بازیابی سریع متن در اسناد را فراهم می‌کند. این کتابخانه از بیش از 70 فرمت فایل، از جمله PDF، Word، Excel و PowerPoint پشتیبانی می‌کند و جستجوهای دقیق و کارآمدی را تضمین می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه در اسناد TXT جستجو کنیم"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) جستجوی متن در اسناد TXT را برای برنامه‌های Node.js via Java ساده و کارآمد می‌سازد.
      
      1. یک دایرکتوری برای ذخیره ایندکس جستجو ایجاد کنید.
      2. پوشه‌ای که شامل اسناد است را انتخاب کنید.
      3. گزینه‌های جستجو را برای شامل کردن فقط فایل‌های TXT تنظیم کنید.
      4. جستجو را اجرا کنید و نتایج را بازیابی کنید.
   
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

        // یک دایرکتوری برای ذخیره ایندکس جستجو تعیین کنید
        const index = new searchLib.Index("c:/MyIndex");

        // پوشه‌ای که شامل اسناد قابل جستجو است را مشخص کنید
        index.add("c:/MyDocuments");

        // جستجو را به فرمت‌های خاص فایل محدود کنید
        const options = new searchLib.SearchOptions();
        options.SearchDocumentFilter = 
            searchLib.SearchDocumentFilter.createFileExtension(".txt");

        // نتایج جستجو را بازیابی و پردازش کنید
        const result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "قابلیت‌های جستجوی پیشرفته"
  description: "GroupDocs.Search for Node.js via Java کارآیی جستجوی اسناد را با ایندکس‌گذاری بیش از 70 فرمت فایل بهبود می‌بخشد. با استفاده از تکنیک‌های جستجوی پیشرفته، بازیابی محتوا را بهینه‌سازی کنید."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Search"
  features:
    # feature loop
    - title: "جستجوی جامع متن"
      content: "متن را در قالب‌های سند محبوب مانند PDF، فایل‌های Word، صفحات گسترده و ارائه‌ها استخراج و پیدا کنید. از جستجوی تقریبی، هم‌صداها و کوئری‌های wildcard پشتیبانی می‌کند."

    # feature loop
    - title: "ایندکس‌گذاری بهینه برای عملکرد"
      content: "با ایجاد ایندکس‌های قابل استفاده مجدد، جستجوها را تسریع کنید. این ویژگی سرعت و کارآمدی را هنگام کار با مجموعه‌های بزرگ اسناد افزایش می‌دهد."

    # feature loop
    - title: "پشتیبانی از چند زبان"
      content: "در بیش از 80 زبان به جستجو در اسناد بپردازید. برای دقت بیشتر، چیدمان‌های صفحه کلید و واریانت‌های کلمات را شناسایی می‌کند."

    # feature loop
    - title: "گزینه‌های جستجوی قابل تنظیم"
      content: "نتایج جستجو را با فیلترها، عبارات منظم، حساسیت به حروف بزرگ و سایر تنظیمات انعطاف‌پذیر به دقت تنظیم کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "فیلتر کردن اسناد قابل جستجو"
      content: |
        با نحوه بهبود جستجوهای سند با استفاده از فیلترها آشنا شوید.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // یک ایندکس را برای استثنا کردن فرمت‌های فایل نامطلوب پیکربندی کنید
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            searchLib.DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = 
            searchLib.DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new searchLib.Index("c:/MyIndex", settings);
              
          // دایرکتوری حاوی اسناد را مشخص کنید
          index.add("c:/MyDocuments");

          // خروجی جستجو را برای استفاده‌های بعدی پردازش کنید
          const result = index.Search("Lorem", options);
          
          // خروجی جستجو را برای استفاده‌های بعدی پردازش کنید
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
            link: "/examples/search/formats/searchfilters.txt"
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
    exclude: "filters"
    description: "جستجوهای سریع و دقیقی را در اسناد انجام دهید."
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
    title: "جستجو در فرمت‌های مختلف سند"
    exclude: "TXT"
    description: "GroupDocs.Search از بیش از 70 نوع فایل پشتیبانی می‌کند و امکان جستجوی مؤثر متن را در انواع اسناد اداری و تجاری فراهم می‌کند."
    items: 
        # format loop 1
        - name: "فیلترهای جستجو برای DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/filters/docx/"
          description: "سند XML باز مایکروسافت ورد"
          
        # format loop 2
        - name: "فیلترهای جستجو برای PDF"
          format: "PDF"
          link: "/search/nodejs-java/filters/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 3
        - name: "فیلترهای جستجو برای PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/filters/pptx/"
          description: "ارائه XML باز پاورپوینت"

        # format loop 4
        - name: "فیلترهای جستجو برای TXT"
          format: "TXT"
          link: "/search/nodejs-java/filters/txt/"
          description: "سند متنی"
          
        # format loop 5
        - name: "فیلترهای جستجو برای XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "برگه XML باز مایکروسافت اکسل"
  

---