
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:33
draft: false
lang: uk
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Виконання чутливих до регістру пошуків у TXT з Node.js"
head_description: "API GroupDocs.Search for Node.js via Java дозволяє розробникам JavaScript виконувати чутливі до регістру пошуки серед різних типів документів."

############################# Header ############################
title: "Чутливий до регістру пошук" 
description: "GroupDocs.Search for Node.js via Java дозволяє реалізувати розширену функціональність чутливого до регістру пошуку у ваших приложеннях Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Завантажити безкоштовно"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Що таке GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Дізнатися більше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) — потужна бібліотека для пошуку та індексації тексту у документах. Вона підтримує понад 70 форматів, включаючи PDF, Word, Excel, PowerPoint, зображення та ZIP-файли, що дозволяє ефективно обробляти великі обсяги даних.

############################# Steps ############################
steps:
    enable: true
    title: "Кроки для виконання чутливих до регістру пошуків у файлах TXT"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) спрощує виконання чутливих до регістру пошуків у файлах TXT, покращуючи ваші робочі процеси Node.js via Java.
      
      1. Налаштуйте папку для зберігання індексу пошуку.
      2. Виберіть папку, що містить файли TXT.
      3. Запустіть пошук і отримайте результати.
      4. Обробіть та використайте результати.
   
    code:
      platform: "nodejs-java"
      copy_title: "Копіювати"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "клікніть для копіювання"
        copy_done: "скопійовано"
      links:
        #  loop
        - title: "Більше прикладів"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "Документація"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // Вкажіть шлях до папки індексу
        const index = new searchLib.Index("c:/MyIndex");

        // Встановіть папку, що містить документи для пошуку
        index.add("c:/MyDocuments");

        // Увімкніть налаштування чутливого до регістру пошуку
        const options = new groupdocs.search.SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Виконайте пошук
        const result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Ключові функції для пошуку та індексації документів"
  description: "За допомогою GroupDocs.Search for Node.js via Java ви можете виконувати пошук і індексацію тексту в понад 70 форматах документів. Доступ до інформації та її організація здійснюється легко завдяки розширеним інструментам пошуку."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Основні функції GroupDocs.Search"
  features:
    # feature loop
    - title: "Комплексний текстовий пошук"
      content: "Знайдіть текст у різних типах документів, таких як PDF, файли Word, електронні таблиці та презентації. Використовуйте такі опції, як точні збіги, нечіткі пошуки та підстановочні знаки для отримання точних результатів."

    # feature loop
    - title: "Ефективна індексація даних"
      content: "Створюйте та управляйте індексами для прискорення пошуків. Індексація допомагає організувати та швидко знаходити дані у великих колекціях документів."

    # feature loop
    - title: "Підтримка декількох мов"
      content: "Пошук документів більш ніж 80 мовами з підтримкою різних розкладок клавіатури та варіацій слів, що забезпечує точність результатів пошуку."

    # feature loop
    - title: "Налаштовувані параметри пошуку"
      content: "Регулюйте параметри пошуку, включаючи чутливість до регістру, фільтри дат і виключення певних термінів або даних під час індексації."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Приклад: Реалізація чутливого до регістру пошуку"
      content: |
        Цей приклад демонструє, як здійснити чутливі до регістру пошуки для документів TXT.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Визначте папку для індексу пошуку
          const index = new searchLib.Index("c:/MyIndex");
              
          // Надайте шлях до папки документів
          index.add("c:/MyDocuments");

          // Налаштуйте запит на пошук
          const wordQuery = searchLib.SearchQuery.createWordQuery("Lorem");

          // Активуйте налаштування чутливого до регістру пошуку
          const options = new groupdocs.search.SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Шукайте текст у документах
          const result = index.search(wordQuery, options);
          
          // Обробіть і обробіть результати
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "Копіювати"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "клікніть для копіювання"
          copy_done: "скопійовано"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.txt"
        links:
          #  loop
          - title: "Більше прикладів"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "Документація"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Готові почати?"
  description: "Спробуйте функції GroupDocs.Search безкоштовно або запитайте ліцензію"
  items:
    #  loop
    - title: "завантаження NPM"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "Ліцензування"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Ключові функціональні можливості"
    exclude: "case-sensitive"
    description: "Досліджуйте розширені функції для швидкого та точного пошуку документів."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Сумісні формати документів"
    exclude: "TXT"
    description: "GroupDocs.Search підтримує понад 70 форматів документів. Налаштуйте свої параметри пошуку та заощадьте час на індексацію."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "Презентація PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Текстовий документ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Таблиця Microsoft Excel Open XML"
  

---