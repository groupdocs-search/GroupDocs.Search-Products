
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:48
draft: false
lang: ru
format: Docx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Выполнение поиска с учетом регистра в DOCX с помощью Node.js"
head_description: "API GroupDocs.Search for Node.js via Java позволяет разработчикам на JavaScript выполнять поиск с учетом регистра в различных типах документов."

############################# Header ############################
title: "Поиск с учетом регистра" 
description: "GroupDocs.Search for Node.js via Java позволяет вам реализовать расширенные функции поиска с учетом регистра в ваших приложениях на Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачать бесплатно"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Что такое GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Узнать больше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) — это мощная библиотека для поиска и индексации текста в документах. Она поддерживает более 70 форматов, включая PDF, Word, Excel, PowerPoint, изображения и ZIP-файлы, что позволяет эффективно обрабатывать большие объемы данных.

############################# Steps ############################
steps:
    enable: true
    title: "Шаги для выполнения поиска с учетом регистра в файлах DOCX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) упрощает выполнение поиска с учетом регистра в файлах DOCX, улучшая ваши рабочие процессы Node.js via Java.
      
      1. Настройте папку для хранения индекса поиска.
      2. Выберите папку, содержащую файлы DOCX.
      3. Запустите поиск и получите результаты.
      4. Обработайте и используйте результаты.
   
    code:
      platform: "nodejs-java"
      copy_title: "Копировать"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Результат поиска"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "нажмите, чтобы скопировать"
        copy_done: "скопировано"
      links:
        #  loop
        - title: "Больше примеров"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "Документация"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // Укажите путь к папке индекса
        const index = new searchLib.Index("c:/MyIndex");

        // Установите папку, содержащую документы для поиска
        index.add("c:/MyDocuments");

        // Включите поиск с учетом регистра в настройках
        const options = new groupdocs.search.SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Выполните поиск
        const result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Ключевые функции для поиска и индексации документов"
  description: "С помощью GroupDocs.Search for Node.js via Java вы можете искать и индексировать текст в более чем 70 форматах файлов. Доступайтесь и организуйте информацию без усилий с использованием продвинутых инструментов поиска."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Основные функции GroupDocs.Search"
  features:
    # feature loop
    - title: "Всеобъемлющий текстовый поиск"
      content: "Находите текст в различных типах документов, таких как PDF, файлы Word, таблицы и презентации. Используйте такие параметры, как точные совпадения, нечеткий поиск и подстановочные знаки для получения точных результатов."

    # feature loop
    - title: "Эффективная индексация данных"
      content: "Создавайте и управляйте индексами для ускорения поиска. Индексация помогает организовать и быстро находить данные в крупных коллекциях документов."

    # feature loop
    - title: "Поддержка нескольких языков"
      content: "Ищите документы на более чем 80 языках с поддержкой различных раскладок клавиатуры и вариантов написания слов, обеспечивая точные результаты поиска."

    # feature loop
    - title: "Настраиваемые параметры поиска"
      content: "Регулируйте параметры поиска, включая учет регистра, фильтры по датам и исключение определенных терминов или данных при индексации."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Пример: Реализация поиска с учетом регистра"
      content: |
        Этот пример демонстрирует, как выполнять поиск с учетом регистра для документов DOCX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Определите папку для индекса поиска
          const index = new searchLib.Index("c:/MyIndex");
              
          // Укажите путь к папке документов
          index.add("c:/MyDocuments");

          // Настройте запрос поиска
          const wordQuery = searchLib.SearchQuery.createWordQuery("Lorem");

          // Активируйте параметры поиска с учетом регистра
          const options = new groupdocs.search.SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Ищите текст в документах
          const result = index.search(wordQuery, options);
          
          // Обработайте и управляйте результатами
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "Копировать"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "нажмите, чтобы скопировать"
          copy_done: "скопировано"
        top_links:
          #  loop
          - title: "Скачать результат"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.docx"
        links:
          #  loop
          - title: "Больше примеров"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "Документация"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Search бесплатно или запросите лицензию"
  items:
    #  loop
    - title: "Скачивание NPM"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "Лицензирование"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Ключевые функциональные возможности"
    exclude: "case-sensitive"
    description: "Изучите расширенные функции для быстрого и точного поиска документов."
    items: 
          
        # operation loop 1
        - name: "Поиск по условию"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/docx/"
          description: "Находите информацию в документах, используя булевы условия"

        # operation loop 2
        - name: "Чувствительный к регистру поиск"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "Улучшите точность поиска, учитывая регистр"

        # operation loop 3
        - name: "Индексирование документов"
          operation: "document"
          link: "/search/nodejs-java/document/docx/"
          description: "Индексируйте документы один раз и повторно используйте индекс для множества поисков"

        # operation loop 4
        - name: "Поисковые фильтры"
          operation: "filters"
          link: "/search/nodejs-java/filters/docx/"
          description: "Используйте фильтры для уточнения обрабатываемых данных"

        # operation loop 5
        - name: "Точная фраза"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/docx/"
          description: "Ищите конкретное предложение или фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Совместимые форматы документов"
    exclude: "DOCX"
    description: "GroupDocs.Search поддерживает более 70 форматов документов. Настройте параметры поиска и сэкономьте время на индексацию."
    items: 
        # format loop 1
        - name: "Чувствительный к регистру поиск в DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Чувствительный к регистру поиск в PDF"
          format: "PDF"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: "Чувствительный к регистру поиск в PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: "Чувствительный к регистру поиск в TXT"
          format: "TXT"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: "Чувствительный к регистру поиск в XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---