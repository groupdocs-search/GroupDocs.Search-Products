
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:45
draft: false
lang: fa
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "TXT را در .NET با استفاده از اپراتورهای بولی جستجو کنید"
head_description: "API GroupDocs.Search for .NET به توسعه‌دهندگان C# این امکان را می‌دهد که محتوای اسناد را با استفاده از اپراتورهای بولی مانند AND، OR و NOT جستجو کنند."

############################# Header ############################
title: "جستجوی متن با منطق بولی" 
description: "GroupDocs.Search for .NET ایجاد پرسش‌های جستجوی پیشرفته با استفاده از اپراتورهای بولی (AND، OR، NOT) در برنامه‌های .NET شما را ساده می‌سازد."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "رایگان دانلود کنید"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search چیست؟"
    link: "/search/net/"
    link_title: "بیشتر بیاموزید"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) یک کتابخانه جامع برای جستجو و نمایه‌سازی متن در اسناد است. این کتابخانه از بیش از 70 فرمت فایل مانند PDF، Word، PowerPoint، Excel، تصاویر و فایل‌های ZIP پشتیبانی می‌کند و پردازش کارآمد مقادیر زیادی اطلاعات را ممکن می‌سازد.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه محتوای سند TXT را با استفاده از منطق بولی جستجو کنیم"
    content: |
      [GroupDocs.Search](/search/net/) جستجوی محتوای سند TXT را ساده می‌کند. این ابزار شرایط جستجوی منطقی بولی را برای تصحیح نتایج در برنامه‌های .NET فراهم می‌آورد.
      
      1. پوشه‌ای برای ذخیره نمایه جستجو مشخص کنید.
      2. پوشه حاوی فایل‌های TXT را انتخاب کنید.
      3. جستجو را اجرا کرده و نتایج را بازیابی کنید.
      4. نتایج را پردازش کنید.
   
    code:
      platform: "net"
      copy_title: "کپی"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "نتیجه جستجو"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "برای کپی کلیک کنید"
        copy_done: "کپی شد"
      links:
        #  loop
        - title: "مثال‌های بیشتر"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "مستندات"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // مسیر پوشه نمایه را تنظیم کنید
        Index index = new Index("c:/MyIndex");

        // پوشه حاوی اسنادی که باید جستجو شوند را مشخص کنید
        index.Add("c:/MyDocuments");

        // یک جستجو با استفاده از یک پرسش پیچیده اجرا کنید
        SearchResult result = index.Search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ویژگی‌های پیشرفته جستجو و نمایه‌سازی اسناد را کشف کنید"
  description: "کتابخانه GroupDocs.Search for .NET جستجو و نمایه‌سازی متن را برای بیش از 70 فرمت فایل ساده می‌کند. اطلاعات را با استفاده از ابزارهای جستجوی پیشرفته راحت پیدا و مدیریت کنید."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "ویژگی‌های اصلی GroupDocs.Search"
  features:
    # feature loop
    - title: "جستجوی متنی قدرتمند"
      content: "به جستجوی متن در انواع مختلف فایل‌ها، از جمله PDF، اسناد Word، ارائه‌های PowerPoint و صفحات گسترده بپردازید. از ویژگی‌هایی مانند تطابق دقیق، جستجوهای تقریبی و کاراکترهای حاشیه‌ای برای تصحیح نتایج استفاده کنید."

    # feature loop
    - title: "نمایه‌سازی مجموعه‌های داده بزرگ"
      content: "ایجاد و نگهداری نمایه‌ها برای جستجوهای سریع‌تر. نمایه‌سازی داده را ساختاردهی و سازمان‌دهی می‌کند و جستجوی مجموعه‌های چشمگیر اسناد را آسان‌تر می‌سازد."

    # feature loop
    - title: "پشتیبانی از چندین زبان"
      content: "جستجوی اسناد به بیش از 80 زبان، با پشتیبانی از چیدمان‌های صفحه‌کلید مختلف و اشکال کلماتی ساختاریافته برای افزایش دقت جستجو."

    # feature loop
    - title: "گزینه‌های جستجوی قابل تنظیم"
      content: "تنظیمات جستجو را با ویژگی‌هایی مانند حساسیت به حرف بزرگ و کوچک، فیلترهای بازه تاریخ و امکان حذف کلمات یا داده‌های خاص در طول نمایه‌سازی تنظیم کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "استفاده از پرسش‌های جستجوی بولی پیشرفته"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توان از پرسش‌های بولی برای جستجوی اسناد TXT استفاده کرد.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // پوشه نمایه جستجو را تنظیم کنید
          Index index = new Index("c:/MyIndex");
              
          // مسیر اسناد برای جستجو را مشخص کنید
          index.Add("c:/MyDocuments");

          // یک پرسش جستجو با استفاده از منطق بولی ایجاد کنید
          SearchQuery wordQuery1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.CreateWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.CreateAndQuery(wordQuery1, wordQuery2);

          // نتایج جستجو را بازیابی کنید
          SearchResult result = index.Search(booleanQuery);
          
          // نتایج جستجو را پردازش کنید
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "کپی"
        install:
          command: "dotnet add package GroupDocs.Search"
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
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "مستندات"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "آماده شروع هستید؟"
  description: "ویژگی‌های GroupDocs.Search را رایگان امتحان کنید یا درخواست مجوز دهید"
  items:
    #  loop
    - title: "دانلود Nuget"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "مجوزدهی"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "ویژگی‌های کلیدی را کشف کنید"
    exclude: "boolean"
    description: "عملکردهای جستجوی پیشرفته و کارآمد را بررسی کنید."
    items: 
          
        # operation loop 1
        - name: "جستجو با شرط"
          operation: "boolean"
          link: "/search/net/boolean/txt/"
          description: "یافتن اطلاعات در اسناد با استفاده از شرایط بولی"

        # operation loop 2
        - name: "جستجوی حساس به حروف بزرگ و کوچک"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/txt/"
          description: "دقت جستجو را با در نظر گرفتن حساسیت حروف افزایش دهید"

        # operation loop 3
        - name: "شاخص‌گذاری اسناد"
          operation: "document"
          link: "/search/net/document/txt/"
          description: "اسناد را یک‌بار شاخص‌گذاری کنید و از شاخص برای جستجوهای متعدد استفاده کنید"

        # operation loop 4
        - name: "فیلترهای جستجو"
          operation: "filters"
          link: "/search/net/filters/txt/"
          description: "از فیلترها برای محدود کردن داده‌های پردازش‌شده استفاده کنید"

        # operation loop 5
        - name: "عبارت دقیق"
          operation: "phrase"
          link: "/search/net/phrase/txt/"
          description: "جستجو برای یک جمله یا عبارت خاص"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "جستجو در فرمت‌های رایج اسناد"
    exclude: "TXT"
    description: "GroupDocs.Search از بیش از 70 فرمت فایل پشتیبانی می‌کند. قواعد جستجو را سفارشی‌سازی کرده و از نمایه‌سازی برای صرفه‌جویی در زمان و تلاش بهره‌برداری کنید."
    items: 
        # format loop 1
        - name: "جستجوی بولی در DOCX"
          format: "DOCX"
          link: "/search/net/boolean/docx/"
          description: "سند XML باز مایکروسافت ورد"
          
        # format loop 2
        - name: "جستجوی بولی در PDF"
          format: "PDF"
          link: "/search/net/boolean/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 3
        - name: "جستجوی بولی در PPTX"
          format: "PPTX"
          link: "/search/net/boolean/pptx/"
          description: "ارائه XML باز پاورپوینت"

        # format loop 4
        - name: "جستجوی بولی در TXT"
          format: "TXT"
          link: "/search/net/boolean/txt/"
          description: "سند متنی"
          
        # format loop 5
        - name: "جستجوی بولی در XLSX"
          format: "XLSX"
          link: "/search/net/boolean/xlsx/"
          description: "برگه XML باز مایکروسافت اکسل"
  

---