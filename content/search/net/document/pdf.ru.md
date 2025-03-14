
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: ru
format: Pdf
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Поиск документов PDF в .NET с помощью GroupDocs.Search"
head_description: "Используйте GroupDocs.Search for .NET для эффективного текстового поиска в различных форматах документов с использованием C#."

############################# Header ############################
title: "Расширенный текстовый поиск в документах" 
description: "GroupDocs.Search for .NET упрощает текстовый поиск в популярных форматах документов, позволяя вам создавать мощные поисковые запросы в ваших приложениях .NET."
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
       [GroupDocs.Search for .NET](/search/net/) — это мощная библиотека, предназначенная для полнотекстового поиска и индексирования в документах. Она поддерживает более 70 форматов файлов, включая PDF, Word, PowerPoint, Excel, изображения и ZIP-архивы, обеспечивая быстрые и точные результаты поиска.

############################# Steps ############################
steps:
    enable: true
    title: "Как выполнить текстовый поиск в документах PDF"
    content: |
      [GroupDocs.Search](/search/net/) позволяет выполнять расширенные операции поиска содержимого в документах PDF, обеспечивая уточненные результаты поиска в приложениях .NET.
      
      1. Настройте папку для хранения индекса поиска.
      2. Выберите папку, содержащую файлы PDF.
      3. Настройте дополнительные параметры поиска.
      4. Запустите поиск и просмотрите результаты.
   
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
        // Определите путь к индексу поиска
        Index index = new Index("c:/MyIndex");

        // Выберите папку, содержащую документы для поиска
        index.Add("c:/MyDocuments");

        // Включите поиск гомофонов для нахождения слов, звучащих похоже
        SearchOptions options = new SearchOptions();
        options.UseHomophoneSearch = true;

        // Выполните сложный поисковый запрос
        SearchResult result = index.Search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Расширенные возможности поиска и индексирования"
  description: "GroupDocs.Search for .NET улучшает текстовый поиск и индексирование более чем в 70 форматах файлов, предоставляя эффективные инструменты для поиска и управления информацией."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Ключевые функции GroupDocs.Search"
  features:
    # feature loop
    - title: "Мощный текстовый поиск"
      content: "Ищите текст в различных типах документов, включая PDF, документы Word, презентации PowerPoint и таблицы. Используйте такие функции, как точные совпадения, нечеткий поиск и подстановочные знаки для уточнения ваших результатов."

    # feature loop
    - title: "Быстрое индексирование больших наборов данных"
      content: "Создавайте и управляйте индексами поиска для быстрого извлечения информации. Индексирование оптимизирует поисковые операции по обширным коллекциям документов."

    # feature loop
    - title: "Поддержка нескольких языков"
      content: "Выполняйте поиск на более чем 80 языках с поддержкой различных раскладок клавиатуры и вариантов слов для повышения точности."

    # feature loop
    - title: "Настраиваемые параметры поиска"
      content: "Настройте параметры поиска с опциями, такими как чувствительность к регистру, фильтры по диапазону дат и исключения слов для получения лучших результатов."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Выполнение сложных поисковых запросов"
      content: |
        Этот пример демонстрирует, как применять поисковые запросы для документов PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Определите папку для индекса поиска
          Index index = new Index("c:/MyIndex");
              
          // Укажите путь к документам
          index.Add("c:/MyDocuments");

          // Предоставьте пароль для защищенных документов
          index.Dictionaries.DocumentPasswords.Add("protected.pdf", "123456");

          // Включите нечеткий поиск для нахождения похожих слов
          SearchOptions options = new SearchOptions();
          options.FuzzySearch.Enabled = true;
          options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8);

          // Получите результаты поиска
          SearchResult result = index.Search("Loarem", options);
          
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
            link: "/examples/search/formats/searchdocument.pdf"
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
    exclude: "document"
    description: "Воспользуйтесь расширенными и высокопроизводительными функциями поиска."
    items: 
          
        # operation loop 1
        - name: "Поиск по условию"
          operation: "boolean"
          link: "/search/net/boolean/pdf/"
          description: "Находите информацию в документах, используя булевы условия"

        # operation loop 2
        - name: "Чувствительный к регистру поиск"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pdf/"
          description: "Улучшите точность поиска, учитывая регистр"

        # operation loop 3
        - name: "Индексирование документов"
          operation: "document"
          link: "/search/net/document/pdf/"
          description: "Индексируйте документы один раз и повторно используйте индекс для множества поисков"

        # operation loop 4
        - name: "Поисковые фильтры"
          operation: "filters"
          link: "/search/net/filters/pdf/"
          description: "Используйте фильтры для уточнения обрабатываемых данных"

        # operation loop 5
        - name: "Точная фраза"
          operation: "phrase"
          link: "/search/net/phrase/pdf/"
          description: "Ищите конкретное предложение или фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Поиск по вашим бизнес-документам"
    exclude: "PDF"
    description: "GroupDocs.Search поддерживает более 70 форматов файлов, включая офисные документы, что обеспечивает быструю и эффективную поисковую индексацию."
    items: 
        # format loop 1
        - name: "Поиск в документе DOCX"
          format: "DOCX"
          link: "/search/net/document/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Поиск в документе PDF"
          format: "PDF"
          link: "/search/net/document/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: "Поиск в документе PPTX"
          format: "PPTX"
          link: "/search/net/document/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: "Поиск в документе TXT"
          format: "TXT"
          link: "/search/net/document/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: "Поиск в документе XLSX"
          format: "XLSX"
          link: "/search/net/document/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---