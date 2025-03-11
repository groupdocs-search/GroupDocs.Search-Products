
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:37
draft: false
lang: ru
format: Pptx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Поиск в документах формата PPTX с использованием .NET"
head_description: "GroupDocs.Search for .NET улучшает приложения C# с помощью эффективного текстового поиска по различным форматам бизнес-документов."

############################# Header ############################
title: "Поиск текста в бизнес-документах" 
description: "GroupDocs.Search for .NET позволяет проводить мощные и гибкие текстовые поиски в ваших документах. Интегрируйте функциональность поиска в приложения .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачать бесплатно"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Что такое GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Узнать больше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) — это мощная библиотека для эффективного текстового поиска и индексации документов. Она поддерживает более 70 форматов файлов, включая стандартные документы, такие как PDF, Word, Excel и PowerPoint. Улучшите скорость поиска с помощью быстрых и точных результатов.

############################# Steps ############################
steps:
    enable: true
    title: "Как осуществить поиск в данных PPTX"
    content: |
      [GroupDocs.Search](/search/net/) позволяет эффективно проводить текстовые поиски в документах PPTX, что делает его идеальным для приложений .NET.
      
      1. Настройте папку для хранения поискового индекса.
      2. Выберите папку, содержащую ваши файлы.
      3. Настройте параметры поиска, чтобы обрабатывать только документы PPTX.
      4. Выполните поиск и получите результаты.
   
    code:
      platform: "net"
      copy_title: "Копировать"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "нажмите, чтобы скопировать"
        copy_done: "скопировано"
      links:
        #  loop
        - title: "Больше примеров"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "Документация"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // Путь для хранения многоразового поискового индекса
        Index index = new Index("c:/MyIndex");

        // Папка с документами
        index.Add("c:/MyDocuments");

        // Поиск только в определенных форматах файлов
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".pptx");

        // Получение результатов поиска
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Расширенные функции поиска"
  description: "GroupDocs.Search for .NET обеспечивает сложные текстовые поисковые операции по более чем 70 форматам файлов. Индексация повышает эффективность поиска и помогает эффективно управлять содержимым документов."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Основные функции GroupDocs.Search"
  features:
    # feature loop
    - title: "Расширенный текстовый поиск"
      content: "Извлекайте актуальный текст из популярных бизнес-документов, включая PDFs, Word-файлы, презентации и таблицы. Поддерживает несколько методов поиска, таких как неформальный поиск, поиск однозвучных слов и подстановочные знаки."

    # feature loop
    - title: "Оптимизированная индексация для более быстрого поиска"
      content: "Создавайте и повторно используйте поисковые индексы для повышения скорости поиска. Индексация оптимизирует производительность при поиске в больших коллекциях документов."

    # feature loop
    - title: "Поддержка нескольких языков"
      content: "Выполняйте поиски в документах, написанных более чем на 80 языках. Определяет различные раскладки клавиатуры и варианты слов для повышения точности."

    # feature loop
    - title: "Гибкие настройки поиска"
      content: "Уточняйте результаты поиска с помощью настраиваемых опций, включая фильтры, регулярные выражения и параметры чувствительности к регистру."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Фильтр документов для обработки"
      content: |
        Узнайте, как сузить поиск документов с помощью фильтров.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Настройте индекс, исключающий определенные форматы файлов.
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.CreateFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter);
          settings.DocumentFilter = invertedFilter;

          Index index = new Index("c:/MyIndex", settings);
              
          // Укажите директорию документа.
          index.Add("c:/MyDocuments");

          // Получите результаты поиска.
          SearchResult result = index.Search("Lorem");
          
          // Обработайте и используйте результаты поиска.
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "Копировать"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "нажмите, чтобы скопировать"
          copy_done: "скопировано"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchfilters.pptx"
        links:
          #  loop
          - title: "Больше примеров"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "Документация"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Готовы начать?"
  description: "Попробуйте возможности GroupDocs.Search бесплатно или запросите лицензию"
  items:
    #  loop
    - title: "Скачивание Nuget"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "Лицензирование"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Ключевые особенности"
    exclude: "filters"
    description: "Проводите точные и эффективные поиски данных."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Найдите данные в ваших бизнес-документах"
    exclude: "PPTX"
    description: "GroupDocs.Search поддерживает более 70 форматов файлов, что позволяет эффективно обрабатывать и искать популярные офисные документы."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---