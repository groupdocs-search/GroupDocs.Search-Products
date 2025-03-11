
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:39
draft: false
lang: fa
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "جستجوی عبارات در XLSX با استفاده از Java"
head_description: "GroupDocs.Search for Java توانایی‌های جستجوی پیشرفته عبارات را برای محتوای اسناد به برنامه‌های Java اضافه می‌کند."

############################# Header ############################
title: "یافتن عبارات در اسناد" 
description: "به سرعت عبارات خاص را با GroupDocs.Search for Java پیدا کنید. قابلیت‌های جستجوی قوی را به برنامه‌های Java خود اضافه کنید."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دانلود"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "ویژگی‌های GroupDocs.Search"
    link: "/search/java/"
    link_title: "بیشتر بدانید"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) یک کتابخانه‌ی قوی برای ایندکس‌گذاری و جستجو در متن اسناد است. این کتابخانه از بیش از ۷۰ فرمت فایل، از جمله PDFها، اسناد Word، صفحه‌گسترده‌های Excel، تصاویر و فایل‌های ZIP پشتیبانی می‌کند و نتایج جستجوی سریع و دقیقی را تضمین می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه عبارات را در اسناد XLSX پیدا کنیم"
    content: |
      [GroupDocs.Search](/search/java/) جستجوی عبارات را در اسناد XLSX ساده می‌کند. از گزینه‌های مختلف برای بهبود نتایج جستجو در برنامه‌های Java استفاده کنید.
      
      1. یک دایرکتوری برای ایندکس جستجو ایجاد کنید.
      2. پوشه حاوی فایل‌های XLSX را تعیین کنید.
      3. پارامترهای جستجو را تنظیم کنید.
      4. نتایج جستجو را بازیابی و تجزیه و تحلیل کنید.
   
    code:
      platform: "java"
      copy_title: "کپی"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
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
        // مسیر ایندکس جستجو را مشخص کنید
        Index index = new Index("c:/MyIndex");

        // پوشه حاوی اسناد را تعیین کنید
        index.add("c:/MyDocuments");

        // تنظیمات جستجو را مشخص کنید
        SearchQuery word1 = SearchQuery.createWordQuery("lorem");
        SearchQuery word2 = SearchQuery.createWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.createWordQuery("dolor");

        SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, word2, word3);
        
        // کوئری جستجو را اجرا کنید
        SearchResult result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "کشف موتور جستجوی اسناد Java"
  description: "GroupDocs.Search for Java این قابلیت را دارد که در بیش از ۷۰ فرمت فایل جستجو انجام دهد. داده‌ها را با استفاده از ویژگی‌های پیشرفته جستجو پیدا و سازماندهی کنید."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "قابلیت‌های کلیدی GroupDocs.Search"
  features:
    # feature loop
    - title: "جستجوی عبارات"
      content: "عبارات دقیق را در اسناد تجاری، مانند PDFها، فایل‌های Word، ارائه‌ها و صفحه‌گسترده‌ها پیدا کنید. از کاراکترهای جایگزین و گزینه‌های دیگر وقتی عبارت دقیق مشخص نیست استفاده کنید."

    # feature loop
    - title: "ایندکس‌گذاری بهینه داده‌ها"
      content: "با ایجاد و استفاده مجدد از ایندکس‌های جستجو، جستجو در اسناد را تسریع کنید. ایندکس‌گذاری داده‌ها را به‌طور مؤثری سازماندهی می‌کند تا جستجوی سریع‌تر و دقیق‌تری را امکان‌پذیر کند."

    # feature loop
    - title: "سازگاری چندزبانه"
      content: "در بیش از ۸۰ زبان در اسناد جستجو کنید. از طرح‌های مختلف صفحه‌کلید و تجزیه و تحلیل ریخت‌شناختی برای بهبود دقت جستجو پشتیبانی می‌کند."

    # feature loop
    - title: "گزینه‌های جستجوی پیشرفته"
      content: "جستجوها را با حساسیت به حروف، جستجوی فازی، تطابق هم‌صدا، فیلتر کردن اسناد و سایر ویژگی‌های قدرتمند سفارشی کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "استفاده از روش‌های جستجوی پیشرفته"
      content: |
        یاد بگیرید چگونه کوئری‌ها را برای جستجو در XLSX بسازید.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // دایرکتوری ایندکس جستجو را تعریف کنید
          Index index = new Index("c:/MyIndex");
              
          // مسیر به اسناد هدف را تنظیم کنید
          index.add("c:/MyDocuments");

          // یک کوئری جستجو برای یک عبارت خاص ایجاد کنید
          SearchQuery word1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.createWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.createWordQuery("dolor");

          SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // نتایج جستجو را بازیابی کنید
          SearchResult result = index.search(query);
          
          // نتایج بازیابی‌شده را پردازش و استفاده کنید
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
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchphrase.xlsx"
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
  description: "امکانات GroupDocs.Search را به صورت رایگان امتحان کنید یا درخواست مجوز دهید"
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
    title: "قابلیت‌های جستجوی پیشرفته"
    exclude: "phrase"
    description: "از قابلیت‌های جستجوی پیشرفته برای بهبود دقت و عملکرد استفاده کنید."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/xlsx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/xlsx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/xlsx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/xlsx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/xlsx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "جستجوی عبارات در اسناد تجاری"
    exclude: "XLSX"
    description: "GroupDocs.Search امکان جستجوی عبارات در بیش از ۷۰ فرمت سند را فراهم می‌کند. از گزینه‌های پیشرفته و ایندکس‌گذاری برای جستجوهای مؤثر استفاده کنید."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/phrase/docx/"
          description: "مدرک مایکروسافت ورد Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/phrase/pdf/"
          description: "فرمت مدرک قابل حمل Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/phrase/pptx/"
          description: "ارائه PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/phrase/txt/"
          description: "مدرک متنی"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/phrase/xlsx/"
          description: "جدول محتوای Open XML مایکروسافت اکسل"
  

---