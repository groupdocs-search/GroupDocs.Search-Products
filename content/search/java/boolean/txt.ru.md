
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:29
draft: false
lang: ru
format: Txt
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Булевый поиск в TXT с Java"
head_description: "С помощью GroupDocs.Search for Java разработчики могут выполнять поиск по документам с использованием булевых операторов, таких как AND, OR и NOT."

############################# Header ############################
title: "Булевый текстовый поиск" 
description: "Используйте GroupDocs.Search for Java для создания сложных булевых (AND, OR, NOT) запросов поиска в ваших проектах Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачать бесплатно"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "О GroupDocs.Search"
    link: "/search/java/"
    link_title: "Узнать больше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) - это универсальная библиотека, предназначенная для текстового поиска и индексации данных в документах. Она поддерживает более 70 форматов файлов, включая PDF, Word, Excel, PowerPoint, изображения и ZIP-архивы, что позволяет эффективно осуществлять поиск по большим объемам данных.

############################# Steps ############################
steps:
    enable: true
    title: "Как выполнять булевые поиски в документах TXT"
    content: |
      [GroupDocs.Search](/search/java/) позволяет выполнять текстовые поиски в документах TXT. Поддержка булевых условий помогает повысить точность поиска в приложениях Java.
      
      1. Укажите папку для хранения индекса поиска.
      2. Выберите папку с документами TXT.
      3. Выполните поисковой запрос и получите результаты.
      4. Обработайте полученные результаты.
   
    code:
      platform: "java"
      copy_title: "Копировать"
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
        copy_tip: "нажмите, чтобы скопировать"
        copy_done: "скопировано"
      links:
        #  loop
        - title: "Больше примеров"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "Документация"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // Установите путь к папке индекса
        Index index = new Index("c:/MyIndex");

        // Укажите путь к папке, содержащей документы для поиска
        index.add("c:/MyDocuments");

        // Выполните поиск с помощью сложного запроса
        SearchResult result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Мощные инструменты для поиска и индексации документов"
  description: "GroupDocs.Search for Java упрощает текстовые поиски и индексацию данных для более чем 70 форматов. Его расширенные инструменты позволяют находить и управлять содержимым эффективно."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Ключевые функции GroupDocs.Search"
  features:
    # feature loop
    - title: "Полный текстовый поиск"
      content: "Выполняйте поиск по множеству форматов, таких как PDF, документы Word, презентации, таблицы и другим. Используйте такие опции, как точное соответствие, нечеткий поиск и запросы с подстановочными знаками для уточнения результатов."

    # feature loop
    - title: "Эффективная индексация данных"
      content: "Создавайте и поддерживайте индексы для более быстрого поиска документов. Эта функция организует данные эффективно, позволяя легко работать с большими коллекциями документов."

    # feature loop
    - title: "Поддержка нескольких языков"
      content: "Ищите в документах, написанных более чем на 80 языках. Повышайте точность, используя морфологические формы слов и различные раскладки клавиатуры."

    # feature loop
    - title: "Гибкая настройка поиска"
      content: "Настраивайте параметры поиска с помощью таких функций, как чувствительность к регистру, фильтры по диапазону дат и исключения для уточнения результатов."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Использование сложных булевых запросов"
      content: |
        Этот пример демонстрирует, как выполнять булевые поиски в файлах TXT.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Установите папку для индекса поиска
          Index index = new Index("c:/MyIndex");
              
          // Укажите путь к документам для поиска
          index.add("c:/MyDocuments");

          // Составьте запрос с использованием булевой логики
          SearchQuery wordQuery1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.createWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Получите результаты поиска
          SearchResult result = index.search(booleanQuery);
          
          // Обработайте полученные результаты
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "Копировать"
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
          copy_tip: "нажмите, чтобы скопировать"
          copy_done: "скопировано"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchboolean.txt"
        links:
          #  loop
          - title: "Больше примеров"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "Документация"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Готовы начать?"
  description: "Попробуйте возможности GroupDocs.Search бесплатно или запросите лицензию"
  items:
    #  loop
    - title: "Скачивание Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Лицензирование"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Ключевые функции в одном взгляде"
    exclude: "boolean"
    description: "Разблокируйте мощные и эффективные возможности поиска"
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
    title: "Поиск популярных форматов документов"
    exclude: "TXT"
    description: "GroupDocs.Search поддерживает более 70 форматов файлов, позволяя вам настраивать правила поиска и использовать индексацию для оптимизации производительности."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---