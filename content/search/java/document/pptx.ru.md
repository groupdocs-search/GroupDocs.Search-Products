
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:34
draft: false
lang: ru
format: Pptx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Найдите текст в документах PPTX с помощью GroupDocs.Search для Java"
head_description: "GroupDocs.Search for Java помогает разработчикам Java быстро искать текст в различных форматах документов."

############################# Header ############################
title: "Умный поиск текста в документах" 
description: "С помощью GroupDocs.Search for Java вы можете без проблем искать и извлекать текст из различных типов документов в ваших приложениях Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Получить бесплатную пробную версию"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Что делает GroupDocs.Search?"
    link: "/search/java/"
    link_title: "Узнать больше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) — это мощная библиотека для поиска и индексирования документов, которая поддерживает более 70 форматов файлов, включая PDF, Word, PowerPoint, Excel, изображения и ZIP-архивы. Она обеспечивает быстрые, точные и масштабируемые возможности поиска для больших коллекций документов.

############################# Steps ############################
steps:
    enable: true
    title: "Выполнение текстовых поисков в файлах PPTX"
    content: |
      [GroupDocs.Search](/search/java/) облегчает поиск по файлам PPTX, используя сложную логику и индексирование, что улучшает точность поиска в приложениях Java.
      
      1. Настройте каталог для хранения индекса поиска.
      2. Выберите папку, содержащую файлы PPTX.
      3. Определите дополнительные параметры поиска.
      4. Выполните поиск и проанализируйте результаты.
   
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
        // Установите каталог для хранения индекса поиска
        Index index = new Index("c:/MyIndex");

        // Укажите папку, содержащую документы для поиска
        index.add("c:/MyDocuments");

        // Включите поиск по схожим звучанием словам
        SearchOptions options = new SearchOptions();
        options.setUseHomophoneSearch(true);

        // Выполните сложный поисковый запрос
        SearchResult result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Расширенные возможности поиска и индексирования"
  description: "GroupDocs.Search for Java упрощает поиск текста и индексирование в более чем 70 форматах документов, предоставляя эффективные инструменты для быстрой обработки и извлечения информации."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Основные функции GroupDocs.Search"
  features:
    # feature loop
    - title: "Всеобъемлющий текстовый поиск"
      content: "Ищите текст в различных форматах документов, таких как PDF, документы Word, презентации PowerPoint и таблицы. Используйте точные совпадения, нечеткий поиск и подстановочные знаки для уточнения результатов поиска."

    # feature loop
    - title: "Оптимизированное индексирование для больших данных"
      content: "Создайте структурированные индексы для ускорения поиска, что облегчает навигацию по обширным репозиториям документов."

    # feature loop
    - title: "Поддержка нескольких языков"
      content: "Проводите поиски на 80+ языках с помощью встроенной поддержки различных раскладок клавиатуры и вариантов морфологии слов, что повышает точность."

    # feature loop
    - title: "Гибкие параметры поиска"
      content: "Настройте поиск с помощью таких опций, как чувствительность к регистру, фильтрация по дате и возможность исключения определенных слов для получения точных результатов."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Реализация сложных поисковых запросов"
      content: |
        Этот пример иллюстрирует, как эффективно использовать поисковые запросы для поиска в документах PPTX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Укажите каталог для индексирования поиска
          Index index = new Index("c:/MyIndex");
              
          // Предоставьте путь к файлам документов
          index.add("c:/MyDocuments");

          // Введите пароль для зашифрованных документов
          index.getDictionaries().getDocumentPasswords().add("protected.pptx", "123456");

          // Активируйте нечеткий поиск для обнаружения схожих слов
          SearchOptions options = new SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8));

          // Получите результаты поиска
          SearchResult result = index.Search("Loarem", options);
          
          // Обработайте и проанализируйте результаты поиска
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
            link: "/examples/search/formats/searchdocument.pptx"
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
    title: "Обзор ключевых функций"
    exclude: "document"
    description: "Откройте для себя высокопроизводительные функции текстового поиска, разработанные для эффективности и точности."
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
    title: "Найдите информацию в документах PPTX с помощью GroupDocs.Search"
    exclude: "PPTX"
    description: "GroupDocs.Search поддерживает более 70 форматов, включая офисные файлы, что обеспечивает быстрый поиск с расширенными функциями индексирования."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/document/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/document/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/document/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/document/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/document/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---