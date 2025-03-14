
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:45
draft: false
lang: ru
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Булевый поиск в XLSX с Java"
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
    title: "Как выполнять булевые поиски в документах XLSX"
    content: |
      [GroupDocs.Search](/search/java/) позволяет выполнять текстовые поиски в документах XLSX. Поддержка булевых условий помогает повысить точность поиска в приложениях Java.
      
      1. Укажите папку для хранения индекса поиска.
      2. Выберите папку с документами XLSX.
      3. Выполните поисковой запрос и получите результаты.
      4. Обработайте полученные результаты.
   
    code:
      platform: "java"
      copy_title: "Копировать"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Результат поиска"
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
        Этот пример демонстрирует, как выполнять булевые поиски в файлах XLSX.
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
          - title: "Скачать результат"
            icon: "download"
            link: "/examples/search/formats/searchboolean.xlsx"
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
  description: "Попробуйте функции GroupDocs.Search бесплатно или запросите лицензию"
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
        - name: "Поиск по условию"
          operation: "boolean"
          link: "/search/java/boolean/xlsx/"
          description: "Находите информацию в документах, используя булевы условия"

        # operation loop 2
        - name: "Чувствительный к регистру поиск"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Улучшите точность поиска, учитывая регистр"

        # operation loop 3
        - name: "Индексирование документов"
          operation: "document"
          link: "/search/java/document/xlsx/"
          description: "Индексируйте документы один раз и повторно используйте индекс для множества поисков"

        # operation loop 4
        - name: "Поисковые фильтры"
          operation: "filters"
          link: "/search/java/filters/xlsx/"
          description: "Используйте фильтры для уточнения обрабатываемых данных"

        # operation loop 5
        - name: "Точная фраза"
          operation: "phrase"
          link: "/search/java/phrase/xlsx/"
          description: "Ищите конкретное предложение или фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Поиск популярных форматов документов"
    exclude: "XLSX"
    description: "GroupDocs.Search поддерживает более 70 форматов файлов, позволяя вам настраивать правила поиска и использовать индексацию для оптимизации производительности."
    items: 
        # format loop 1
        - name: "Булевый поиск в DOCX"
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Булевый поиск в PDF"
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: "Булевый поиск в PPTX"
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: "Булевый поиск в TXT"
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: "Булевый поиск в XLSX"
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---