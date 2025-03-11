
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:30
draft: false
lang: ru
format: Pdf
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Булевый поиск PDF через Node.js"
head_description: "Используйте API GroupDocs.Search for Node.js via Java для выполнения продвинутых поисков в содержимом документов с булевыми операторами, такими как AND, OR и NOT, ориентированного на разработчиков JavaScript."

############################# Header ############################
title: "Выполнение поисков с булевой логикой" 
description: "С помощью GroupDocs.Search for Node.js via Java вы можете легко создавать сложные поисковые запросы, используя булевые операторы (AND, OR, NOT) в вашем окружении Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачать сейчас"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Что такое GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Узнать больше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) — это мощный инструмент для поиска и индексирования текста в документах. Он поддерживает более 70 форматов, таких как PDF, Word, Excel, PowerPoint, изображения и ZIP-файлы, что позволяет эффективно обрабатывать большие объемы информации.

############################# Steps ############################
steps:
    enable: true
    title: "Как искать в документах PDF с использованием булевых операторов"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) позволяет эффективно искать контент в файлах PDF. С помощью булевой логики вы можете уточнить ваши поисковые запросы в приложениях Node.js via Java для улучшения точности.
      
      1. Настройте папку для хранения поискового индекса.
      2. Выберите папку, содержащую файлы PDF для поиска.
      3. Запустите поисковый запрос и получите результаты.
      4. Обработайте и проанализируйте результаты поиска.
   
    code:
      platform: "nodejs-java"
      copy_title: "Копировать"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
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

        // Установите местоположение для папки индекса
        const index = new searchLib.Index("c:/MyIndex");

        // Укажите папку, содержащую документы для поиска
        index.add("c:/MyDocuments");

        // Выполните поисковый запрос с использованием продвинутой логики
        const result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Мощные инструменты для поиска и индексирования документов"
  description: "GroupDocs.Search for Node.js via Java упрощает поиск текста и индексирование более чем 70 типов файлов, помогая вам быстрее находить и управлять информацией с точностью."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Ключевые функции GroupDocs.Search"
  features:
    # feature loop
    - title: "Расширенный текстовый поиск"
      content: "Быстро находите текст в различных форматах, таких как PDF, документы Word, презентации и таблицы. Используйте функции, такие как точные совпадения, подстановочные запросы и нечеткий поиск для получения точных результатов."

    # feature loop
    - title: "Эффективное индексирование данных"
      content: "Создавайте и управляйте индексами, чтобы ускорить поиск в больших коллекциях документов. Индексирование обеспечивает быстрый и структурированный доступ к вашим данным."

    # feature loop
    - title: "Многоязычная поддержка"
      content: "Ищите в документах, написанных более чем на 80 языках. Морфологическая поддержка и совместимость раскладок клавиатуры улучшают результаты поиска на разных языках."

    # feature loop
    - title: "Гибкие настройки поиска"
      content: "Настройте свой поиск, включив чувствительность к регистру, применяя фильтры по дате или пропуская конкретные слова и данные во время индексирования."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Пример продвинутого булевого поиска"
      content: |
        Этот пример демонстрирует, как создать запросы на основе булевой логики для поиска контента в документах PDF.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Определите папку для поискового индекса
          const index = new searchLib.Index("c:/MyIndex");
              
          // Укажите местоположение документов для поиска
          index.add("c:/MyDocuments");

          // Сформируйте запрос с использованием булевых операторов
          const wordQuery1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wordQuery2 = searchLib.SearchQuery.createWordQuery("ipsum");
          const booleanQuery = searchLib.SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Получите результаты поиска
          const result = index.search(booleanQuery);
          
          // Обработайте и используйте результаты поиска
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
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchboolean.pdf"
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
  description: "Попробуйте возможности GroupDocs.Search бесплатно или запросите лицензию"
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
    title: "Ключевые возможности GroupDocs.Search"
    exclude: "boolean"
    description: "Откройте для себя продвинутые, эффективные и настраиваемые функции поиска."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/pdf/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/pdf/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Поиск популярных форматов документов"
    exclude: "PDF"
    description: "GroupDocs.Search поддерживает более 70 форматов файлов, предоставляя гибкие правила поиска и эффективное индексирование для экономии времени и усилий."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/boolean/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "Формат переносимого документа Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "Презентация PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Текстовый документ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
  

---