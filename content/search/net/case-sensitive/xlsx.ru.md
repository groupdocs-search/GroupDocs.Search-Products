
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:32
draft: false
lang: ru
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Поиск с учетом регистра в XLSX с использованием .NET"
head_description: "API GroupDocs.Search for .NET позволяет разработчикам C# выполнять поиск с учетом регистра в различных документах."

############################# Header ############################
title: "Поиск с учетом регистра" 
description: "GroupDocs.Search for .NET позволяет вам создавать сложные запросы на поиск с учетом регистра в ваших приложениях .NET."
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
       [GroupDocs.Search for .NET](/search/net/) — это мощная библиотека для текстового поиска и индексации в документах. Она поддерживает более 70 форматов файлов, включая PDF, Word, PowerPoint, Excel, изображения и ZIP-архивы, обеспечивая эффективную обработку больших объемов данных.

############################# Steps ############################
steps:
    enable: true
    title: "Как выполнить поиск с учетом регистра в документах XLSX"
    content: |
      [GroupDocs.Search](/search/net/) упрощает поиск с учетом регистра в документах XLSX. Используйте его для уточнения результатов в приложениях .NET.
      
      1. Определите папку для хранения индекса поиска.
      2. Выберите папку, содержащую файлы XLSX.
      3. Запустите поиск и получите результаты.
      4. Обработайте результаты.
   
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
        // Установите путь к папке индекса
        Index index = new Index("c:/MyIndex");

        // Укажите папку с документами для поиска
        index.Add("c:/MyDocuments");

        // Включите параметры поиска с учетом регистра
        SearchOptions options = new SearchOptions();
        options.UseCaseSensitiveSearch = true;

        // Запустите поиск
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Расширенные функции для поиска и индексации документов"
  description: "Библиотека GroupDocs.Search for .NET упрощает текстовый поиск и индексацию в более чем 70 форматах файлов. Эффективно находите и управляйте информацией с помощью мощных инструментов поиска."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Ключевые особенности GroupDocs.Search"
  features:
    # feature loop
    - title: "Расширенный текстовый поиск"
      content: "Ищите текст в различных форматах файлов, включая PDF, документы Word, таблицы и презентации. Используйте такие параметры, как точные совпадения, нечеткий поиск и подстановочные знаки для получения точных результатов."

    # feature loop
    - title: "Индексация больших объемов данных"
      content: "Создавайте и поддерживайте индексы для более быстрого поиска. Организованная индексация облегчает поиск в больших коллекциях документов."

    # feature loop
    - title: "Поддержка нескольких языков"
      content: "Ищите по документам на более чем 80 языках, с поддержкой различных раскладок клавиатуры и форм слов для более точных результатов."

    # feature loop
    - title: "Настраиваемые параметры поиска"
      content: "Настройте параметры поиска с учетом регистра, фильтры по диапазону дат и возможность исключать определенные слова или данные во время индексации."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Использование запросов поиска с учетом регистра"
      content: |
        Этот пример демонстрирует, как использовать запросы с учетом регистра для поиска в документах XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Установите папку для индекса поиска
          Index index = new Index("c:/MyIndex");
              
          // Укажите путь к документам, которые следует искать
          index.Add("c:/MyDocuments");

          // Создайте запрос на поиск
          SearchQuery wordQuery = SearchQuery.CreateWordQuery("Lorem");

          // Включите параметры поиска с учетом регистра
          SearchOptions options = new SearchOptions();
          options.UseCaseSensitiveSearch = true;

          // Ищите текст в документах
          SearchResult result = index.Search(wordQuery, options);
          
          // Обработайте результаты поиска
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
            link: "/examples/search/formats/searchcase-sensitive.xlsx"
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
    title: "Изучите ключевые функции"
    exclude: "case-sensitive"
    description: "Откройте для себя расширенные и эффективные функции поиска."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Поиск популярных форматов документов"
    exclude: "XLSX"
    description: "GroupDocs.Search поддерживает более 70 форматов файлов. Настраивайте правила поиска и используйте индексацию для экономии времени и усилий."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/case-sensitive/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/case-sensitive/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/case-sensitive/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/case-sensitive/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---