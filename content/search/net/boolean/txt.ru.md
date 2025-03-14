
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:46
draft: false
lang: ru
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Поиск TXT в .NET с использованием логических операторов"
head_description: "API GroupDocs.Search for .NET позволяет разработчикам C# искать содержимое документов, используя логические операторы, такие как AND, OR и NOT."

############################# Header ############################
title: "Поиск текста с использованием логической логики" 
description: "GroupDocs.Search for .NET упрощает создание сложных поисковых запросов с использованием логических операторов (AND, OR, NOT) в ваших приложениях .NET."
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
       [GroupDocs.Search for .NET](/search/net/) — это обширная библиотека для поиска и индексирования текста в документах. Она поддерживает более 70 форматов файлов, таких как PDF, Word, PowerPoint, Excel, изображения и ZIP-файлы, что позволяет эффективно обрабатывать большие объемы информации.

############################# Steps ############################
steps:
    enable: true
    title: "Как искать содержимое документа TXT с использованием логической логики"
    content: |
      [GroupDocs.Search](/search/net/) упрощает поиск содержимого документа TXT. Она предоставляет условия поиска с логикой Boolean для уточнения результатов в приложениях .NET.
      
      1. Укажите папку для хранения индекса поиска.
      2. Выберите папку, содержащую файлы TXT.
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

        // Укажите папку, содержащую документы для поиска
        index.Add("c:/MyDocuments");

        // Запустите поиск с использованием сложного запроса
        SearchResult result = index.Search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Изучите расширенные функции для поиска и индексирования документов"
  description: "Библиотека GroupDocs.Search for .NET упрощает поиск текста и индексирование для более чем 70 форматов файлов. Находите и управляйте информацией с помощью расширенных поисковых инструментов."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Основные функции GroupDocs.Search"
  features:
    # feature loop
    - title: "Мощный поиск текста"
      content: "Ищите текст в различных типах файлов, включая PDF, документы Word, презентации PowerPoint и таблицы. Используйте такие функции, как точные совпадения, нечеткие поиски и подстановочные знаки для уточнения результатов."

    # feature loop
    - title: "Индексирование больших наборов данных"
      content: "Создавайте и поддерживайте индексы для более быстрого поиска. Индексирование структурирует и организует данные, что упрощает поиск в обширных коллекциях документов."

    # feature loop
    - title: "Поддержка нескольких языков"
      content: "Ищите документы на более чем 80 языках, с поддержкой различных раскладок клавиатуры и морфологических форм слов для повышения точности поиска."

    # feature loop
    - title: "Настраиваемые параметры поиска"
      content: "Настраивайте параметры поиска с помощью функций, таких как чувствительность к регистру, фильтры по диапазону дат и возможность исключать определенные слова или данные во время индексирования."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Использование расширенных логических поисковых запросов"
      content: |
        Этот пример демонстрирует, как применять логические запросы для поиска документов TXT.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Установите папку для индекса поиска
          Index index = new Index("c:/MyIndex");
              
          // Укажите путь к документам для поиска
          index.Add("c:/MyDocuments");

          // Создайте поисковый запрос с использованием логической логики
          SearchQuery wordQuery1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.CreateWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.CreateAndQuery(wordQuery1, wordQuery2);

          // Получите результаты поиска
          SearchResult result = index.Search(booleanQuery);
          
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
            link: "/examples/search/formats/searchboolean.txt"
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
    exclude: "boolean"
    description: "Изучайте расширенные и эффективные функции поиска."
    items: 
          
        # operation loop 1
        - name: "Поиск по условию"
          operation: "boolean"
          link: "/search/net/boolean/txt/"
          description: "Находите информацию в документах, используя булевы условия"

        # operation loop 2
        - name: "Чувствительный к регистру поиск"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/txt/"
          description: "Улучшите точность поиска, учитывая регистр"

        # operation loop 3
        - name: "Индексирование документов"
          operation: "document"
          link: "/search/net/document/txt/"
          description: "Индексируйте документы один раз и повторно используйте индекс для множества поисков"

        # operation loop 4
        - name: "Поисковые фильтры"
          operation: "filters"
          link: "/search/net/filters/txt/"
          description: "Используйте фильтры для уточнения обрабатываемых данных"

        # operation loop 5
        - name: "Точная фраза"
          operation: "phrase"
          link: "/search/net/phrase/txt/"
          description: "Ищите конкретное предложение или фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Поиск по популярным форматам документов"
    exclude: "TXT"
    description: "GroupDocs.Search поддерживает более 70 форматов файлов. Настраивайте правила поиска и используйте индексирование, чтобы сэкономить время и усилия."
    items: 
        # format loop 1
        - name: "Булевый поиск в DOCX"
          format: "DOCX"
          link: "/search/net/boolean/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Булевый поиск в PDF"
          format: "PDF"
          link: "/search/net/boolean/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: "Булевый поиск в PPTX"
          format: "PPTX"
          link: "/search/net/boolean/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: "Булевый поиск в TXT"
          format: "TXT"
          link: "/search/net/boolean/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: "Булевый поиск в XLSX"
          format: "XLSX"
          link: "/search/net/boolean/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---