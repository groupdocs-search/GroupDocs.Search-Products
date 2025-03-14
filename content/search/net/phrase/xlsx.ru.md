
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: ru
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Поиск фраз в XLSX с использованием .NET"
head_description: "GroupDocs.Search for .NET расширяет возможности приложений C# мощными функциями поиска фраз в содержимом документов."

############################# Header ############################
title: "Поиск фраз в документах" 
description: "Быстро находите конкретные фразы с помощью GroupDocs.Search for .NET. Интегрируйте эффективный механизм поиска в ваши приложения .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачать"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Возможности GroupDocs.Search"
    link: "/search/net/"
    link_title: "Узнать больше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) — это мощная библиотека для индексирования и поиска текста в документах. Она поддерживает более 70 форматов файлов, включая PDF, документы Word, таблицы Excel, изображения и ZIP-файлы, обеспечивая быстрые и точные результаты поиска.

############################# Steps ############################
steps:
    enable: true
    title: "Как искать фразы в документах XLSX"
    content: |
      [GroupDocs.Search](/search/net/) упрощает поиск в документах XLSX. Используйте различные параметры для уточнения результатов поиска в приложениях .NET.
      
      1. Настройте папку для поискового индекса.
      2. Укажите папку, содержащую файлы XLSX.
      3. Настройте параметры поиска.
      4. Получайте и обрабатывайте результаты поиска.
   
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
        // Путь для хранения поискового индекса
        Index index = new Index("c:/MyIndex");

        // Папка, содержащая документы
        index.Add("c:/MyDocuments");

        // Настройте параметры поиска
        SearchQuery word1 = SearchQuery.CreateWordQuery("lorem");
        SearchQuery word2 = SearchQuery.CreateWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.CreateWordQuery("dolor");

        SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, word2, word3);

        // Выполните поиск
        SearchResult result = index.Search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Исследуйте поисковый движок документов .NET"
  description: "GroupDocs.Search for .NET позволяет осуществлять поиск фраз в более чем 70 форматах файлов. Удобно находите и управляйте данными с помощью продвинутых возможностей поиска."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Ключевые особенности GroupDocs.Search"
  features:
    # feature loop
    - title: "Поиск фраз"
      content: "Ищите точные фразы в деловых документах, включая PDF, файлы Word, презентации и таблицы. Используйте подстановочные знаки и другие параметры, если точная фраза неизвестна."

    # feature loop
    - title: "Эффективное индексирование данных"
      content: "Создавайте и повторно используйте поисковые индексы для ускорения поиска по документам. Индексирование структурирует данные эффективно, что делает поиск фраз быстрее."

    # feature loop
    - title: "Поддержка нескольких языков"
      content: "Ищите документы на более чем 80 языках. Поддерживает различные раскладки клавиатуры и морфологические формы слов для повышения точности поиска."

    # feature loop
    - title: "Гибкие параметры поиска"
      content: "Настраивайте поисковые запросы с помощью таких функций, как чувствительность к регистру, нечеткий поиск и поиск омофонов, фильтрация документов и многое другое."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Использование продвинутых техник поиска"
      content: |
        Узнайте, как создавать запросы для поиска в XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Укажите папку для поискового индекса
          Index index = new Index("c:/MyIndex");
              
          // Установите путь к документам для поиска
          index.Add("c:/MyDocuments");

          // Создайте запрос для конкретной фразы
          SearchQuery word1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.CreateWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.CreateWordQuery("dolor");

          SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, wildcard, word2);

          // Получите результаты поиска
          SearchResult result = index.Search(query);
          
          // Обработайте и используйте результаты
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
            link: "/examples/search/formats/searchphrase.xlsx"
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
    title: "Расширенные функции"
    exclude: "phrase"
    description: "Используйте мощные и эффективные возможности поиска."
    items: 
          
        # operation loop 1
        - name: "Поиск по условию"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "Находите информацию в документах, используя булевы условия"

        # operation loop 2
        - name: "Чувствительный к регистру поиск"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Улучшите точность поиска, учитывая регистр"

        # operation loop 3
        - name: "Индексирование документов"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "Индексируйте документы один раз и повторно используйте индекс для множества поисков"

        # operation loop 4
        - name: "Поисковые фильтры"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "Используйте фильтры для уточнения обрабатываемых данных"

        # operation loop 5
        - name: "Точная фраза"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "Ищите конкретное предложение или фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Поиск фраз в деловых документах"
    exclude: "XLSX"
    description: "GroupDocs.Search поддерживает поиск в более чем 70 форматах документов. Используйте продвинутые параметры и индексирование для оптимизации вашего процесса поиска."
    items: 
        # format loop 1
        - name: "Поиск фразы в DOCX"
          format: "DOCX"
          link: "/search/net/phrase/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Поиск фразы в PDF"
          format: "PDF"
          link: "/search/net/phrase/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: "Поиск фразы в PPTX"
          format: "PPTX"
          link: "/search/net/phrase/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: "Поиск фразы в TXT"
          format: "TXT"
          link: "/search/net/phrase/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: "Поиск фразы в XLSX"
          format: "XLSX"
          link: "/search/net/phrase/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---