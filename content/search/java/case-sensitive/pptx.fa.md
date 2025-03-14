
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: fa
format: Pptx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "انجام جستجوهای حساس به حروف بزرگ و کوچک در PPTX با Java"
head_description: "رابط برنامه‌نویسی GroupDocs.Search for Java به توسعه‌دهندگان Java کمک می‌کند تا جستجوهای حساس به حروف بزرگ و کوچک را در انواع مختلف مستندات انجام دهند."

############################# Header ############################
title: "جستجوی مستندات حساس به حروف بزرگ و کوچک" 
description: "GroupDocs.Search for Java این امکان را به شما می‌دهد تا قابلیت جستجوی حساس به حروف بزرگ و کوچک را در پروژه‌های Java خود پیاده‌سازی کنید."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دریافت رایگان"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "بیشتر درباره GroupDocs.Search بدانید"
    link: "/search/java/"
    link_title: "بیشتر بیاموزید"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) یک ابزار چندمنظوره برای جستجو و نمایه‌سازی متن در مستندات متنوع است. این محصول از بیش از 70 فرمت مانند PDF، فایل‌های Word، ارائه‌های PowerPoint، صفحات Excel، تصاویر و ZIP پشتیبانی می‌کند و به شما کمک می‌کند تا داده‌های گسترده را به‌طور مؤثر مدیریت کنید.

