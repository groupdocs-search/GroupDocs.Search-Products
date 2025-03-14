
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:50
draft: false
lang: fa
format: Pdf
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "جستجو در مدارک PDF با استفاده از Java"
head_description: "GroupDocs.Search for Java به برنامه‌های Java امکان جستجوی متنی قدرتمند را اضافه می‌کند و از فرمت‌های مختلف مدارک تجاری پشتیبانی می‌کند."

############################# Header ############################
title: "یافتن متن در مدارک تجاری" 
description: "GroupDocs.Search for Java به شما این امکان را می‌دهد که با استفاده از پرس و جوهای انعطاف‌پذیر و دقیق، متن را در مدارک جستجو کنید. عملکرد جستجو را به راحتی در برنامه‌های Java خود یکپارچه کنید."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود رایگان"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search چیست؟"
    link: "/search/java/"
    link_title: "بیشتر بیاموزید"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) یک کتابخانه قوی برای جستجوی سریع متن و فهرست‌سازی مدارک است. این کتابخانه از بیش از 70 فرمت فایل، از جمله استانداردهای صنعتی مانند PDF، Word، Excel و PowerPoint پشتیبانی می‌کند. برنامه‌های خود را با قابلیت‌های جستجو سریع و دقیق بهبود دهید.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه در مدارک PDF جستجو کنیم"
    content: |
      [GroupDocs.Search](/search/java/) امکان جستجوهای سریع و کارآمد متن در مدارک PDF را فراهم می‌کند که برای برنامه‌های Java ایده‌آل است.
      
      1. یک پوشه برای ذخیره فهرست جستجو مشخص کنید.
      2. پوشه‌ای را که شامل مدارک شما است انتخاب کنید.
      3. گزینه‌های جستجو را پیکربندی کنید تا نتایج به مدارک PDF محدود شود.
      4. جستجو را اجرا کرده و نتایج را دریافت کنید.
   
    code:
      platform: "java"
      copy_title: "کپی"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "نتیجه جستجو"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-search</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "برای کپی کلیک کنید"
        copy_done: "کپی شد"
      links:
        #  loop
        - title: "مثال‌های بیشتر"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "مستندات"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // مسیر برای ذخیره فهرست جستجوی قابل استفاده مجدد
        Index index = new Index("c:/MyIndex");

        // پوشه‌ای که شامل مدارک است
        index.add("c:/MyDocuments");

        // فیلتر کردن جستجوها بر اساس فرمت مدارک
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.createFileExtension(".pdf");

        // دریافت نتایج جستجو
        SearchResult result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "قابلیت‌های جستجوی پیشرفته"
  description: "GroupDocs.Search for Java جستجوی متنی پیشرفته‌ای را در بیش از 70 فرمت فایل ارائه می‌دهد. فهرست‌سازی، جستجوها را سرعت می‌بخشد و کارایی مدیریت مدارک را افزایش می‌دهد."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Search"
  features:
    # feature loop
    - title: "جستجوی متنی قدرتمند"
      content: "یافتن متن در فرمت‌های محبوب مدارک مانند PDF، فایل‌های Word، ارایه‌ها و صفحه‌گسترده‌ها. از روش‌های جستجوی متعدد از جمله جستجوی فازی، هم‌صدایی و کاراکترهای جایگزین پشتیبانی می‌کند."

    # feature loop
    - title: "فهرست‌گذاری بهینه شده برای عملکرد بهتر"
      content: "ایجاد و استفاده مجدد از فهرست‌های جستجو برای افزایش سرعت و کارایی جستجو، به ویژه در مجموعه‌های بزرگ مدارک."

    # feature loop
    - title: "پشتیبانی از جستجوی چند زبانه"
      content: "جستجو در مدارکی که به بیش از 80 زبان نوشته شده‌اند. تشخیص چیدمان‌های صفحه‌کلید مختلف و واریسیون‌های کلمات برای دقت بیشتر."

    # feature loop
    - title: "گزینه‌های جستجوی قابل تنظیم"
      content: "نتایج جستجو را با فیلترها، عبارات منظم و سایر تنظیمات جستجوی پیشرفته محدود کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "فیلتر مدارک قبل از جستجو"
      content: |
        یاد بگیرید چگونه با استفاده از فیلترها جستجوها را پالایش کنید
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // راه‌اندازی فهرستی که برخی فرمت‌های فایل را استثنا می‌کند
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new Index("c:/MyIndex", settings);
              
          // مشخص کردن مسیر ذخیره‌سازی مدارک
          index.add("c:/MyDocuments");

          // دریافت نتایج جستجو
          SearchResult result = index.search("Lorem", options);
          
          // فرآیند و استفاده از نتایج جستجو
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "کپی"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-search</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "برای کپی کلیک کنید"
          copy_done: "کپی شد"
        top_links:
          #  loop
          - title: "دانلود نتیجه"
            icon: "download"
            link: "/examples/search/formats/searchfilters.pdf"
        links:
          #  loop
          - title: "مثال‌های بیشتر"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "مستندات"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "آماده شروع هستید؟"
  description: "ویژگی‌های GroupDocs.Search را رایگان امتحان کنید یا درخواست مجوز دهید"
  items:
    #  loop
    - title: "دانلود Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "مجوزدهی"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "ویژگی‌های کلیدی"
    exclude: "filters"
    description: "انجام جستجوهای دقیق و کارآمد متن."
    items: 
          
        # operation loop 1
        - name: "جستجو با شرط"
          operation: "boolean"
          link: "/search/java/boolean/pdf/"
          description: "یافتن اطلاعات در اسناد با استفاده از شرایط بولی"

        # operation loop 2
        - name: "جستجوی حساس به حروف بزرگ و کوچک"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pdf/"
          description: "دقت جستجو را با در نظر گرفتن حساسیت حروف افزایش دهید"

        # operation loop 3
        - name: "شاخص‌گذاری اسناد"
          operation: "document"
          link: "/search/java/document/pdf/"
          description: "اسناد را یک‌بار شاخص‌گذاری کنید و از شاخص برای جستجوهای متعدد استفاده کنید"

        # operation loop 4
        - name: "فیلترهای جستجو"
          operation: "filters"
          link: "/search/java/filters/pdf/"
          description: "از فیلترها برای محدود کردن داده‌های پردازش‌شده استفاده کنید"

        # operation loop 5
        - name: "عبارت دقیق"
          operation: "phrase"
          link: "/search/java/phrase/pdf/"
          description: "جستجو برای یک جمله یا عبارت خاص"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "جستجو در مدارک تجاری"
    exclude: "PDF"
    description: "GroupDocs.Search از بیش از 70 فرمت فایل پشتیبانی می‌کند و جستجو در مدارک اداری پرکاربرد را آسان می‌سازد."
    items: 
        # format loop 1
        - name: "فیلترهای جستجو برای DOCX"
          format: "DOCX"
          link: "/search/java/filters/docx/"
          description: "سند XML باز مایکروسافت ورد"
          
        # format loop 2
        - name: "فیلترهای جستجو برای PDF"
          format: "PDF"
          link: "/search/java/filters/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 3
        - name: "فیلترهای جستجو برای PPTX"
          format: "PPTX"
          link: "/search/java/filters/pptx/"
          description: "ارائه XML باز پاورپوینت"

        # format loop 4
        - name: "فیلترهای جستجو برای TXT"
          format: "TXT"
          link: "/search/java/filters/txt/"
          description: "سند متنی"
          
        # format loop 5
        - name: "فیلترهای جستجو برای XLSX"
          format: "XLSX"
          link: "/search/java/filters/xlsx/"
          description: "برگه XML باز مایکروسافت اکسل"
  

---