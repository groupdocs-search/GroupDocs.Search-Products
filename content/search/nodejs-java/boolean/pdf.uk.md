
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:30
draft: false
lang: uk
format: Pdf
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Булевий пошук PDF через Node.js"
head_description: "Використовуйте API GroupDocs.Search for Node.js via Java для виконання вдосконалених пошуків у вмісті документів з булевими операторами такими як AND, OR та NOT, спеціально розроблений для розробників на JavaScript."

############################# Header ############################
title: "Виконуйте пошуки з булевою логікою" 
description: "За допомогою GroupDocs.Search for Node.js via Java ви можете створювати вдосконалені пошукові запити, використовуючи булеві оператори (AND, OR, NOT) безперешкодно у вашому середовищі Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Завантажити зараз"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Що таке GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Дізнатися більше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) - це потужний інструмент для пошуку та індексації тексту в документах. Він підтримує понад 70 форматів, таких як PDF, Word, Excel, PowerPoint, зображення та ZIP файли, що дозволяє ефективно обробляти великі обсяги інформації.

############################# Steps ############################
steps:
    enable: true
    title: "Як шукати в документах PDF за допомогою булевих операторів"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) дозволяє ефективно шукати вміст у файлах PDF. Використовуючи булеву логіку, ви можете уточнити свої пошукові запити в застосунках Node.js via Java для покращення точності.
      
      1. Налаштуйте папку для зберігання індексу пошуку.
      2. Виберіть папку, що містить файли PDF для пошуку.
      3. Запустіть пошуковий запит та отримайте результати.
      4. Обробіть та проаналізуйте результати пошуку.
   
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

        // Встановіть місце для папки індексу
        const index = new searchLib.Index("c:/MyIndex");

        // Вкажіть папку, що містить документи для пошуку
        index.add("c:/MyDocuments");

        // Виконайте пошуковий запит з використанням вдосконаленої логіки
        const result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Потужні інструменти для пошуку та індексації документів"
  description: "GroupDocs.Search for Node.js via Java спрощує пошук тексту та індексацію для понад 70 типів файлів, що допомагає вам швидше знаходити та управляти інформацією з точністю."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Ключові функції GroupDocs.Search"
  features:
    # feature loop
    - title: "Покращений текстовий пошук"
      content: "Швидко знаходьте текст у різних форматах, таких як PDF, документи Word, презентації та електронні таблиці. Використовуйте такі функції, як точні збіги, пошук з використанням символів підстановки та нечіткий пошук для точних результатів."

    # feature loop
    - title: "Ефективна індексація даних"
      content: "Створюйте та керуйте індексами для прискорення пошуку у великих колекціях документів. Індексація забезпечує швидкий і структурований доступ до ваших даних."

    # feature loop
    - title: "Підтримка багатьох мов"
      content: "Шукайте в документах, написаних більш ніж 80 мовами. Морфологічна підтримка та сумісність з розкладкою клавіатури покращують результати пошуку на різних мовах."

    # feature loop
    - title: "Гнучкі налаштування пошуку"
      content: "Налаштуйте свій пошук, включивши чутливість до регістру, застосувавши фільтри за датою або пропускаючи певні слова та дані під час індексації."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Приклад вдосконаленого булевого пошуку"
      content: |
        Цей приклад демонструє, як створити запити на основі булевої логіки для пошуку вмісту у документах PDF.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Визначте папку для індексу пошуку
          const index = new searchLib.Index("c:/MyIndex");
              
          // Вкажіть розташування документів для пошуку
          index.add("c:/MyDocuments");

          // Сформулюйте запит, використовуючи булеві оператори
          const wordQuery1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wordQuery2 = searchLib.SearchQuery.createWordQuery("ipsum");
          const booleanQuery = searchLib.SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Отримайте результати пошуку
          const result = index.search(booleanQuery);
          
          // Обробіть та використовуйте результати пошуку
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
            link: "/examples/search/formats/searchboolean.pdf"
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
    title: "Ключові можливості GroupDocs.Search"
    exclude: "boolean"
    description: "Відкрийте для себе вдосконалені, ефективні та налаштовувані функції пошуку."
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
    title: "Шукайте популярні формати документів"
    exclude: "PDF"
    description: "GroupDocs.Search підтримує понад 70 форматів файлів, надаючи гнучкі правила пошуку і ефективну індексацію для економії часу та зусиль."
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
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "Презентація PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Текстовий документ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Таблиця Microsoft Excel Open XML"
  

---