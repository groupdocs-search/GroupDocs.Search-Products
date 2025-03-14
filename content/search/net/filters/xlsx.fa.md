
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: fa
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "جستجو در اسناد XLSX با استفاده از .NET"
head_description: "GroupDocs.Search for .NET برنامه‌های C# را با جستجوی متنی موثر در فرمت‌های مختلف اسناد تجاری تقویت می‌کند."

############################# Header ############################
title: "جستجوی متن در اسناد تجاری" 
description: "GroupDocs.Search for .NET جستجوهای متنی قدرتمند و انعطاف‌پذیر را در اسناد شما امکان‌پذیر می‌سازد. قابلیت جستجو را در برنامه‌های .NET به راحتی ادغام کنید."
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
    title: "GroupDocs.Search چیست؟"
    link: "/search/net/"
    link_title: "بیشتر بیاموزید"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) یک کتابخانه قوی برای جستجوی متنی موثر و ایندکس‌گذاری اسناد است. این کتابخانه از بیش از 70 فرمت فایل، از جمله اسناد استاندارد صنعتی مانند PDF، Word، Excel و PowerPoint پشتیبانی می‌کند. با نتایج سریع و دقیق، عملکرد جستجو را بهبود دهید.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه در داده‌های XLSX جستجو کنید"
    content: |
      [GroupDocs.Search](/search/net/) جستجوهای متنی کارآمدی را در اسناد XLSX امکان‌پذیر می‌کند و آن را برای برنامه‌های .NET ایدئال می‌سازد.
      
      1. یک پوشه برای ذخیره ایندکس جستجو تنظیم کنید.
      2. پوشه‌ای که شامل فایل‌های شما است را انتخاب کنید.
      3. گزینه‌های جستجو را برای پردازش فقط اسناد XLSX پیکربندی کنید.
      4. جستجو را انجام دهید و نتایج را بازیابی کنید.
   
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
        // مسیر برای ذخیره ایندکس جستجوی قابل استفاده مجدد
        Index index = new Index("c:/MyIndex");

        // پوشه‌ای که شامل اسناد است
        index.Add("c:/MyDocuments");

        // جستجو فقط در فرمت‌های فایل خاص
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".xlsx");

        // بازیابی نتایج جستجو
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ویژگی‌های پیشرفته جستجو"
  description: "GroupDocs.Search for .NET امکان جستجوهای پیچیده متنی را در بیش از 70 فرمت فایل فراهم می‌کند. ایندکس‌گذاری کارایی جستجو را بهبود می‌بخشد و به مدیریت محتوای اسناد کمک می‌کند."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "ویژگی‌های اصلی GroupDocs.Search"
  features:
    # feature loop
    - title: "جستجوی پیشرفته متن"
      content: "متن‌های مربوطه را از اسناد تجاری محبوب، از جمله PDFها، فایل‌های Word، ارائه‌ها و صفحه‌گسترده‌ها استخراج کنید. از تکنیک‌های جستجوی متعدد مانند جستجوی تقریب، شناسایی همصدایی و کاراکترهای wildcard پشتیبانی می‌کند."

    # feature loop
    - title: "ایندکس‌گذاری بهینه برای جستجوهای سریع‌تر"
      content: "ایندکس‌های جستجو را بسازید و دوباره استفاده کنید تا سرعت جستجو را افزایش دهید. ایندکس‌گذاری عملکرد جستجو در مجموعه‌های بزرگ اسناد را بهینه می‌کند."

    # feature loop
    - title: "پشتیبانی از چندین زبان"
      content: "جستجوها را در اسنادی که به بیش از 80 زبان نوشته شده‌اند، انجام دهید. الگوهای مختلف کیبورد و واریته‌های واژه را برای بهبود دقت تشخیص می‌دهد."

    # feature loop
    - title: "تنظیمات جستجوی انعطاف‌پذیر"
      content: "نتایج جستجو را با گزینه‌های قابل سفارشی‌سازی، از جمله فیلترها، عبارات منظم و تنظیمات حساس به حروف، تصفیه کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "فیلتر کردن اسنادی که باید پردازش شوند"
      content: |
        یاد بگیرید که چگونه جستجوهای اسناد را با استفاده از فیلترها محدود کنید.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // یک ایندکس تنظیم کنید که شامل فرمت‌های فایل خاصی نباشد.
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.CreateFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter);
          settings.DocumentFilter = invertedFilter;

          Index index = new Index("c:/MyIndex", settings);
              
          // دایرکتوری سند را مشخص کنید.
          index.Add("c:/MyDocuments");

          // نتایج جستجو را بازیابی کنید.
          SearchResult result = index.Search("Lorem");
          
          // خروجی جستجو را پردازش و استفاده کنید.
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
            link: "/examples/search/formats/searchfilters.xlsx"
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
    title: "ویژگی‌های کلیدی"
    exclude: "filters"
    description: "اجرای جستجوهای دقیق و کارآمد داده."
    items: 
          
        # operation loop 1
        - name: "جستجو با شرط"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "یافتن اطلاعات در اسناد با استفاده از شرایط بولی"

        # operation loop 2
        - name: "جستجوی حساس به حروف بزرگ و کوچک"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "دقت جستجو را با در نظر گرفتن حساسیت حروف افزایش دهید"

        # operation loop 3
        - name: "شاخص‌گذاری اسناد"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "اسناد را یک‌بار شاخص‌گذاری کنید و از شاخص برای جستجوهای متعدد استفاده کنید"

        # operation loop 4
        - name: "فیلترهای جستجو"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "از فیلترها برای محدود کردن داده‌های پردازش‌شده استفاده کنید"

        # operation loop 5
        - name: "عبارت دقیق"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "جستجو برای یک جمله یا عبارت خاص"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "یافتن داده‌ها در اسناد تجاری شما"
    exclude: "XLSX"
    description: "GroupDocs.Search از بیش از 70 فرمت فایل پشتیبانی می‌کند که امکان پردازش و جستجوی کارآمد اسناد اداری محبوب را فراهم می‌آورد."
    items: 
        # format loop 1
        - name: "فیلترهای جستجو برای DOCX"
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "سند XML باز مایکروسافت ورد"
          
        # format loop 2
        - name: "فیلترهای جستجو برای PDF"
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 3
        - name: "فیلترهای جستجو برای PPTX"
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "ارائه XML باز پاورپوینت"

        # format loop 4
        - name: "فیلترهای جستجو برای TXT"
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "سند متنی"
          
        # format loop 5
        - name: "فیلترهای جستجو برای XLSX"
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "برگه XML باز مایکروسافت اکسل"
  

---