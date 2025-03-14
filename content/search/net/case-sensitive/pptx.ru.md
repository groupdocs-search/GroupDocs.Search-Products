
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: ru
format: Pptx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Поиск с учетом регистра в PPTX с использованием .NET"
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
    title: "Как выполнить поиск с учетом регистра в документах PPTX"
    content: |
      [GroupDocs.Search](/search/net/) упрощает поиск с учетом регистра в документах PPTX. Используйте его для уточнения результатов в приложениях .NET.
      
      1. Определите папку для хранения индекса поиска.
      2. Выберите папку, содержащую файлы PPTX.
      3. Запустите поиск и получите результаты.
      4. Обработайте результаты.
   
    code:
      platform: "net"
      copy_title: "Копировать"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Результат поиска"
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
        Этот пример демонстрирует, как использовать запросы с учетом регистра для поиска в документах PPTX.
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
          - title: "Скачать результат"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.pptx"
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
  description: "Попробуйте функции GroupDocs.Search бесплатно или запросите лицензию"
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
        - name: "Поиск по условию"
          operation: "boolean"
          link: "/search/net/boolean/pptx/"
          description: "Находите информацию в документах, используя булевы условия"

        # operation loop 2
        - name: "Чувствительный к регистру поиск"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pptx/"
          description: "Улучшите точность поиска, учитывая регистр"

        # operation loop 3
        - name: "Индексирование документов"
          operation: "document"
          link: "/search/net/document/pptx/"
          description: "Индексируйте документы один раз и повторно используйте индекс для множества поисков"

        # operation loop 4
        - name: "Поисковые фильтры"
          operation: "filters"
          link: "/search/net/filters/pptx/"
          description: "Используйте фильтры для уточнения обрабатываемых данных"

        # operation loop 5
        - name: "Точная фраза"
          operation: "phrase"
          link: "/search/net/phrase/pptx/"
          description: "Ищите конкретное предложение или фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Поиск популярных форматов документов"
    exclude: "PPTX"
    description: "GroupDocs.Search поддерживает более 70 форматов файлов. Настраивайте правила поиска и используйте индексацию для экономии времени и усилий."
    items: 
        # format loop 1
        - name: "Чувствительный к регистру поиск в DOCX"
          format: "DOCX"
          link: "/search/net/case-sensitive/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Чувствительный к регистру поиск в PDF"
          format: "PDF"
          link: "/search/net/case-sensitive/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: "Чувствительный к регистру поиск в PPTX"
          format: "PPTX"
          link: "/search/net/case-sensitive/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: "Чувствительный к регистру поиск в TXT"
          format: "TXT"
          link: "/search/net/case-sensitive/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: "Чувствительный к регистру поиск в XLSX"
          format: "XLSX"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---