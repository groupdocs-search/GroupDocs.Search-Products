
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:35
draft: false
lang: fa
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "یافتن متن در TXT با GroupDocs.Search در Node.js"
head_description: "از GroupDocs.Search for Node.js via Java با JavaScript برای جستجوی کارآمد متن در فرمت‌های مختلف اسنادی استفاده کنید."

############################# Header ############################
title: "راهکار جستجوی هوشمند اسناد" 
description: "متن را در فرمت‌های مختلف اسنادی با استفاده از GroupDocs.Search for Node.js via Java راحت پیدا کنید. پرس‌و‌جوهای جستجوی پیشرفته‌ای را در برنامه‌های Node.js خود ایجاد کنید."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "رایگان امتحان کنید"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "آشنایی با GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "بیشتر بدانید"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) یک کتابخانه با کارایی بالا برای جستجو و فهرست‌گذاری متنی کامل است. این کتابخانه از بیش از 70 نوع فایل پشتیبانی می‌کند، از جمله PDF، ورد، پاورپوینت، اکسل، تصاویر و آرشیوهای ZIP، که نتایج سریع و دقیقی را تضمین می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "جستجو در فایل‌های TXT"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) به شما این امکان را می‌دهد که جستجوها را در فایل‌های TXT اجرا کنید و نتایج را در برنامه‌های Node.js via Java تصفیه کنید.
      
      1. یک پوشه ذخیره‌سازی برای اندکس جستجو تعریف کنید.
      2. یک پوشه حاوی فایل‌های TXT انتخاب کنید.
      3. پارامترهای جستجوی اضافی را تنظیم کنید.
      4. جستجو را اجرا کرده و نتایج را تحلیل کنید.
   
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

        // دایرکتوری برای ذخیره‌سازی اندکس جستجو را مشخص کنید
        const index = new searchLib.Index("c:/MyIndex");

        // فولدر حاوی اسنادی که می‌خواهید جستجو کنید را انتخاب کنید
        index.add("c:/MyDocuments");

        // جستجوی هم‌صدا برای کلماتی که صداهای مشابهی دارند را فعال کنید
        const options = new searchLib.SearchOptions();
        options.setUseHomophoneSearch(true);

        // یک پرس‌و‌جوی جستجوی پیچیده را اجرا کنید
        const result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "قابلیت‌های پیشرفته جستجو و فهرست‌گذاری"
  description: "GroupDocs.Search for Node.js via Java ابزارهای قدرتمند جستجو و فهرست‌گذاری متن را در بیش از 70 فرمت سند ارائه می‌دهد، که پیدا کردن و سازماندهی اطلاعات را آسان می‌سازد."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "مزایای کلیدی GroupDocs.Search"
  features:
    # feature loop
    - title: "جستجوی جامع متن"
      content: "متن را در انواع مختلف اسناد، از جمله PDF، اسناد ورد، ارائه‌های پاورپوینت و صفحه‌گسترده‌ها پیدا کنید. از مطابقت‌های دقیق، جستجوی تقریبی و کاراکترهایWildcard برای نتایج دقیق‌تر استفاده کنید."

    # feature loop
    - title: "فهرست‌گذاری کارآمد برای داده‌های بزرگ"
      content: "با ایجاد فهرست‌های ساختاری، جستجوها را تسریع کنید و استفاده از اطلاعات از مجموعه‌های بزرگ اسنادی را آسان‌تر کنید."

    # feature loop
    - title: "پشتیبانی از بیش از 80 زبان"
      content: "در اسناد به زبان‌های مختلف جستجو کنید، با شناسایی خودکار فرم‌های مختلف کلمات و چیدمان‌های صفحه‌کلید."

    # feature loop
    - title: "تنظیمات جستجوی سفارشی"
      content: "گزینه‌های جستجو مانند حساسیت به حروف بزرگ و کوچک، فیلترهای تاریخ و حذف کلمات را تنظیم کنید تا نتایج دقیق‌تری بگیرید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "استفاده از جستجو برای اسناد TXT"
      content: |
        این مثال نشان می‌دهد که چگونه از پرسش‌های جستجو درون اسناد TXT استفاده کنید.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // دایرکتوری برای فهرست‌گذاری جستجو را تنظیم کنید
          const index = new searchLib.Index("c:/MyIndex");
              
          // مسیر فایل برای ذخیره‌سازی سند را ارائه دهید
          index.add("c:/MyDocuments");

          // رمز عبور برای فایل‌های محافظت‌شده را وارد کنید
          index.getDictionaries().getDocumentPasswords().add("protected.txt", '123456');

          // جستجوی تقریبی را برای شناسایی کلمات مشابه فعال کنید
          const options = new searchLib.SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new searchLib.SimilarityLevel(0.8));

          // نتایج جستجو را استخراج کنید
          const result = index.search("Loarem", options);
          
          // نتایج را پردازش و بررسی کنید
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
            link: "/examples/search/formats/searchdocument.txt"
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
    title: "ویژگی‌های کلیدی را بررسی کنید"
    exclude: "document"
    description: "ویژگی‌های جستجوی با سرعت بالا را کشف کنید که بهبود کارایی و دقت را طراحی کرده‌اند."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "جستجو در انواع مختلف اسناد"
    exclude: "TXT"
    description: "GroupDocs.Search با بیش از 70 فرمت فایل، از جمله اسناد اداری کار می‌کند و جستجوهای سریع و دقیقی را با پشتیبانی از فهرست‌گذاری تضمین می‌کند."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/document/docx/"
          description: "مدرک مایکروسافت ورد Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/document/pdf/"
          description: "فرمت مدرک قابل حمل Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/document/pptx/"
          description: "ارائه PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/document/txt/"
          description: "مدرک متنی"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/document/xlsx/"
          description: "جدول محتوای Open XML مایکروسافت اکسل"
  

---