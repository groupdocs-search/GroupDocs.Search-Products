
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: uk
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Пошук фраз у PPTX за допомогою Node.js"
head_description: "GroupDocs.Search for Node.js via Java додає потужну функціональність пошуку фраз до застосунків JavaScript для ефективного пошуку документів."

############################# Header ############################
title: "Знайдіть фрази в документах" 
description: "Швидко знаходьте конкретні фрази за допомогою GroupDocs.Search for Node.js via Java. Інтегруйте швидкі та точні можливості пошуку у ваші застосунки Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Завантажити"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Можливості GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "Дізнатися більше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) — це бібліотека високої продуктивності для індексації та пошуку тексту в документах. Вона підтримує понад 70 форматів файлів, включаючи PDF, документи Word, електронні таблиці Excel, зображення та ZIP-архіви, що забезпечує точні та швидкі результати пошуку.

############################# Steps ############################
steps:
    enable: true
    title: "Як знайти фрази у документах PPTX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) спрощує пошук фраз у документах PPTX. Застосуйте різні параметри пошуку, щоб уточнити результати в застосунках Node.js via Java.
      
      1. Налаштуйте папку для індексу пошуку.
      2. Визначте папку, що містить файли PPTX.
      3. Налаштуйте параметри пошуку.
      4. Отримайте та обробіть результати пошуку.
   
    code:
      platform: "nodejs-java"
      copy_title: "Копіювати"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Результат пошуку"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "клікніть, щоб скопіювати"
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

        // Вкажіть шлях для зберігання індексу пошуку
        const index = new searchLib.Index("c:/MyIndex");

        // Встановіть папку з документами
        index.add("c:/MyDocuments");

        // Налаштуйте параметри пошуку
        const word1 = searchLib.SearchQuery.createWordQuery("lorem");
        const word2 = searchLib.SearchQuery.createWordQuery("ipsum");
        const word3 = searchLib.SearchQuery.createWordQuery("dolor");

        const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, word2, word3);

        // Виконайте запит на пошук
        const result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Відкрийте для себе пошуковий двигун документів Node.js"
  description: "GroupDocs.Search for Node.js via Java дозволяє виконувати пошук фраз у понад 70 форматах файлів, що полегшує знаходження та організацію даних за допомогою розширених функцій пошуку."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Основні можливості GroupDocs.Search"
  features:
    # feature loop
    - title: "Пошук фраз"
      content: "Знайдіть точні фрази в ділових документах, таких як PDF, файли Word, презентації та електронні таблиці. Використовуйте підстановчі знаки та гнучкі параметри пошуку, коли повна фраза невідома."

    # feature loop
    - title: "Оптимізований індекс даних"
      content: "Підвищте продуктивність пошуку, створюючи багаторазові індекси. Структуроване індексування прискорює пошук документів та покращує точність."

    # feature loop
    - title: "Сумісність з багатьма мовами"
      content: "Виконуйте пошук у документах понад 80 мовами з підтримкою різних розкладок клавіатури та морфологічних варіацій слів, забезпечуючи точні результати."

    # feature loop
    - title: "Розширені параметри пошуку"
      content: "Налаштуйте пошукові запити з урахуванням регістру, нечіткого відповідності, виявлення омонімів, фільтрації документів та інших потужних функцій."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Використання розширених методів пошуку"
      content: |
        Дізнайтеся, як будувати запити для пошуку в PPTX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Визначте директорію для індексу пошуку
          const index = new searchLib.Index("c:/MyIndex");
              
          // Встановіть шлях до цільових документів
          index.add("c:/MyDocuments");

          // Створіть запит для бажаної фрази
          const word1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wildcard = searchLib.SearchQuery.createWildcardQuery(1, 7);
          const word2 = searchLib.SearchQuery.createWordQuery("dolor");

          const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Отримайте результати пошуку
          const result = index.search(query);
          
          // Обробіть та використайте результати
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "Копіювати"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "клікніть, щоб скопіювати"
          copy_done: "скопійовано"
        top_links:
          #  loop
          - title: "Завантажити результат"
            icon: "download"
            link: "/examples/search/formats/searchphrase.pptx"
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
  title: "Готові розпочати?"
  description: "Спробуйте функції GroupDocs.Search безкоштовно або запитайте ліцензію"
  items:
    #  loop
    - title: "Завантажити NPM"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "Ліцензування"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Розширені можливості пошуку"
    exclude: "phrase"
    description: "Використовуйте потужні функції пошуку для швидших і точніших результатів."
    items: 
          
        # operation loop 1
        - name: "Пошук за умовою"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "Знайти інформацію в документах, використовуючи логічні умови"

        # operation loop 2
        - name: "Пошук чутливий до регістру"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "Покращте точність пошуку, враховуючи чутливість до регістру"

        # operation loop 3
        - name: "Індексація документів"
          operation: "document"
          link: "/search/nodejs-java/document/pptx/"
          description: "Індексуйте документи один раз та повторно використовуйте індекс для кількох пошуків"

        # operation loop 4
        - name: "Фільтри пошуку"
          operation: "filters"
          link: "/search/nodejs-java/filters/pptx/"
          description: "Використовуйте фільтри для звуження оброблюваних даних"

        # operation loop 5
        - name: "Точна фраза"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "Шукайте конкретне речення або фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Пошук фраз у ділових документах"
    exclude: "PPTX"
    description: "GroupDocs.Search підтримує пошук фраз у понад 70 форматах документів. Використовуйте розширені параметри та індексування для оптимізації процесу пошуку."
    items: 
        # format loop 1
        - name: "Пошук фрази у DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/phrase/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Пошук фрази у PDF"
          format: "PDF"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "Формат Adobe Portable Document"
          
        # format loop 3
        - name: "Пошук фрази у PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "Презентація PowerPoint Open XML"

        # format loop 4
        - name: "Пошук фрази у TXT"
          format: "TXT"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Текстовий документ"
          
        # format loop 5
        - name: "Пошук фрази у XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Таблиця Microsoft Excel Open XML"
  

---