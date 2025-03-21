
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: ru
format: Docx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Поиск в документах DOCX с использованием Node.js"
head_description: "GroupDocs.Search for Node.js via Java добавляет быстрые и точные возможности текстового поиска в приложения JavaScript, поддерживая множество форматов документов."

############################# Header ############################
title: "Найдите текст в бизнес-документах" 
description: "GroupDocs.Search for Node.js via Java предоставляет мощную и гибкую функциональность поиска для документов. Интегрируйте текстовый поиск в приложения Node.js."
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
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) — это мощная библиотека для поиска и индексирования, которая обеспечивает быстрый поиск текста в документах. Она поддерживает более 70 форматов файлов, включая PDF, Word, Excel и PowerPoint, обеспечивая точные и эффективные результаты поиска.

############################# Steps ############################
steps:
    enable: true
    title: "Как выполнить поиск в документах DOCX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) упрощает поиск текста в DOCX документах для приложений Node.js via Java.
      
      1. Создайте каталог для хранения индекса поиска.
      2. Выберите папку, содержащую документы.
      3. Настройте параметры поиска, чтобы включить только файлы DOCX.
      4. Запустите поиск и получите результаты.
   
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

        // Определите каталог для хранения индекса поиска
        const index = new searchLib.Index("c:/MyIndex");

        // Укажите папку, содержащую документы для поиска
        index.add("c:/MyDocuments");

        // Ограничьте поиск конкретными форматами файлов
        const options = new searchLib.SearchOptions();
        options.SearchDocumentFilter = 
            searchLib.SearchDocumentFilter.createFileExtension(".docx");

        // Получите и обработайте результаты поиска
        const result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Усовершенствованные возможности поиска"
  description: "GroupDocs.Search for Node.js via Java повышает эффективность поиска документов, индексируя более 70 форматов файлов. Оптимизируйте извлечение содержимого с помощью усовершенствованных поисковых технологий."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Ключевые особенности GroupDocs.Search"
  features:
    # feature loop
    - title: "Всеобъемлющий текстовый поиск"
      content: "Извлекайте и находите текст в популярных форматах документов, таких как PDF, файлы Word, электронные таблицы и презентации. Поддерживает нечеткий поиск, омографы и подстановочные запросы."

    # feature loop
    - title: "Оптимизированное индексирование для повышения производительности"
      content: "Ускоряйте поиски с помощью создания повторно используемых индексов. Увеличивает скорость и эффективность при работе с большими коллекциями документов."

    # feature loop
    - title: "Многоязычная поддержка"
      content: "Ищите документы на более чем 80 языках. Признает раскладки клавиатуры и вариации слов для повышения точности."

    # feature loop
    - title: "Настраиваемые параметры поиска"
      content: "Тонко настраивайте результаты поиска с помощью фильтров, регулярных выражений, учета регистра и других гибких параметров."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Фильтрация документов для поиска"
      content: |
        Узнайте, как уточнить поисковые запросы с помощью фильтров.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Настройте индекс для исключения ненужных форматов файлов
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            searchLib.DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = 
            searchLib.DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new searchLib.Index("c:/MyIndex", settings);
              
          // Укажите каталог, содержащий документы
          index.add("c:/MyDocuments");

          // Обработайте результаты поиска для дальнейшего использования
          const result = index.Search("Lorem", options);
          
          // Обработайте результаты поиска для дальнейшего использования
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
            link: "/examples/search/formats/searchfilters.docx"
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
    title: "Ключевые функции"
    exclude: "filters"
    description: "Проводите быстрые и точные текстовые поиски по документам."
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
    title: "Поиск в различных форматах документов"
    exclude: "DOCX"
    description: "GroupDocs.Search поддерживает более 70 типов файлов, позволяя эффективно искать текст в различных офисных и бизнес-документах."
    items: 
        # format loop 1
        - name: "Поиск с фильтрами для DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/filters/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Поиск с фильтрами для PDF"
          format: "PDF"
          link: "/search/nodejs-java/filters/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: "Поиск с фильтрами для PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/filters/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: "Поиск с фильтрами для TXT"
          format: "TXT"
          link: "/search/nodejs-java/filters/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: "Поиск с фильтрами для XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---