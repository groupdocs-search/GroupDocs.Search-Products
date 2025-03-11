
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:39
draft: false
lang: ru
format: Pptx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Поиск фраз в PPTX с помощью Java"
head_description: "GroupDocs.Search for Java улучшает приложения Java мощными возможностями поиска фраз в содержимом документов."

############################# Header ############################
title: "Найдите фразы в документах" 
description: "Быстро находите определенные фразы с помощью GroupDocs.Search for Java. Добавьте мощный функционал поиска в ваши приложения Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачать"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Особенности GroupDocs.Search"
    link: "/search/java/"
    link_title: "Узнать больше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) — это надежная библиотека для индексации и поиска текста в документах. Она поддерживает более 70 форматов файлов, включая PDFs, документы Word, электронные таблицы Excel, изображения и ZIP-файлы, обеспечивая быстрые и точные результаты поиска.

############################# Steps ############################
steps:
    enable: true
    title: "Как найти фразы в документах PPTX"
    content: |
      [GroupDocs.Search](/search/java/) упрощает поиск фраз в документах PPTX. Используйте различные опции для уточнения результатов поиска в приложениях Java.
      
      1. Создайте каталог индекса поиска.
      2. Укажите папку с файлами PPTX.
      3. Настройте параметры поиска.
      4. Получите и проанализируйте результаты поиска.
   
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
        // Определите путь к индексу поиска
        Index index = new Index("c:/MyIndex");

        // Укажите папку с документами
        index.add("c:/MyDocuments");

        // Установите параметры поиска
        SearchQuery word1 = SearchQuery.createWordQuery("lorem");
        SearchQuery word2 = SearchQuery.createWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.createWordQuery("dolor");

        SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, word2, word3);
        
        // Выполните поисковой запрос
        SearchResult result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Исследуйте поисковую систему документов Java"
  description: "GroupDocs.Search for Java позволяет выполнять поиск фраз более чем в 70 форматах файлов. Найдите и организуйте данные с помощью расширенных функций поиска."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Ключевые возможности GroupDocs.Search"
  features:
    # feature loop
    - title: "Поиск фраз"
      content: "Находите точные фразы в деловых документах, таких как PDFs, файлы Word, презентации и электронные таблицы. Используйте подстановочные знаки и другие опции, когда точная фраза неизвестна."

    # feature loop
    - title: "Оптимизированная индексация данных"
      content: "Ускорьте поиск документов, создавая и повторно используя индексы поиска. Индексация эффективно организует данные для более быстрых и точных поисков."

    # feature loop
    - title: "Поддержка нескольких языков"
      content: "Ищите документы на более чем 80 языках. Поддерживает различные раскладки клавиатуры и морфологический анализ для повышения точности поиска."

    # feature loop
    - title: "Расширенные параметры поиска"
      content: "Настройте поиск с учетом регистров, нечёткого поиска, соответствия однозвучных слов, фильтрации документов и других мощных функций."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Использование расширенных методов поиска"
      content: |
        Узнайте, как составить запросы для поиска в PPTX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Определите каталог для индекса поиска
          Index index = new Index("c:/MyIndex");
              
          // Установите путь к целевым документам
          index.add("c:/MyDocuments");

          // Создайте поисковой запрос для конкретной фразы
          SearchQuery word1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.createWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.createWordQuery("dolor");

          SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Получите результаты поиска
          SearchResult result = index.search(query);
          
          // Обработайте и используйте полученные результаты
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
            link: "/examples/search/formats/searchphrase.pptx"
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
    title: "Расширенные возможности поиска"
    exclude: "phrase"
    description: "Используйте современные функции поиска для повышения точности и производительности."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Поиск фраз в деловых документах"
    exclude: "PPTX"
    description: "GroupDocs.Search позволяет выполнять поиск фраз в более чем 70 форматах документов. Используйте расширенные опции и индексацию для эффективного поиска."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/phrase/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/phrase/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/phrase/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/phrase/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/phrase/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---