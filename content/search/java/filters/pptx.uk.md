
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: uk
format: Pptx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Пошук у документах PPTX з використанням Java"
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
    title: "Як шукати в документах PPTX"
    content: |
      [GroupDocs.Search](/search/java/) дозволяє швидко і ефективно шукати текст у документах PPTX, ідеально підходячи для додатків Java.
      
      1. Вкажіть папку для зберігання пошукового індексу.
      2. Виберіть папку, що містить ваші документи.
      3. Налаштуйте параметри пошуку, щоб обмежити результати до документів PPTX.
      4. Запустіть пошук і отримайте результати.
   
    code:
      platform: "java"
      copy_title: "Копіювати"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Результат пошуку"
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
        copy_tip: "клікніть, щоб скопіювати"
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
            SearchDocumentFilter.createFileExtension(".pptx");

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
          copy_tip: "клікніть, щоб скопіювати"
          copy_done: "скопійовано"
        top_links:
          #  loop
          - title: "Завантажити результат"
            icon: "download"
            link: "/examples/search/formats/searchfilters.pptx"
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
  title: "Готові розпочати?"
  description: "Спробуйте функції GroupDocs.Search безкоштовно або запитайте ліцензію"
  items:
    #  loop
    - title: "Завантажити Maven"
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
        - name: "Пошук за умовою"
          operation: "boolean"
          link: "/search/java/boolean/pptx/"
          description: "Знайти інформацію в документах, використовуючи логічні умови"

        # operation loop 2
        - name: "Пошук чутливий до регістру"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pptx/"
          description: "Покращте точність пошуку, враховуючи чутливість до регістру"

        # operation loop 3
        - name: "Індексація документів"
          operation: "document"
          link: "/search/java/document/pptx/"
          description: "Індексуйте документи один раз та повторно використовуйте індекс для кількох пошуків"

        # operation loop 4
        - name: "Фільтри пошуку"
          operation: "filters"
          link: "/search/java/filters/pptx/"
          description: "Використовуйте фільтри для звуження оброблюваних даних"

        # operation loop 5
        - name: "Точна фраза"
          operation: "phrase"
          link: "/search/java/phrase/pptx/"
          description: "Шукайте конкретне речення або фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Пошук у бізнес-документах"
    exclude: "PPTX"
    description: "GroupDocs.Search підтримує більше 70 форматів файлів, що забезпечує можливість пошуку в широко використовуваних офісних документах."
    items: 
        # format loop 1
        - name: "Фільтри для пошуку у DOCX"
          format: "DOCX"
          link: "/search/java/filters/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Фільтри для пошуку у PDF"
          format: "PDF"
          link: "/search/java/filters/pdf/"
          description: "Формат Adobe Portable Document"
          
        # format loop 3
        - name: "Фільтри для пошуку у PPTX"
          format: "PPTX"
          link: "/search/java/filters/pptx/"
          description: "Презентація PowerPoint Open XML"

        # format loop 4
        - name: "Фільтри для пошуку у TXT"
          format: "TXT"
          link: "/search/java/filters/txt/"
          description: "Текстовий документ"
          
        # format loop 5
        - name: "Фільтри для пошуку у XLSX"
          format: "XLSX"
          link: "/search/java/filters/xlsx/"
          description: "Таблиця Microsoft Excel Open XML"
  

---