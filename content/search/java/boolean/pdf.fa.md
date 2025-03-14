
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:45
draft: false
lang: fa
format: Pdf
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "جستجوی بولی در PDF با Java"
head_description: "با GroupDocs.Search for Java، توسعه‌دهندگان می‌توانند جستجوهای مستند را با استفاده از عملگرهای بولی مانند AND، OR و NOT انجام دهند."

############################# Header ############################
title: "جستجوی متنی بولی" 
description: "از GroupDocs.Search for Java برای ایجاد کوئری‌های پیشرفته جستجوی بولی (AND، OR، NOT) در پروژه‌های Java خود استفاده کنید."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "رایگان دانلود کنید"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "درباره GroupDocs.Search"
    link: "/search/java/"
    link_title: "بیشتر بیاموزید"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) یک کتابخانه چندمنظوره است که برای جستجوی متن و ایندکس‌گذاری داده‌ها در اسناد طراحی شده است. این کتابخانه از بیش از 70 نوع فایل استفاده می‌کند، از جمله PDF، Word، Excel، تصاویر PowerPoint و آرشیوهای ZIP، که جستجوهای کارآمدی را در مجموعه‌های داده بزرگ فراهم می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "چگونه جستجوهای بولی را در مستندات PDF انجام دهیم"
    content: |
      [GroupDocs.Search](/search/java/) جستجوهای متنی را در مستندات PDF ممکن می‌سازد. با پشتیبانی از شرایط بولی، می‌توانید دقت جستجو را در برنامه‌های Java خود افزایش دهید.
      
      1. پوشه‌ای را برای ذخیره ایندکس جستجو مشخص کنید.
      2. پوشه‌ای را که شامل مستندات PDF است انتخاب کنید.
      3. کوئری جستجو را اجرا کرده و نتایج را بازیابی کنید.
      4. نتایج به‌دست‌آمده را پردازش کنید.
   
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
        // مسیر پوشه ایندکس را تنظیم کنید
        Index index = new Index("c:/MyIndex");

        // مسیر پوشه‌ای را که شامل مستندات برای جستجو است ارائه دهید
        index.add("c:/MyDocuments");

        // با یک کوئری پیچیده جستجو را انجام دهید
        SearchResult result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ابزارهای قدرتمند برای جستجو و ایندکس‌گذاری اسناد"
  description: "GroupDocs.Search for Java جستجوهای متنی و ایندکس‌گذاری داده‌ها را برای بیش از 70 فرمت ساده می‌کند. ابزارهای پیشرفته این کتابخانه به شما امکان می‌دهد محتوا را به سادگی پیدا و مدیریت کنید."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "ویژگی‌های کلیدی GroupDocs.Search"
  features:
    # feature loop
    - title: "جستجوی جامع متنی"
      content: "در چندین فرمت مانند PDF، اسناد Word، ارائه‌ها، صفحات گسترده و بیشتر جستجو کنید. از گزینه‌هایی مانند تطابق دقیق، جستجوی نامشخص و کوئری‌های wildcard برای تصحیح نتایج استفاده کنید."

    # feature loop
    - title: "ایندکس‌گذاری داده‌های کارآمد"
      content: "ایندکس‌هایی برای جستجوهای سریع‌تر در اسناد ایجاد و نگهداری کنید. این ویژگی داده‌ها را به‌صورت کارآمد سازماندهی می‌کند و مدیریت مجموعه‌های بزرگ مستندات را آسان‌تر می‌سازد."

    # feature loop
    - title: "پشتیبانی از چندین زبان"
      content: "در اسناد نوشته شده به بیش از 80 زبان جستجو کنید. با بهره‌برداری از اشکال کلمه‌ای مورفولوژیک و طرح‌های مختلف صفحه‌کلید، دقت را افزایش دهید."

    # feature loop
    - title: "سفارشی‌سازی جستجوهای انعطاف‌پذیر"
      content: "تنظیمات جستجو را با ویژگی‌هایی مانند حساسیت به حروف بزرگ و کوچک، فیلترهای تاریخ، و استثناها تنظیم کنید تا نتایج خود را دقیق‌تر کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "استفاده از کوئری‌های جستجوی بولی پیچیده"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توان جستجوهای بولی را در فایل‌های PDF انجام داد.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // پوشه را برای ایندکس جستجو تنظیم کنید
          Index index = new Index("c:/MyIndex");
              
          // مسیر را به مستندات برای جستجو ارائه دهید
          index.add("c:/MyDocuments");

          // کوئری را با استفاده از منطق بولی بسازید
          SearchQuery wordQuery1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.createWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // نتایج جستجو را بازیابی کنید
          SearchResult result = index.search(booleanQuery);
          
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
            link: "/examples/search/formats/searchboolean.pdf"
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
    title: "ویژگی‌های کلیدی در یک نگاه"
    exclude: "boolean"
    description: "قابلیت‌های جستجوی قدرتمند و کارآمد را باز کنید"
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
    title: "جستجوی فرمت‌های محبوب مستندات"
    exclude: "PDF"
    description: "GroupDocs.Search از بیش از 70 نوع فایل پشتیبانی می‌کند و به شما امکان می‌دهد قوانین جستجو را سفارشی کنید و با استفاده از ایندکس‌گذاری، عملکرد را بهینه کنید."
    items: 
        # format loop 1
        - name: "جستجوی بولی در DOCX"
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "سند XML باز مایکروسافت ورد"
          
        # format loop 2
        - name: "جستجوی بولی در PDF"
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "فرمت سند قابل حمل Adobe"
          
        # format loop 3
        - name: "جستجوی بولی در PPTX"
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "ارائه XML باز پاورپوینت"

        # format loop 4
        - name: "جستجوی بولی در TXT"
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "سند متنی"
          
        # format loop 5
        - name: "جستجوی بولی در XLSX"
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "برگه XML باز مایکروسافت اکسل"
  

---