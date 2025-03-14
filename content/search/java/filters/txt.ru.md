
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: ru
format: Txt
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Поиск в документах TXT с использованием Java"
head_description: "GroupDocs.Search for Java добавляет мощный текстовый поиск в приложениях на Java, поддерживая различные форматы бизнес-документов."

############################# Header ############################
title: "Находите текст в бизнес-документах" 
description: "GroupDocs.Search for Java позволяет осуществлять поиск текста в документах с помощью гибких и точных запросов. Интегрируйте функцию поиска в приложения на Java."
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
    title: "Что такое GroupDocs.Search?"
    link: "/search/java/"
    link_title: "Узнать больше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) — это мощная библиотека для быстрого текстового поиска и индексирования документов. Она поддерживает более 70 форматов файлов, включая стандартные форматы, такие как PDF, Word, Excel и PowerPoint. Улучшите свои приложения с помощью высокоскоростных и точных возможностей поиска.

############################# Steps ############################
steps:
    enable: true
    title: "Как осуществлять поиск в документах TXT"
    content: |
      [GroupDocs.Search](/search/java/) позволяет быстро и эффективно искать текст в документах TXT, идеально подходит для приложений Java.
      
      1. Укажите папку для хранения индекса поиска.
      2. Выберите папку, содержащую ваши документы.
      3. Настройте параметры поиска, чтобы ограничить результаты документами TXT.
      4. Запустите поиск и получите результаты.
   
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
        // Каталог для хранения повторно используемого индекса поиска
        Index index = new Index("c:/MyIndex");

        // Папка, содержащая документы
        index.add("c:/MyDocuments");

        // Фильтровать поиск по формату документа
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.createFileExtension(".txt");

        // Получить результаты поиска
        SearchResult result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Расширенные возможности поиска"
  description: "GroupDocs.Search for Java предоставляет возможности продвинутого текстового поиска по более чем 70 форматам файлов. Индексирование ускоряет поиск и повышает эффективность управления документами."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Ключевые функции GroupDocs.Search"
  features:
    # feature loop
    - title: "Мощный текстовый поиск"
      content: "Находите текст в популярных форматах документов, таких как PDF, файлы Word, презентации и таблицы. Поддерживаются различные методы поиска, включая нечеткий поиск, одногласные слова и подстановочные знаки."

    # feature loop
    - title: "Оптимизированное индексирование для лучшей производительности"
      content: "Создавайте и повторно используйте поисковые индексы для повышения скорости и эффективности поиска, особенно в больших коллекциях документов."

    # feature loop
    - title: "Поддержка многиязычного поиска"
      content: "Ищите внутри документов, написанных более чем на 80 языках. Определение различных раскладок клавиатуры и вариаций слов для повышения точности."

    # feature loop
    - title: "Настраиваемые параметры поиска"
      content: "Уточняйте результаты поиска с помощью фильтров, регулярных выражений и других расширенных настроек поиска."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Фильтрация документов перед поиском"
      content: |
        Узнайте, как уточнить поиски с помощью фильтров
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Настройте индекс, исключающий определенные форматы файлов
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new Index("c:/MyIndex", settings);
              
          // Укажите путь для хранения документов
          index.add("c:/MyDocuments");

          // Получите результаты поиска
          SearchResult result = index.search("Lorem", options);
          
          // Обработайте и используйте результаты поиска
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
            link: "/examples/search/formats/searchfilters.txt"
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
    title: "Ключевые функции"
    exclude: "filters"
    description: "Осуществляйте точные и эффективные текстовые поиски."
    items: 
          
        # operation loop 1
        - name: "Поиск по условию"
          operation: "boolean"
          link: "/search/java/boolean/txt/"
          description: "Находите информацию в документах, используя булевы условия"

        # operation loop 2
        - name: "Чувствительный к регистру поиск"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/txt/"
          description: "Улучшите точность поиска, учитывая регистр"

        # operation loop 3
        - name: "Индексирование документов"
          operation: "document"
          link: "/search/java/document/txt/"
          description: "Индексируйте документы один раз и повторно используйте индекс для множества поисков"

        # operation loop 4
        - name: "Поисковые фильтры"
          operation: "filters"
          link: "/search/java/filters/txt/"
          description: "Используйте фильтры для уточнения обрабатываемых данных"

        # operation loop 5
        - name: "Точная фраза"
          operation: "phrase"
          link: "/search/java/phrase/txt/"
          description: "Ищите конкретное предложение или фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Поиск в бизнес-документах"
    exclude: "TXT"
    description: "GroupDocs.Search поддерживает более 70 форматов файлов, что упрощает поиск по широко используемым офисным документам."
    items: 
        # format loop 1
        - name: "Поиск с фильтрами для DOCX"
          format: "DOCX"
          link: "/search/java/filters/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Поиск с фильтрами для PDF"
          format: "PDF"
          link: "/search/java/filters/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: "Поиск с фильтрами для PPTX"
          format: "PPTX"
          link: "/search/java/filters/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: "Поиск с фильтрами для TXT"
          format: "TXT"
          link: "/search/java/filters/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: "Поиск с фильтрами для XLSX"
          format: "XLSX"
          link: "/search/java/filters/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---