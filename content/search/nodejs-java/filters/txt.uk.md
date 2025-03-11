
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:38
draft: false
lang: uk
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Пошук у документах TXT за допомогою Node.js"
head_description: "GroupDocs.Search for Node.js via Java додає швидкі та точні можливості текстового пошуку в додатках JavaScript, підтримуючи численні формати документів."

############################# Header ############################
title: "Знайдіть текст у бізнес-документах" 
description: "GroupDocs.Search for Node.js via Java забезпечує потужну та гнучку функціональність пошуку для документів. Інтегруйте текстовий пошук у додатки Node.js."
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
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) - це надійна бібліотека для пошуку та індексування, яка забезпечує швидке отримання тексту в документах. Вона підтримує понад 70 форматів файлів, включаючи PDF, Word, Excel та PowerPoint, що гарантує точний та ефективний пошук.

############################# Steps ############################
steps:
    enable: true
    title: "Як виконати пошук у документах TXT"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) спрощує та підвищує ефективність пошуку тексту в документах TXT для додатків Node.js via Java.
      
      1. Створіть каталог для зберігання індексу пошуку.
      2. Виберіть папку, що містить документи.
      3. Встановіть параметри пошуку, щоб включити лише файли TXT.
      4. Запустіть пошук та отримайте результати.
   
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

        // Визначте каталог для зберігання індексу пошуку
        const index = new searchLib.Index("c:/MyIndex");

        // Вкажіть папку, що містить документи для пошуку
        index.add("c:/MyDocuments");

        // Обмежте пошук лише певними форматами файлів
        const options = new searchLib.SearchOptions();
        options.SearchDocumentFilter = 
            searchLib.SearchDocumentFilter.createFileExtension(".txt");

        // Отримайте та обробіть результати пошуку
        const result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Розширені можливості пошуку"
  description: "GroupDocs.Search for Node.js via Java підвищує ефективність пошуку документів, індексуючи понад 70 форматів файлів. Оптимізуйте отримання вмісту за допомогою розширених технік пошуку."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Ключові функції GroupDocs.Search"
  features:
    # feature loop
    - title: "Всеохоплюючий текстовий пошук"
      content: "Витягуйте та знаходьте текст у популярних форматах документів, таких як PDF, Word, електронні таблиці та презентації. Підтримується нечіткий пошук, омоніми та запити з підстановками."

    # feature loop
    - title: "Оптимізоване індексування для продуктивності"
      content: "Прискорте пошук, створюючи багаторазові індекси. Підвищує швидкість та ефективність при роботі з великими колекціями документів."

    # feature loop
    - title: "Підтримка кількох мов"
      content: "Шукайте в документах більше ніж 80 мовами. Визначає розкладки клавіатури та варіації слів для кращої точності."

    # feature loop
    - title: "Налаштовувані параметри пошуку"
      content: "Тонко налаштуйте результати пошуку за допомогою фільтрів, регулярних виразів, чутливості до регістру та інших гнучких налаштувань."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Фільтруйте документи для пошуку"
      content: |
        Дізнайтеся, як уточнити пошук документів, використовуючи фільтри.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Налаштуйте індекс, щоб виключити небажані формати файлів
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            searchLib.DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = 
            searchLib.DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new searchLib.Index("c:/MyIndex", settings);
              
          // Вкажіть каталог, що містить документи
          index.add("c:/MyDocuments");

          // Обробіть результати пошуку для подальшого використання
          const result = index.Search("Lorem", options);
          
          // Обробіть результати пошуку для подальшого використання
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
            link: "/examples/search/formats/searchfilters.txt"
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
    exclude: "filters"
    description: "Виконуйте швидкі та точні текстові пошуки в документах."
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
    title: "Пошук у різноманітних форматах документів"
    exclude: "TXT"
    description: "GroupDocs.Search підтримує понад 70 типів файлів, що дозволяє ефективно шукати текст у різних офісних та бізнес-документах."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/filters/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/filters/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/filters/pptx/"
          description: "Презентація PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/filters/txt/"
          description: "Текстовий документ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Таблиця Microsoft Excel Open XML"
  

---