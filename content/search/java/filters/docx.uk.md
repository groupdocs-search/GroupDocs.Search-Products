
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:36
draft: false
lang: uk
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Пошук у документах DOCX з використанням Java"
head_description: "GroupDocs.Search for Java додає потужний текстовий пошук до додатків Java, підтримуючи різні формати бізнес-документів."

############################# Header ############################
title: "Знайти текст у бізнес-документах" 
description: "GroupDocs.Search for Java дозволяє шукати текст у документах з використанням гнучких і точних запитів. Інтегруйте функціональність пошуку у додатки Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Завантажити безкоштовно"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Що таке GroupDocs.Search?"
    link: "/search/java/"
    link_title: "Дізнатися більше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) — це надійна бібліотека для швидкого пошуку тексту та індексування документів. Вона підтримує більше 70 форматів файлів, включаючи галузеві стандарти, такі як PDF, Word, Excel та PowerPoint. Покращте свої додатки можливостями високошвидкісного та точного пошуку.

############################# Steps ############################
steps:
    enable: true
    title: "Як шукати в документах DOCX"
    content: |
      [GroupDocs.Search](/search/java/) дозволяє швидко і ефективно шукати текст у документах DOCX, ідеально підходячи для додатків Java.
      
      1. Вкажіть папку для зберігання пошукового індексу.
      2. Виберіть папку, що містить ваші документи.
      3. Налаштуйте параметри пошуку, щоб обмежити результати до документів DOCX.
      4. Запустіть пошук і отримайте результати.
   
    code:
      platform: "java"
      copy_title: "Копіювати"
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
        copy_tip: "клікніть для копіювання"
        copy_done: "скопійовано"
      links:
        #  loop
        - title: "Більше прикладів"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "Документація"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // Директорія для зберігання багаторазового пошукового індексу
        Index index = new Index("c:/MyIndex");

        // Папка, що містить документи
        index.add("c:/MyDocuments");

        // Фільтруйте пошук за форматом документа
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.createFileExtension(".docx");

        // Отримайте результати пошуку
        SearchResult result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Розширені можливості пошуку"
  description: "GroupDocs.Search for Java надає розширений текстовий пошук серед більш ніж 70 форматів файлів. Індексація пришвидшує пошук і підвищує ефективність управління документами."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Ключові функції GroupDocs.Search"
  features:
    # feature loop
    - title: "Потужний текстовий пошук"
      content: "Знайдіть текст у популярних форматах документів, таких як PDF, файли Word, презентації та електронні таблиці. Підтримує декілька методів пошуку, включаючи нечіткий пошук, омоніми та заміщення."

    # feature loop
    - title: "Оптимізоване індексування для кращої продуктивності"
      content: "Створюйте та повторно використовуйте пошукові індекси для підвищення швидкості та ефективності пошуку, особливо в великих колекціях документів."

    # feature loop
    - title: "Підтримка багатомовного пошуку"
      content: "Шукайте у документах, написаних більш ніж 80 мовами. Визначає різні розкладки клавіатури та варіації слів для покращення точності."

    # feature loop
    - title: "Налаштовувані параметри пошуку"
      content: "Звужуйте результати пошуку за допомогою фільтрів, регулярних виразів та інших розширених налаштувань пошуку."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Фільтрація документів перед пошуком"
      content: |
        Дізнайтеся, як уточнити пошук за допомогою фільтрів
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Налаштуйте індекс, який виключає певні формати файлів
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new Index("c:/MyIndex", settings);
              
          // Вкажіть шлях до зберігання документів
          index.add("c:/MyDocuments");

          // Отримайте результати пошуку
          SearchResult result = index.search("Lorem", options);
          
          // Обробіть і використовуйте результати пошуку
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "Копіювати"
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
          copy_tip: "клікніть для копіювання"
          copy_done: "скопійовано"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchfilters.docx"
        links:
          #  loop
          - title: "Більше прикладів"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "Документація"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Готові почати?"
  description: "Спробуйте функції GroupDocs.Search безкоштовно або запитайте ліцензію"
  items:
    #  loop
    - title: "завантаження Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Ліцензування"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Ключові функції"
    exclude: "filters"
    description: "Виконуйте точні та ефективні текстові пошуки."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Пошук у бізнес-документах"
    exclude: "DOCX"
    description: "GroupDocs.Search підтримує більше 70 форматів файлів, що забезпечує можливість пошуку в широко використовуваних офісних документах."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/filters/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/filters/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/filters/pptx/"
          description: "Презентація PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/filters/txt/"
          description: "Текстовий документ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/filters/xlsx/"
          description: "Таблиця Microsoft Excel Open XML"
  

---