
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:34
draft: false
lang: fa
format: Txt
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "یافتن متن در اسناد TXT با GroupDocs.Search برای Java"
head_description: "GroupDocs.Search for Java به توسعه‌دهندگان Java کمک می‌کند تا به‌سرعت متن را در فرمت‌های مختلف اسنادی جستجو کنند."

############################# Header ############################
title: "جستجوی هوشمند متن مستندات" 
description: "با GroupDocs.Search for Java، می‌توانید به‌راحتی متن را از انواع مختلف اسناد در برنامه‌های Java خود جستجو و استخراج کنید."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "دریافت نسخه آزمایشی رایگان"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "وظیفه GroupDocs.Search چیست؟"
    link: "/search/java/"
    link_title: "بیشتر بدانید"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) یک کتابخانه جستجو و فهرست‌سازی اسناد قدرتمند است که از بیش از 70 فرمت فایل، از جمله PDF، Word، PowerPoint، Excel، تصاویر و آرشیوهای ZIP پشتیبانی می‌کند. این امکان را برای جستجوی سریع، دقیق و مقیاس‌پذیر در مجموعه‌های بزرگ اسناد فراهم می‌کند.

############################# Steps ############################
steps:
    enable: true
    title: "انجام جستجوهای متنی در فایل‌های TXT"
    content: |
      [GroupDocs.Search](/search/java/) این امکان را برای جستجوی فایل‌های TXT با استفاده از منطق و فهرست‌سازی پیچیده فراهم می‌کند و دقت جستجو را در برنامه‌های Java بهبود می‌بخشد.
      
      1. دایرکتوری را برای ذخیره فهرست جستجو تنظیم کنید.
      2. پوشه‌ای را که شامل فایل‌های TXT است انتخاب کنید.
      3. گزینه‌های جستجو اضافی را تعریف کنید.
      4. جستجو را اجرا کرده و نتایج را تجزیه و تحلیل کنید.
   
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
        // دایرکتوری را برای ذخیره فهرست جستجو تنظیم کنید
        Index index = new Index("c:/MyIndex");

        // پوشه‌ای که شامل اسناد قابل جستجو است را مشخص کنید
        index.add("c:/MyDocuments");

        // جستجوی هم‌صدایی را برای مطابقت کلمات با تلفظ مشابه فعال کنید
        SearchOptions options = new SearchOptions();
        options.setUseHomophoneSearch(true);

        // یک پرسش جستجوی پیشرفته را اجرا کنید
        SearchResult result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "قابلیت‌های پیشرفته جستجو و فهرست‌سازی"
  description: "GroupDocs.Search for Java جستجوی متن و فهرست‌سازی را در بیش از 70 فرمت اسنادی ساده کرده و ابزارهای کارآمدی برای مدیریت و بازیابی اطلاعات به‌سرعت فراهم می‌کند."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "قابلیت‌های اصلی GroupDocs.Search"
  features:
    # feature loop
    - title: "جستجوی جامع متن"
      content: "متن را در فرمت‌های مختلف اسنادی مانند PDF، اسناد Word، ارائه‌های PowerPoint و اکسل پیدا کنید. از تطابق‌های دقیق، جستجوی تقریبی و عملگرهای wildcard برای دستیابی به نتایج جستجوی دقیق استفاده کنید."

    # feature loop
    - title: "فهرست‌سازی بهینه برای داده‌های بزرگ"
      content: "فهرست‌های ساختاری ایجاد کنید تا جستجوها را تسریع کنید و به‌راحتی از طریق مخزن‌های بزرگ اسنادی به‌صورت کارآمد پیمایش کنید."

    # feature loop
    - title: "پشتیبانی از زبان‌های متعدد"
      content: "جستجوها را در بیش از 80 زبان با پشتیبانی داخلی از چیدمان‌های صفحه‌کلید و تغییرات مورفولوژی کلمات انجام دهید که دقت را بهبود می‌بخشد."

    # feature loop
    - title: "تنظیمات جستجوی انعطاف‌پذیر"
      content: "جستجوها را با گزینه‌هایی مانند حساسیت به حروف بزرگ و کوچک، فیلتر بر اساس تاریخ و قابلیت حذف کلمات خاص برای دستیابی به نتایج دقیق سفارشی‌سازی کنید."
      
  code_samples_ext:
    # code sample ext loop
    - title: "پیاده‌سازی پرسش‌های جستجوی پیشرفته"
      content: |
        این مثال نشان می‌دهد که چگونه می‌توان از پرسش‌های جستجو برای جستجو در اسناد TXT به‌طور مؤثر استفاده کرد.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // دایرکتوری را برای فهرست‌سازی جستجو تعریف کنید
          Index index = new Index("c:/MyIndex");
              
          // مسیر فایل اسناد را ارائه دهید
          index.add("c:/MyDocuments");

          // رمز عبور اسناد رمزگذاری‌شده را وارد کنید
          index.getDictionaries().getDocumentPasswords().add("protected.txt", "123456");

          // جستجوی تقریبی را برای تشخیص کلمات مشابه فعال کنید
          SearchOptions options = new SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8));

          // نتایج جستجو را دریافت کنید
          SearchResult result = index.Search("Loarem", options);
          
          // نتایج جستجو را پردازش و تجزیه و تحلیل کنید
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
            link: "/examples/search/formats/searchdocument.txt"
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
    title: "مروری بر ویژگی‌های کلیدی"
    exclude: "document"
    description: "با عملکردهای جستجوی متنی با عملکرد بالا، طراحی شده برای کارایی و دقت، آشنا شوید."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/txt/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/txt/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/txt/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/txt/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/txt/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "یافتن اطلاعات در اسناد TXT با GroupDocs.Search"
    exclude: "TXT"
    description: "GroupDocs.Search از بیش از 70 فرمت پشتیبانی می‌کند که شامل فایل‌های اداری بوده و امکان جستجوهای سریع با قابلیت‌های پیشرفته فهرست‌سازی را فراهم می‌کند."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/document/docx/"
          description: "مدرک مایکروسافت ورد Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/document/pdf/"
          description: "فرمت مدرک قابل حمل Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/document/pptx/"
          description: "ارائه PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/document/txt/"
          description: "مدرک متنی"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/document/xlsx/"
          description: "جدول محتوای Open XML مایکروسافت اکسل"
  

---