
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: uk
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Пошук у документах TXT з використанням .NET"
head_description: "GroupDocs.Search for .NET покращує додатки C# завдяки ефективному текстовому пошуку в різних форматах бізнес-документів."

############################# Header ############################
title: "Пошук тексту в бізнес-документах" 
description: "GroupDocs.Search for .NET забезпечує потужні та гнучкі текстові запити у ваших документах. Інтегруйте функціональність пошуку в додатки .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Скачати безкоштовно"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Що таке GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Дізнатися більше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) — потужна бібліотека для ефективного текстового пошуку та індексації документів. Вона підтримує понад 70 форматів файлів, включаючи стандартні документи, такі як PDF, Word, Excel та PowerPoint. Поліпшуйте продуктивність пошуку з швидкими та точними результатами.

############################# Steps ############################
steps:
    enable: true
    title: "Як шукати у даних TXT"
    content: |
      [GroupDocs.Search](/search/net/) забезпечує ефективний текстовий пошук у документах TXT, що робить його ідеальним для додатків .NET.
      
      1. Налаштуйте папку для зберігання пошукового індексу.
      2. Виберіть папку, що містить ваші файли.
      3. Налаштуйте параметри пошуку для обробки лише документів TXT.
      4. Виконайте пошук та отримайте результати.
   
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
        // Шлях для збереження повторно використовуваного пошукового індексу
        Index index = new Index("c:/MyIndex");

        // Папка з документами
        index.Add("c:/MyDocuments");

        // Шукати лише у певних форматах файлів
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".txt");

        // Отримати результати пошуку
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Розширені функції пошуку"
  description: "GroupDocs.Search for .NET забезпечує складні текстові запити по більше ніж 70 форматах файлів. Індексація підвищує ефективність пошуку та допомагає ефективно керувати вмістом документів."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Основні функції GroupDocs.Search"
  features:
    # feature loop
    - title: "Розширений текстовий пошук"
      content: "Витягайте релевантний текст з популярних бізнес-документів, включаючи PDF, файли Word, презентації та електронні таблиці. Підтримує кілька методів пошуку, таких як нечіткий пошук, виявлення однозвучності та підстановочні знаки."

    # feature loop
    - title: "Оптимізована індексація для швидших пошуків"
      content: "Створюйте та повторно використовуйте пошукові індекси для покращення швидкості пошуку. Індексація оптимізує продуктивність при пошуку серед великих колекцій документів."

    # feature loop
    - title: "Підтримка кількох мов"
      content: "Виконуйте пошук у документах, написаних більш ніж 80 мовами. Визначає різні розкладки клавіатури та варіанти слів для підвищення точності."

    # feature loop
    - title: "Гнучкі налаштування пошуку"
      content: "Уточнюйте результати пошуку з допомогою налаштовуваних опцій, включаючи фільтри, регулярні вирази та налаштування чутливості до регістру."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Фільтруйте документи для обробки"
      content: |
        Дізнайтеся, як звузити пошук документів за допомогою фільтрів.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Налаштуйте індекс, який виключає певні формати файлів.
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.CreateFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter);
          settings.DocumentFilter = invertedFilter;

          Index index = new Index("c:/MyIndex", settings);
              
          // Вкажіть директорію документів.
          index.Add("c:/MyDocuments");

          // Отримайте результати пошуку.
          SearchResult result = index.Search("Lorem");
          
          // Обробіть та використовуйте вихідні дані пошуку.
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
            link: "/examples/search/formats/searchfilters.txt"
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
    title: "Ключові функції"
    exclude: "filters"
    description: "Виконуйте точні та ефективні пошуки даних."
    items: 
          
        # operation loop 1
        - name: "Пошук за умовою"
          operation: "boolean"
          link: "/search/net/boolean/txt/"
          description: "Знайти інформацію в документах, використовуючи логічні умови"

        # operation loop 2
        - name: "Пошук чутливий до регістру"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/txt/"
          description: "Покращте точність пошуку, враховуючи чутливість до регістру"

        # operation loop 3
        - name: "Індексація документів"
          operation: "document"
          link: "/search/net/document/txt/"
          description: "Індексуйте документи один раз та повторно використовуйте індекс для кількох пошуків"

        # operation loop 4
        - name: "Фільтри пошуку"
          operation: "filters"
          link: "/search/net/filters/txt/"
          description: "Використовуйте фільтри для звуження оброблюваних даних"

        # operation loop 5
        - name: "Точна фраза"
          operation: "phrase"
          link: "/search/net/phrase/txt/"
          description: "Шукайте конкретне речення або фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Знайдіть дані у ваших бізнес-документах"
    exclude: "TXT"
    description: "GroupDocs.Search підтримує понад 70 форматів файлів, що дозволяє ефективно обробляти та шукати популярні офісні документи."
    items: 
        # format loop 1
        - name: "Фільтри для пошуку у DOCX"
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Фільтри для пошуку у PDF"
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "Формат Adobe Portable Document"
          
        # format loop 3
        - name: "Фільтри для пошуку у PPTX"
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "Презентація PowerPoint Open XML"

        # format loop 4
        - name: "Фільтри для пошуку у TXT"
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "Текстовий документ"
          
        # format loop 5
        - name: "Фільтри для пошуку у XLSX"
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "Таблиця Microsoft Excel Open XML"
  

---