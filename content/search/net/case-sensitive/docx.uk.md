
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: uk
format: Docx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Пошук з урахуванням регістру в DOCX за допомогою .NET"
head_description: "API GroupDocs.Search for .NET дозволяє розробникам C# виконувати пошук з урахуванням регістру в різних документах."

############################# Header ############################
title: "Пошук з урахуванням регістру" 
description: "GroupDocs.Search for .NET спрощує створення складних запитів пошуку з урахуванням регістру у ваших програмах .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Завантажити безкоштовно"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Що таке GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Дізнатися більше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) — це потужна бібліотека для пошуку тексту та індексації в документах. Вона підтримує понад 70 форматів файлів, включно з PDF, Word, PowerPoint, Excel, зображеннями та ZIP-файлами, забезпечуючи ефективну обробку великих обсягів даних.

############################# Steps ############################
steps:
    enable: true
    title: "Як виконати пошук з урахуванням регістру в документах DOCX"
    content: |
      [GroupDocs.Search](/search/net/) спрощує пошук з урахуванням регістру в документах DOCX. Використовуйте його для уточнення результатів у програмах .NET.
      
      1. Визначте папку для зберігання індексу пошуку.
      2. Виберіть папку, що містить файли DOCX.
      3. Виконайте пошук і отримайте результати.
      4. Обробіть результати.
   
    code:
      platform: "net"
      copy_title: "Копіювати"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Результат пошуку"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "клікніть, щоб скопіювати"
        copy_done: "скопійовано"
      links:
        #  loop
        - title: "Більше прикладів"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "Документація"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // Встановіть шлях до папки з індексом
        Index index = new Index("c:/MyIndex");

        // Вкажіть папку, що містить документи для пошуку
        index.Add("c:/MyDocuments");

        // Увімкніть пошук з урахуванням регістру в параметрах
        SearchOptions options = new SearchOptions();
        options.UseCaseSensitiveSearch = true;

        // Виконайте пошук
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Розширені функції для пошуку та індексації документів"
  description: "Бібліотека GroupDocs.Search for .NET спрощує пошук тексту та індексацію в понад 70 форматах файлів. З легкістю знаходьте та керуйте інформацією за допомогою потужних інструментів пошуку."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Ключові особливості GroupDocs.Search"
  features:
    # feature loop
    - title: "Розширений текстовий пошук"
      content: "Виконуйте пошук тексту в різних форматах файлів, включно з PDF, документами Word, електронними таблицями та презентаціями. Використовуйте параметри, такі як точні збіги, нечіткий пошук та шаблони для отримання точних результатів."

    # feature loop
    - title: "Індексація великих обсягів даних"
      content: "Створюйте та підтримуйте індекси для швидших пошуків. Організована індексація спрощує пошук у великих колекціях документів."

    # feature loop
    - title: "Підтримка багатьох мов"
      content: "Виконуйте пошук у документах більш ніж 80 мовами, з підтримкою різних розкладок клавіатури та форм слів для отримання більш точних результатів."

    # feature loop
    - title: "Налаштовувані параметри пошуку"
      content: "Налаштуйте параметри пошуку, включаючи чутливість до регістру, фільтри за діапазоном дат та можливість виключення конкретних слів чи даних під час індексації."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Використання запитів на пошук з урахуванням регістру"
      content: |
        Цей приклад демонструє, як використовувати запити з урахуванням регістру для пошуку в документах DOCX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Встановіть папку для індексу пошуку
          Index index = new Index("c:/MyIndex");
              
          // Вкажіть шлях до документів, що підлягають пошуку
          index.Add("c:/MyDocuments");

          // Створіть запит на пошук
          SearchQuery wordQuery = SearchQuery.CreateWordQuery("Lorem");

          // Увімкніть параметри пошуку з урахуванням регістру
          SearchOptions options = new SearchOptions();
          options.UseCaseSensitiveSearch = true;

          // Шукайте текст у документах
          SearchResult result = index.Search(wordQuery, options);
          
          // Обробіть результати пошуку
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "Копіювати"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "клікніть, щоб скопіювати"
          copy_done: "скопійовано"
        top_links:
          #  loop
          - title: "Завантажити результат"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.docx"
        links:
          #  loop
          - title: "Більше прикладів"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "Документація"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Готові розпочати?"
  description: "Спробуйте функції GroupDocs.Search безкоштовно або запитайте ліцензію"
  items:
    #  loop
    - title: "Завантажити Nuget"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "Ліцензування"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Відкрийте ключові функції"
    exclude: "case-sensitive"
    description: "Вивчайте розширені та ефективні функціональні можливості пошуку."
    items: 
          
        # operation loop 1
        - name: "Пошук за умовою"
          operation: "boolean"
          link: "/search/net/boolean/docx/"
          description: "Знайти інформацію в документах, використовуючи логічні умови"

        # operation loop 2
        - name: "Пошук чутливий до регістру"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/docx/"
          description: "Покращте точність пошуку, враховуючи чутливість до регістру"

        # operation loop 3
        - name: "Індексація документів"
          operation: "document"
          link: "/search/net/document/docx/"
          description: "Індексуйте документи один раз та повторно використовуйте індекс для кількох пошуків"

        # operation loop 4
        - name: "Фільтри пошуку"
          operation: "filters"
          link: "/search/net/filters/docx/"
          description: "Використовуйте фільтри для звуження оброблюваних даних"

        # operation loop 5
        - name: "Точна фраза"
          operation: "phrase"
          link: "/search/net/phrase/docx/"
          description: "Шукайте конкретне речення або фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Пошук популярних форматів документів"
    exclude: "DOCX"
    description: "GroupDocs.Search підтримує понад 70 форматів файлів. Налаштуйте правила пошуку та використовуйте індексацію для економії часу та зусиль."
    items: 
        # format loop 1
        - name: "Чутливий до регістру пошук у DOCX"
          format: "DOCX"
          link: "/search/net/case-sensitive/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Чутливий до регістру пошук у PDF"
          format: "PDF"
          link: "/search/net/case-sensitive/pdf/"
          description: "Формат Adobe Portable Document"
          
        # format loop 3
        - name: "Чутливий до регістру пошук у PPTX"
          format: "PPTX"
          link: "/search/net/case-sensitive/pptx/"
          description: "Презентація PowerPoint Open XML"

        # format loop 4
        - name: "Чутливий до регістру пошук у TXT"
          format: "TXT"
          link: "/search/net/case-sensitive/txt/"
          description: "Текстовий документ"
          
        # format loop 5
        - name: "Чутливий до регістру пошук у XLSX"
          format: "XLSX"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Таблиця Microsoft Excel Open XML"
  

---