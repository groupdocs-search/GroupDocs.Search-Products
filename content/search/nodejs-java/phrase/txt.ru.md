
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: ru
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Поиск фраз в TXT с использованием Node.js"
head_description: "GroupDocs.Search for Node.js via Java добавляет мощную функциональность поиска фраз в приложения JavaScript для эффективного поиска документов."

############################# Header ############################
title: "Найдите фразы в документах" 
description: "Быстро находите конкретные фразы с помощью GroupDocs.Search for Node.js via Java. Интегрируйте быстрые и точные функции поиска в ваши приложения Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачать"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Функции GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "Узнать больше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) - это высокопроизводительная библиотека для индексирования и поиска текста в документах. Она поддерживает более 70 форматов файлов, включая PDF, Word документы, Excel таблицы, изображения и ZIP архивы, обеспечивая точные и быстрые результаты поиска.

############################# Steps ############################
steps:
    enable: true
    title: "Как найти фразы в TXT документах"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) упрощает поиск фраз в TXT документах. Применяйте различные параметры поиска, чтобы уточнить результаты в приложениях Node.js via Java.
      
      1. Настройте папку для поискового индекса.
      2. Определите папку, содержащую файлы TXT.
      3. Настройте параметры поиска.
      4. Получите и обработайте результаты поиска.
   
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

        // Укажите путь для хранения поискового индекса
        const index = new searchLib.Index("c:/MyIndex");

        // Установите папку, содержащую документы
        index.add("c:/MyDocuments");

        // Настройте параметры поиска
        const word1 = searchLib.SearchQuery.createWordQuery("lorem");
        const word2 = searchLib.SearchQuery.createWordQuery("ipsum");
        const word3 = searchLib.SearchQuery.createWordQuery("dolor");

        const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, word2, word3);

        // Выполните запрос поиска
        const result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Откройте для себя поисковую систему документов Node.js"
  description: "GroupDocs.Search for Node.js via Java позволяет выполнять поиск фраз более чем в 70 форматах файлов, что упрощает организацию данных с помощью расширенных функций поиска."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Ключевые возможности GroupDocs.Search"
  features:
    # feature loop
    - title: "Поиск фраз"
      content: "Находите точные фразы в деловых документах, таких как PDF, Word файлы, презентации и таблицы. Используйте подстановочные знаки и гибкие параметры поиска, когда полная фраза неизвестна."

    # feature loop
    - title: "Оптимизированное индексирование данных"
      content: "Увеличьте производительность поиска, создавая повторно используемые индексы. Структурированное индексирование ускоряет поиск документов и улучшает точность."

    # feature loop
    - title: "Поддержка нескольких языков"
      content: "Ищите документы на более чем 80 языках с поддержкой различных раскладок клавиатуры и морфологических вариантов слов, обеспечивая точные результаты."

    # feature loop
    - title: "Расширенные параметры поиска"
      content: "Настраивайте поиск с учетом регистра, нечеткого сопоставления, обнаружения омографов, фильтрации документов и других мощных функций."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Использование продвинутых техник поиска"
      content: |
        Узнайте, как формировать запросы для поиска в TXT.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Определите каталог индекса поиска
          const index = new searchLib.Index("c:/MyIndex");
              
          // Установите путь к целевым документам
          index.add("c:/MyDocuments");

          // Создайте запрос для нужной фразы
          const word1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wildcard = searchLib.SearchQuery.createWildcardQuery(1, 7);
          const word2 = searchLib.SearchQuery.createWordQuery("dolor");

          const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Получите результаты поиска
          const result = index.search(query);
          
          // Обработайте и используйте результаты
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
            link: "/examples/search/formats/searchphrase.txt"
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
    title: "Расширенные возможности поиска"
    exclude: "phrase"
    description: "Используйте мощные функции поиска для более быстрых и точных результатов."
    items: 
          
        # operation loop 1
        - name: "Поиск по условию"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Находите информацию в документах, используя булевы условия"

        # operation loop 2
        - name: "Чувствительный к регистру поиск"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Улучшите точность поиска, учитывая регистр"

        # operation loop 3
        - name: "Индексирование документов"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "Индексируйте документы один раз и повторно используйте индекс для множества поисков"

        # operation loop 4
        - name: "Поисковые фильтры"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "Используйте фильтры для уточнения обрабатываемых данных"

        # operation loop 5
        - name: "Точная фраза"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Ищите конкретное предложение или фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Поиск фраз в деловых документах"
    exclude: "TXT"
    description: "GroupDocs.Search поддерживает поиск фраз более чем в 70 форматах документов. Используйте расширенные параметры и индексирование для оптимизации процесса поиска."
    items: 
        # format loop 1
        - name: "Поиск фразы в DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/phrase/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Поиск фразы в PDF"
          format: "PDF"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: "Поиск фразы в PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: "Поиск фразы в TXT"
          format: "TXT"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: "Поиск фразы в XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---