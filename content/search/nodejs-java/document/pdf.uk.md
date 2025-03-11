
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:35
draft: false
lang: uk
format: Pdf
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Знайдіть текст у PDF за допомогою GroupDocs.Search в Node.js"
head_description: "Використовуйте GroupDocs.Search for Node.js via Java з JavaScript для ефективного пошуку тексту в різних форматах документів."

############################# Header ############################
title: "Розумне рішення для пошуку документів" 
description: "Легко знаходьте текст у різних форматах документів за допомогою GroupDocs.Search for Node.js via Java. Створюйте розширені запити на пошук у ваших програмах для Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Спробуйте безкоштовно"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Огляд GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "Дізнатися більше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) — це бібліотека високої продуктивності для повнотекстового пошуку та індексації документів. Вона підтримує понад 70 типів файлів, включаючи PDF, Word, PowerPoint, Excel, зображення та ZIP-архіви, забезпечуючи швидкі та точні результати.

############################# Steps ############################
steps:
    enable: true
    title: "Виконання пошуку у файлах PDF"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) дозволяє виконувати пошук у файлах PDF, уточнюючи результати в програмах Node.js via Java.
      
      1. Визначте папку для зберігання індексу пошуку.
      2. Виберіть папку з файлами PDF.
      3. Встановіть додаткові параметри пошуку.
      4. Запустіть пошук та проаналізуйте результати.
   
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

        // Вкажіть каталог для зберігання індексу пошуку
        const index = new searchLib.Index("c:/MyIndex");

        // Виберіть папку, що містить документи для пошуку
        index.add("c:/MyDocuments");

        // Увімкніть пошук омонімів для слів, які звучать подібно
        const options = new searchLib.SearchOptions();
        options.setUseHomophoneSearch(true);

        // Запустіть складний запит пошуку
        const result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Розширені можливості пошуку та індексації"
  description: "GroupDocs.Search for Node.js via Java забезпечує потужні інструменти для пошуку тексту та індексації у понад 70 форматах документів, що спрощує знаходження та організацію інформації."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Основні переваги GroupDocs.Search"
  features:
    # feature loop
    - title: "Вичерпний текстовий пошук"
      content: "Знаходьте текст у декількох типах документів, включаючи PDF, Word документи, презентації PowerPoint та електронні таблиці. Використовуйте точні збіги, нечіткий пошук та символи підстановки для уточнення результатів."

    # feature loop
    - title: "Ефективна індексація для великих обсягів даних"
      content: "Прискорте пошук, створюючи структуровані індекси, що полегшує отримання інформації з великих колекцій документів."

    # feature loop
    - title: "Підтримує 80+ мов"
      content: "Пошук у документах різними мовами, з автоматичним розпізнаванням різних форм слів та розкладок клавіатури."

    # feature loop
    - title: "Користувацькі налаштування пошуку"
      content: "Налаштуйте параметри пошуку, такі як чутливість до регістру, фільтри за датою та виключення слів для точних результатів."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Використання пошуку для документів PDF"
      content: |
        Цей приклад демонструє, як використовувати запити на пошук у документах PDF.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Вкажіть каталог для індексації пошуку
          const index = new searchLib.Index("c:/MyIndex");
              
          // Вкажіть шлях до файлу для зберігання документів
          index.add("c:/MyDocuments");

          // Введіть пароль для захищених файлів
          index.getDictionaries().getDocumentPasswords().add("protected.pdf", '123456');

          // Увімкніть нечіткий пошук для виявлення схожих слів
          const options = new searchLib.SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new searchLib.SimilarityLevel(0.8));

          // Екстрактуйте результати пошуку
          const result = index.search("Loarem", options);
          
          // Обробіть і перевірте результати
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
            link: "/examples/search/formats/searchdocument.pdf"
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
    title: "Ознайомтеся з основними функціями"
    exclude: "document"
    description: "Відкрийте для себе функції швидкого пошуку, які покликані підвищити ефективність та точність."
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
    title: "Пошук у різноманітних документах"
    exclude: "PDF"
    description: "GroupDocs.Search працює з понад 70 форматами файлів, включаючи офісні документи, що забезпечує швидкий і точний пошук з підтримкою індексації."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/document/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/document/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/document/pptx/"
          description: "Презентація PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/document/txt/"
          description: "Текстовий документ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Таблиця Microsoft Excel Open XML"
  

---