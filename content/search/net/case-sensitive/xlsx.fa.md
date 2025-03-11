
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:32
draft: false
lang: fa
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "جستجوی حساس به حروف در XLSX با استفاده از .NET"
head_description: "API GroupDocs.Search for .NET به توسعه‌دهندگان C# امکان می‌دهد تا جستجوهای حساس به حروف را در میان اسناد مختلف انجام دهند."

############################# Header ############################
title: "جستجوی حساس به حروف" 
description: "GroupDocs.Search for .NET به شما این امکان را می‌دهد که درخواست‌های جستجوی حساس به حروف پیشرفته‌ای را در برنامه‌های .NET خود ایجاد کنید."
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
    link_title: "بیشتر بدانید"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) یک کتابخانه قدرتمند برای جستجو و ایندکس‌گذاری متن در اسناد است. این کتابخانه از بیش از 70 فرمت فایل، از جمله PDF، Word، PowerPoint، Excel، تصاویر و فایل‌های ZIP پشتیبانی می‌کند و اطمینان حاصل می‌کند که حجم‌های بزرگ داده به‌طور مؤثر مدیریت شوند.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه جستجوی حساس به حروف را در اسناد XLSX انجام دهیم"
    content: |
      [GroupDocs.Search](/search/net/) جستجوی حساس به حروف را در اسناد XLSX ساده می‌کند. از آن برای بهبود نتایج در برنامه‌های .NET استفاده کنید.
      
      1. پوشه‌ای برای نگهداری ایندکس جستجو تعریف کنید.
      2. پوشه‌ای حاوی فایل‌های XLSX انتخاب کنید.
      3. جستجو را اجرا کنید و نتایج را بازیابی کنید.
      4. نتایج را پردازش کنید.
   
    code:
      platform: "net"
      copy_title: "کپی"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
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
        // مسیر پوشه ایندکس را تعیین کنید
        Index index = new Index("c:/MyIndex");

        // پوشه حاوی اسنادی که باید جستجو شوند را مشخص کنید
        index.Add("c:/MyDocuments");

        // حساسیت به حروف را در گزینه‌ها فعال کنید
        SearchOptions options = new SearchOptions();
        options.UseCaseSensitiveSearch = true;

        // جستجو را انجام دهید
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "امکانات پیشرفته برای جستجو و ایندکس‌گذاری اسناد"
  description: "کتابخانه GroupDocs.Search for .NET جستجو و ایندکس‌گذاری متن را در بیش از 70 فرمت فایل ساده می‌کند. اطلاعات را با ابزارهای جستجوی قدرتمند به‌راحتی پیدا و مدیریت کنید."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Search"
  features:
    # feature loop
    - title: "جستجوی متنی پیشرفته"
      content: "متن را در فرمت‌های مختلف فایل، از جمله PDFs، اسناد Word، صفحات گسترده و ارائه‌ها جستجو کنید. از گزینه‌هایی مانند مطابقت دقیق، جستجوی نادقیق و کاراکترهای جایگزین برای نتایج دقیق‌تر استفاده کنید."

    # feature loop
    - title: "ایندکس‌گذاری مجموعه‌های بزرگ داده"
      content: "ایندکس‌ها را برای جستجوهای سریع‌تر ایجاد و نگهداری کنید. ایندکس‌گذاری منظم جستجوی مجموعه‌های گسترده‌ای از اسناد را ساده می‌کند."

    # feature loop
    - title: "پشتیبانی چندزبانه"
      content: "در میان اسناد با بیش از 80 زبان جستجو کنید و از پشتیبانی فرمت‌های کلیدهای مختلف و اشکال کلمات برای نتایج دقیق‌تر بهره‌مند شوید."

    # feature loop
    - title: "گزینه‌های جستجو قابل تنظیم"
      content: "تنظیمات جستجو را با حساسیت به حروف، فیلترهای محدوده تاریخ و توانایی حذف کلمات یا داده‌های خاص در حین ایندکس‌گذاری سفارشی کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "استفاده از درخواست‌های جستجوی حساس به حروف"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توان از درخواست‌های حساس به حروف برای جستجوی اسناد XLSX استفاده کرد.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // پوشه‌ای برای ایندکس جستجو تعیین کنید
          Index index = new Index("c:/MyIndex");
              
          // مسیر اسنادی که باید جستجو شوند را مشخص کنید
          index.Add("c:/MyDocuments");

          // یک درخواست جستجو ایجاد کنید
          SearchQuery wordQuery = SearchQuery.CreateWordQuery("Lorem");

          // گزینه‌های جستجوی حساس به حروف را فعال کنید
          SearchOptions options = new SearchOptions();
          options.UseCaseSensitiveSearch = true;

          // برای متن در اسناد جستجو کنید
          SearchResult result = index.Search(wordQuery, options);
          
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
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.xlsx"
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
  description: "امکانات GroupDocs.Search را به صورت رایگان امتحان کنید یا درخواست مجوز دهید"
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
    exclude: "case-sensitive"
    description: "به بررسی قابلیت‌های جستجوی پیشرفته و کارآمد بپردازید."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "جستجوی فرمت‌های محبوب اسناد"
    exclude: "XLSX"
    description: "GroupDocs.Search از بیش از 70 فرمت فایل پشتیبانی می‌کند. قوانین جستجو را سفارشی کنید و از ایندکس‌گذاری برای صرفه‌جویی در زمان و تلاش استفاده کنید."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/case-sensitive/docx/"
          description: "مدرک مایکروسافت ورد Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/case-sensitive/pdf/"
          description: "فرمت مدرک قابل حمل Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/case-sensitive/pptx/"
          description: "ارائه PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/case-sensitive/txt/"
          description: "مدرک متنی"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/case-sensitive/xlsx/"
          description: "جدول محتوای Open XML مایکروسافت اکسل"
  

---