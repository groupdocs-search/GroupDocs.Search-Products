
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:40
draft: false
lang: fa
format: Pptx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "جستجوی عبارات در PPTX با استفاده از .NET"
head_description: "GroupDocs.Search for .NET قابلیت‌های جستجوی قدرتمند عبارات را برای محتوای اسناد به برنامه‌های C# اضافه می‌کند."

############################# Header ############################
title: "جستجوی عبارات در اسناد" 
description: "با GroupDocs.Search for .NET به‌سرعت عبارات خاص را پیدا کنید. قابلیت جستجوی کارآمد را در برنامه‌های .NET خود ادغام کنید."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "ویژگی‌های GroupDocs.Search"
    link: "/search/net/"
    link_title: "بیشتر بدانید"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) یک کتابخانه قدرتمند برای ایندکس‌گذاری و جستجوی متن در اسناد است. این کتابخانه از بیش از 70 فرمت فایل، از جمله PDF، اسناد Word، صفحات Excel، تصاویر و فایل‌های ZIP پشتیبانی می‌کند و امکان دستیابی به نتایج جستجوی سریع و دقیق را فراهم می‌آورد.

############################# Steps ############################
steps:
    enable: true
    title: "نحوه جستجوی عبارات در اسناد PPTX"
    content: |
      [GroupDocs.Search](/search/net/) جستجو در اسناد PPTX را ساده می‌کند. از گزینه‌های مختلف برای اصلاح نتایج جستجو در برنامه‌های .NET استفاده کنید.
      
      1. پوشه ایندکس جستجو را تنظیم کنید.
      2. پوشه‌ای که شامل فایل‌های PPTX است را مشخص کنید.
      3. تنظیمات جستجو را پیکربندی کنید.
      4. نتایج جستجو را بازیابی و پردازش کنید.
   
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
        // مسیر ذخیره ایندکس جستجو
        Index index = new Index("c:/MyIndex");

        // پوشه‌ای که شامل اسناد است
        index.Add("c:/MyDocuments");

        // تنظیم گزینه‌های جستجو
        SearchQuery word1 = SearchQuery.CreateWordQuery("lorem");
        SearchQuery word2 = SearchQuery.CreateWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.CreateWordQuery("dolor");

        SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, word2, word3);

        // اجرای جستجو
        SearchResult result = index.Search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "انجام جستجوی سندی .NET را کشف کنید"
  description: "GroupDocs.Search for .NET امکان جستجوی عبارات را در بیش از 70 فرمت فایل فراهم می‌کند. با قابلیت‌های جستجوی پیشرفته داده‌ها را به‌راحتی پیدا و مدیریت کنید."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Search"
  features:
    # feature loop
    - title: "جستجوی عبارات"
      content: "در اسناد کسب و کار شامل PDF، فایل‌های Word، ارائه‌ها و صفحات گسترده، به‌دنبال عبارات دقیق بگردید. در صورتی که عبارت دقیق مشخص نیست، از کاراکترهای جایگزین و گزینه‌های دیگر استفاده کنید."

    # feature loop
    - title: "ایندکس‌گذاری کارآمد داده‌ها"
      content: "برای سرعت‌بخشیدن به جستجوهای اسنادی، ایندکس‌های جستجو را ایجاد و مجدداً استفاده کنید. ایندکس‌گذاری داده‌ها را به‌طور مؤثری منظم می‌کند و جستجوهای عبارات را سریع‌تر می‌کند."

    # feature loop
    - title: "پشتیبانی از چند زبان"
      content: "در بیش از 80 زبان، اسناد را جستجو کنید. از چیدمان‌های مختلف صفحه‌کلید و فرم‌های کلمه‌ای شناور برای دقت بیشتر جستجو پشتیبانی می‌کند."

    # feature loop
    - title: "گزینه‌های جستجوی انعطاف‌پذیر"
      content: "جستجوهای خود را با ویژگی‌هایی مانند حساسیت به حروف، جستجوی تقریب و هم‌قافیه، فیلتر کردن اسناد و غیره سفارشی کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "استفاده از تکنیک‌های جستجوی پیشرفته"
      content: |
        یاد بگیرید که چگونه برای جستجو در PPTX پرس‌وجوها ایجاد کنید.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // پوشه برای ایندکس جستجو را مشخص کنید
          Index index = new Index("c:/MyIndex");
              
          // مسیر اسناد برای جستجو را تنظیم کنید
          index.Add("c:/MyDocuments");

          // یک پرس‌وجو برای یک عبارت خاص ایجاد کنید
          SearchQuery word1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.CreateWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.CreateWordQuery("dolor");

          SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, wildcard, word2);

          // نتایج جستجو را بازیابی کنید
          SearchResult result = index.Search(query);
          
          // نتایج را پردازش و از آن‌ها استفاده کنید
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
            link: "/examples/search/formats/searchphrase.pptx"
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
    title: "ویژگی‌های پیشرفته"
    exclude: "phrase"
    description: "از قابلیت‌های جستجوی قدرتمند و کارآمد بهره‌برداری کنید."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "جستجوی عبارات در اسناد کسب و کار"
    exclude: "PPTX"
    description: "GroupDocs.Search از جستجو در بیش از 70 فرمت سند پشتیبانی می‌کند. از گزینه‌های پیشرفته و ایندکس‌گذاری برای تسهیل فرآیند جستجوی خود استفاده کنید."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/phrase/docx/"
          description: "مدرک مایکروسافت ورد Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/phrase/pdf/"
          description: "فرمت مدرک قابل حمل Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/phrase/pptx/"
          description: "ارائه PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/phrase/txt/"
          description: "مدرک متنی"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/phrase/xlsx/"
          description: "جدول محتوای Open XML مایکروسافت اکسل"
  

---