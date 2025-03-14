
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: ru
format: Docx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Поиск в документах формата DOCX с использованием .NET"
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
    title: "Как осуществить поиск в данных DOCX"
    content: |
      [GroupDocs.Search](/search/net/) позволяет эффективно проводить текстовые поиски в документах DOCX, что делает его идеальным для приложений .NET.
      
      1. Настройте папку для хранения поискового индекса.
      2. Выберите папку, содержащую ваши файлы.
      3. Настройте параметры поиска, чтобы обрабатывать только документы DOCX.
      4. Выполните поиск и получите результаты.
   
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
        // Путь для хранения многоразового поискового индекса
        Index index = new Index("c:/MyIndex");

        // Папка с документами
        index.Add("c:/MyDocuments");

        // Поиск только в определенных форматах файлов
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".docx");

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
          - title: "Скачать результат"
            icon: "download"
            link: "/examples/search/formats/searchfilters.docx"
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
    title: "Ключевые особенности"
    exclude: "filters"
    description: "Проводите точные и эффективные поиски данных."
    items: 
          
        # operation loop 1
        - name: "Поиск по условию"
          operation: "boolean"
          link: "/search/net/boolean/docx/"
          description: "Находите информацию в документах, используя булевы условия"

        # operation loop 2
        - name: "Чувствительный к регистру поиск"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/docx/"
          description: "Улучшите точность поиска, учитывая регистр"

        # operation loop 3
        - name: "Индексирование документов"
          operation: "document"
          link: "/search/net/document/docx/"
          description: "Индексируйте документы один раз и повторно используйте индекс для множества поисков"

        # operation loop 4
        - name: "Поисковые фильтры"
          operation: "filters"
          link: "/search/net/filters/docx/"
          description: "Используйте фильтры для уточнения обрабатываемых данных"

        # operation loop 5
        - name: "Точная фраза"
          operation: "phrase"
          link: "/search/net/phrase/docx/"
          description: "Ищите конкретное предложение или фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Найдите данные в ваших бизнес-документах"
    exclude: "DOCX"
    description: "GroupDocs.Search поддерживает более 70 форматов файлов, что позволяет эффективно обрабатывать и искать популярные офисные документы."
    items: 
        # format loop 1
        - name: "Поиск с фильтрами для DOCX"
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Поиск с фильтрами для PDF"
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: "Поиск с фильтрами для PPTX"
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: "Поиск с фильтрами для TXT"
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: "Поиск с фильтрами для XLSX"
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---