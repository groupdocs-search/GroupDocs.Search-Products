
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: fa
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "جستجوی اسناد TXT در .NET با GroupDocs.Search"
head_description: "از GroupDocs.Search for .NET برای انجام جستجوهای متنی کارآمد در قالب‌های مختلف اسنادی با C# استفاده کنید."

############################# Header ############################
title: "جستجوی پیشرفته متن اسناد" 
description: "GroupDocs.Search for .NET جستجوی متن در قالب‌های محبوب اسنادی را ساده می‌کند و به شما اجازه می‌دهد تا کوئری‌های جستجوی قوی در برنامه‌های .NET خود ایجاد کنید."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود رایگان"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search چه‌چیزی است؟"
    link: "/search/net/"
    link_title: "بیشتر بیاموزید"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) یک کتابخانه قدرتمند طراحی شده برای جستجو و ایندکس‌گذاری متن کامل در اسناد است. این کتابخانه از بیش از ۷۰ فرمت فایل پشتیبانی می‌کند، از جمله PDF، Word، PowerPoint، Excel، تصاویر و فایل‌های ZIP، که اطمینان از نتایج جستجوی سریع و دقیق را فراهم می‌آورد.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه در اسناد TXT جستجوی متنی را انجام دهیم"
    content: |
      [GroupDocs.Search](/search/net/) عملیات جستجوی پیشرفته محتوا را در اسناد TXT امکان‌پذیر می‌سازد و اجازه می‌دهد نتایج جستجوی دقیقتری در برنامه‌های .NET داشته باشید.
      
      1. پوشه‌ای را برای ذخیره ایندکس جستجو راه‌اندازی کنید.
      2. پوشه‌ای را انتخاب کنید که شامل فایل‌های TXT است.
      3. گزینه‌های جستجوی اضافی را پیکربندی کنید.
      4. جستجو را اجرا کرده و نتایج را مرور کنید.
   
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
        // مسیر ایندکس جستجو را تعریف کنید
        Index index = new Index("c:/MyIndex");

        // پوشه‌ای را که شامل اسناد است انتخاب کنید که باید جستجو شوند
        index.Add("c:/MyDocuments");

        // جستجوی هم‌صدا را برای پیدا کردن کلمات مشابه فعال کنید
        SearchOptions options = new SearchOptions();
        options.UseHomophoneSearch = true;

        // یک کوئری جستجوی پیچیده را اجرا کنید
        SearchResult result = index.Search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ویژگی‌های پیشرفته جستجو و ایندکس‌گذاری"
  description: "GroupDocs.Search for .NET جستجو و ایندکس‌گذاری متن را در بیش از ۷۰ فرمت فایل تقویت می‌کند و ابزارهای کارآمدی برای پیدا کردن و مدیریت اطلاعات ارائه می‌دهد."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Search"
  features:
    # feature loop
    - title: "جستجوی متن قدرتمند"
      content: "برای جستجوی متن در انواع مختلف اسناد، از جمله PDFها، اسناد Word، ارائه‌های PowerPoint و صفحه‌گسترده‌ها استفاده کنید. از ویژگی‌هایی مانند تطابق دقیق، جستجوی مبهم و کاراکترهای جایگزین برای دقیق‌تر کردن نتایج خود استفاده کنید."

    # feature loop
    - title: "ایندکس‌گذاری سریع برای مجموعه‌های داده بزرگ"
      content: "ایندکس‌های جستجو را برای بازیابی سریع اطلاعات ایجاد و مدیریت کنید. ایندکس‌گذاری جستجوها را در مجموعه‌های گسترده اسنادی بهینه می‌کند."

    # feature loop
    - title: "پشتیبانی چندزبانه"
      content: "جستجوها را در بیش از ۸۰ زبان انجام دهید، با پشتیبانی از طرح‌های صفحه‌کلید مختلف و واریانت‌های واژه برای بهبود دقت."

    # feature loop
    - title: "تنظیمات جستجو قابل تنظیم"
      content: "پارامترهای جستجو را با گزینه‌هایی مانند حساسیت به حروف بزرگ و کوچک، فیلترهای بازه تاریخی و exclusions کلمات برای نتایج بهتر سفارشی کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "اجرای کوئری‌های جستجوی پیشرفته"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توان کوئری‌های جستجو را برای اسناد TXT اعمال کرد.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // پوشه‌ای را برای ایندکس جستجو تعریف کنید
          Index index = new Index("c:/MyIndex");
              
          // مسیر فایل‌های سند را مشخص کنید
          index.Add("c:/MyDocuments");

          // یک رمز عبور برای اسناد محافظت‌شده ارائه دهید
          index.Dictionaries.DocumentPasswords.Add("protected.txt", "123456");

          // جستجوی مبهم را برای پیدا کردن کلمات مشابه فعال کنید
          SearchOptions options = new SearchOptions();
          options.FuzzySearch.Enabled = true;
          options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8);

          // نتایج جستجو را بازیابی کنید
          SearchResult result = index.Search("Loarem", options);
          
          // خروجی جستجو را پردازش کنید
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
            link: "/examples/search/formats/searchdocument.txt"
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
    title: "اکتشاف ویژگی‌های کلیدی"
    exclude: "document"
    description: "از قابلیت‌های جستجوی پیشرفته و با عملکرد بالا بهره‌مند شوید."
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
    title: "جستجو در اسناد تجاری شما"
    exclude: "TXT"
    description: "GroupDocs.Search از بیش از ۷۰ فرمت فایل پشتیبانی می‌کند، از جمله اسناد اداری، که جستجوهای سریع و کارآمد با قابلیت‌های ایندکس‌گذاری را امکان‌پذیر می‌سازد."
    items: 
        # format loop 1
        - name: "جستجو در سند DOCX"
          format: "DOCX"
          link: "/search/net/document/docx/"
          description: "سند XML باز مایکروسافت ورد"
          
        # format loop 2
        - name: "جستجو در سند PDF"
          format: "PDF"
          link: "/search/net/document/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 3
        - name: "جستجو در سند PPTX"
          format: "PPTX"
          link: "/search/net/document/pptx/"
          description: "ارائه XML باز پاورپوینت"

        # format loop 4
        - name: "جستجو در سند TXT"
          format: "TXT"
          link: "/search/net/document/txt/"
          description: "سند متنی"
          
        # format loop 5
        - name: "جستجو در سند XLSX"
          format: "XLSX"
          link: "/search/net/document/xlsx/"
          description: "برگه XML باز مایکروسافت اکسل"
  

---