############################# Steps ############################
steps:
    enable: true
    title: "راهنمای جستجوی حساس به حروف بزرگ و کوچک در فایل‌های PPTX"
    content: |
      با استفاده از [GroupDocs.Search](/search/java/) می‌توانید جستجوهای حساس به حروف بزرگ و کوچک را در مستندات PPTX انجام دهید و پروژه‌های Java خود را بهبود ببخشید.
      
      1. پوشه‌ای برای ذخیره نمایه جستجو تنظیم کنید.
      2. پوشه حاوی فایل‌های PPTX را انتخاب کنید.
      3. جستجوی حساس به حروف بزرگ و کوچک را اجرا کنید و نتایج را جمع‌آوری کنید.
      4. نتایج جستجو را پردازش و استفاده کنید.
   
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
        // محل ذخیره نمایه را مشخص کنید
        Index index = new Index("c:/MyIndex");

        // به پوشه حاوی مستندات برای جستجو اشاره کنید
        index.add("c:/MyDocuments");

        // حالت حساس به حروف بزرگ و کوچک را در تنظیمات جستجو فعال کنید
        SearchOptions options = new SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // جستجو را انجام دهید
        SearchResult result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ابزارهای پیشرفته جستجو و نمایه‌سازی"
  description: "با GroupDocs.Search for Java می‌توانید جستجو و نمایه‌سازی مستندات را برای بیش از 70 فرمت بهینه کنید و پیدا کردن و سازماندهی اطلاعات را تسهیل نمایید."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Search"
  features:
    # feature loop
    - title: "جستجوی انعطاف‌پذیر متن"
      content: "در مستنداتی مانند PDF، فایل‌های Word، صفحات گسترده و ارائه‌ها جستجو کنید. از ابزارهایی مانند تطابق دقیق، جستجوی نادقیق و پشتیبانی از کاراکترهای جایگزین برای بهبود نتایج خود استفاده کنید."

    # feature loop
    - title: "مدیریت مؤثر نمایه"
      content: "داده‌های بزرگ را سازماندهی و نمایه‌گذاری کنید تا سرعت و عملکرد جستجو را هنگام کار با مجموعه‌های مستندات بزرگ بهبود بخشید."

    # feature loop
    - title: "پشتیبانی از زبان‌های جهانی"
      content: "جستجو در بیش از 80 زبان را انجام دهید و از تنوع‌های زبانی و تنظیمات مختلف کیبورد به‌طور دقیق استفاده کنید."

    # feature loop
    - title: "فیلترهای جستجو سفارشی"
      content: "معیارهای جستجو را با گزینه‌هایی مانند حساسیت به حروف بزرگ و کوچک، فیلتر کردن محدوده تاریخ و حذف کلمات یا داده‌های ناخواسته در طول نمایه‌سازی تنظیم کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "مثال: جستجوهای حساس به حروف بزرگ و کوچک"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توان جستجوهای حساس به حروف بزرگ و کوچک را برای مستندات PPTX پیاده‌سازی کرد.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // دایرکتوری برای نمایه جستجو را تعریف کنید
          Index index = new Index("c:/MyIndex");
              
          // محل پوشه مستندات را مشخص کنید
          index.add("c:/MyDocuments");

          // یک پرسش جستجو تنظیم کنید
          SearchQuery wordQuery = SearchQuery.createWordQuery("Lorem");

          // حساسیت به حروف بزرگ و کوچک را در گزینه‌های جستجو فعال کنید
          SearchOptions options = new SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // جستجوی مستندات را انجام دهید
          SearchResult result = index.search(wordQuery, options);
          
          // نتایج به‌دست‌آمده را پردازش کنید
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
            link: "/examples/search/formats/searchcase-sensitive.pptx"
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
    title: "مروری بر ویژگی‌های کلیدی"
    exclude: "case-sensitive"
    description: "توانایی‌های جستجوی قدرتمند و مؤثری که GroupDocs.Search for Java ارائه می‌دهد را کشف کنید."
    items: 
          
        # operation loop 1
        - name: "جستجو با شرط"
          operation: "boolean"
          link: "/search/java/boolean/pptx/"
          description: "یافتن اطلاعات در اسناد با استفاده از شرایط بولی"

        # operation loop 2
        - name: "جستجوی حساس به حروف بزرگ و کوچک"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pptx/"
          description: "دقت جستجو را با در نظر گرفتن حساسیت حروف افزایش دهید"

        # operation loop 3
        - name: "شاخص‌گذاری اسناد"
          operation: "document"
          link: "/search/java/document/pptx/"
          description: "اسناد را یک‌بار شاخص‌گذاری کنید و از شاخص برای جستجوهای متعدد استفاده کنید"

        # operation loop 4
        - name: "فیلترهای جستجو"
          operation: "filters"
          link: "/search/java/filters/pptx/"
          description: "از فیلترها برای محدود کردن داده‌های پردازش‌شده استفاده کنید"

        # operation loop 5
        - name: "عبارت دقیق"
          operation: "phrase"
          link: "/search/java/phrase/pptx/"
          description: "جستجو برای یک جمله یا عبارت خاص"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "فرمت‌های پشتیبانی‌شده برای جستجو"
    exclude: "PPTX"
    description: "GroupDocs.Search با بیش از 70 فرمت مستندات محبوب کار می‌کند و تنظیمات جستجوی قابل تنظیم و نمایه‌سازی مؤثری را ارائه می‌دهد."
    items: 
        # format loop 1
        - name: "جستجوی حساس به حروف بزرگ و کوچک DOCX"
          format: "DOCX"
          link: "/search/java/case-sensitive/docx/"
          description: "سند XML باز مایکروسافت ورد"
          
        # format loop 2
        - name: "جستجوی حساس به حروف بزرگ و کوچک PDF"
          format: "PDF"
          link: "/search/java/case-sensitive/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 3
        - name: "جستجوی حساس به حروف بزرگ و کوچک PPTX"
          format: "PPTX"
          link: "/search/java/case-sensitive/pptx/"
          description: "ارائه XML باز پاورپوینت"

        # format loop 4
        - name: "جستجوی حساس به حروف بزرگ و کوچک TXT"
          format: "TXT"
          link: "/search/java/case-sensitive/txt/"
          description: "سند متنی"
          
        # format loop 5
        - name: "جستجوی حساس به حروف بزرگ و کوچک XLSX"
          format: "XLSX"
          link: "/search/java/case-sensitive/xlsx/"
          description: "برگه XML باز مایکروسافت اکسل"
  

---