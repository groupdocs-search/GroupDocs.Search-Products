
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:50
draft: false
lang: ru
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Найдите текст в PPTX с помощью GroupDocs.Search в Node.js"
head_description: "Используйте GroupDocs.Search for Node.js via Java с JavaScript для эффективного поиска текста в различных форматах документов."

############################# Header ############################
title: "Умное решение для поиска документов" 
description: "Находите текст в различных форматах документов с помощью GroupDocs.Search for Node.js via Java. Создавайте расширенные поисковые запросы в ваших приложениях Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Попробуйте бесплатно"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Введение в GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "Узнать больше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) — это высокопроизводительная библиотека для полного текстового поиска и индексации документов. Она поддерживает более 70 типов файлов, включая PDF, Word, PowerPoint, Excel, изображения и ZIP-архивы, обеспечивая быстрые и точные результаты.

############################# Steps ############################
steps:
    enable: true
    title: "Выполните поиск в файлах PPTX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) позволяет вам выполнять поиски в файлах PPTX, уточняя результаты в приложениях Node.js via Java.
      
      1. Определите папку хранения для поискового индекса.
      2. Выберите папку с файлами PPTX.
      3. Установите дополнительные параметры поиска.
      4. Запустите поиск и проанализируйте результаты.
   
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

        // Укажите директорию для хранения поискового индекса
        const index = new searchLib.Index("c:/MyIndex");

        // Выберите папку, содержащую документы для поиска
        index.add("c:/MyDocuments");

        // Включите поиск по однозвучным словам
        const options = new searchLib.SearchOptions();
        options.setUseHomophoneSearch(true);

        // Запустите сложный поисковый запрос
        const result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Расширенные возможности поиска и индексации"
  description: "GroupDocs.Search for Node.js via Java предоставляет мощные инструменты для текстового поиска и индексации по более чем 70 форматам документов, упрощая нахождение и организацию информации."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Ключевые преимущества GroupDocs.Search"
  features:
    # feature loop
    - title: "Всеобъемлющий текстовый поиск"
      content: "Находите текст в различных типах документов, включая PDF, документами Word, презентациями PowerPoint и электронными таблицами. Используйте точные совпадения, нечеткие поиски и подстановочные знаки для уточненных результатов."

    # feature loop
    - title: "Эффективная индексация для больших данных"
      content: "Ускорьте поиски, создавая структурированные индексы, что облегчает извлечение информации из больших коллекций документов."

    # feature loop
    - title: "Поддерживает более 80 языков"
      content: "Ищите в документах на различных языках с автоматическим распознаванием различных форм слов и раскладок клавиатуры."

    # feature loop
    - title: "Настраиваемые параметры поиска"
      content: "Регулируйте параметры поиска, такие как чувствительность к регистру, фильтры по дате и исключения слов, чтобы получить точные результаты."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Использование поиска для документов PPTX"
      content: |
        В этом примере показано, как использовать поисковые запросы в документах PPTX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Установите директорию для индексирования поиска
          const index = new searchLib.Index("c:/MyIndex");
              
          // Укажите путь к файлу для хранения документа
          index.add("c:/MyDocuments");

          // Введите пароль для защищенных файлов
          index.getDictionaries().getDocumentPasswords().add("protected.pptx", '123456');

          // Включите нечеткий поиск для обнаружения схожих слов
          const options = new searchLib.SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new searchLib.SimilarityLevel(0.8));

          // Извлеките результаты поиска
          const result = index.search("Loarem", options);
          
          // Обработайте и просмотрите результаты
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
            link: "/examples/search/formats/searchdocument.pptx"
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
    title: "Изучите ключевые возможности"
    exclude: "document"
    description: "Откройте для себя функции высокоскоростного поиска, разработанные для повышения эффективности и точности."
    items: 
          
        # operation loop 1
        - name: "Поиск по условию"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "Находите информацию в документах, используя булевы условия"

        # operation loop 2
        - name: "Чувствительный к регистру поиск"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "Улучшите точность поиска, учитывая регистр"

        # operation loop 3
        - name: "Индексирование документов"
          operation: "document"
          link: "/search/nodejs-java/document/pptx/"
          description: "Индексируйте документы один раз и повторно используйте индекс для множества поисков"

        # operation loop 4
        - name: "Поисковые фильтры"
          operation: "filters"
          link: "/search/nodejs-java/filters/pptx/"
          description: "Используйте фильтры для уточнения обрабатываемых данных"

        # operation loop 5
        - name: "Точная фраза"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "Ищите конкретное предложение или фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Поиск в различных документах"
    exclude: "PPTX"
    description: "GroupDocs.Search работает более чем с 70 форматами файлов, включая офисные документы, обеспечивая быстрые и точные поисковые запросы с поддержкой индексации."
    items: 
        # format loop 1
        - name: "Поиск в документе DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/document/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Поиск в документе PDF"
          format: "PDF"
          link: "/search/nodejs-java/document/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: "Поиск в документе PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/document/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: "Поиск в документе TXT"
          format: "TXT"
          link: "/search/nodejs-java/document/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: "Поиск в документе XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---