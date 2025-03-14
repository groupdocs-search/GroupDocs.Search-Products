
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: uk
format: Pdf
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Пошук документів PDF у .NET з GroupDocs.Search"
head_description: "Використовуйте GroupDocs.Search for .NET для виконання ефективних текстових пошуків у різних форматах документів з C#."

############################# Header ############################
title: "Просунутий пошук тексту в документах" 
description: "GroupDocs.Search for .NET спрощує пошук тексту у популярних форматах документів, дозволяючи створювати потужні пошукові запити у ваших додатках .NET."
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
       [GroupDocs.Search for .NET](/search/net/) – потужна бібліотека, створена для повнотекстового пошуку та індексації документів. Вона підтримує понад 70 форматів файлів, включаючи PDF, Word, PowerPoint, Excel, зображення та ZIP-файли, що забезпечує швидкі та точні результати пошуку.

############################# Steps ############################
steps:
    enable: true
    title: "Як виконати текстовий пошук у документах PDF"
    content: |
      [GroupDocs.Search](/search/net/) дозволяє виконувати просунуті операції пошуку вмісту в документах PDF, надаючи уточнені результати пошуку в додатках .NET.
      
      1. Налаштуйте папку для зберігання пошукового індексу.
      2. Виберіть папку, що містить файли PDF.
      3. Настройте додаткові параметри пошуку.
      4. Запустіть пошук і перегляньте результати.
   
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
        // Визначте шлях до пошукового індексу
        Index index = new Index("c:/MyIndex");

        // Виберіть папку, що містить документи для пошуку
        index.Add("c:/MyDocuments");

        // Увімкніть пошук за гомофонами, щоб знаходити слова, які звучать подібно
        SearchOptions options = new SearchOptions();
        options.UseHomophoneSearch = true;

        // Виконайте складний пошуковий запит
        SearchResult result = index.Search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Просунуті можливості пошуку та індексації"
  description: "GroupDocs.Search for .NET покращує текстовий пошук та індексацію у більш ніж 70 форматах файлів, надаючи ефективні інструменти для пошуку та управління інформацією."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Ключові функції GroupDocs.Search"
  features:
    # feature loop
    - title: "Потужний текстовий пошук"
      content: "Шукайте текст у кількох типах документів, включаючи PDF, документи Word, презентації PowerPoint та електронні таблиці. Використовуйте функції, такі як точні співпадіння, нечіткий пошук та підстановочні знаки для уточнення результатів."

    # feature loop
    - title: "Швидка індексація для великих наборів даних"
      content: "Створюйте та керуйте пошуковими індексами для швидкого отримання інформації. Індексація оптимізує пошук у великих колекціях документів."

    # feature loop
    - title: "Підтримка декількох мов"
      content: "Виконуйте пошук більш ніж 80 мовами з підтримкою різних клавіатурних розкладок і варіацій слів для підвищення точності."

    # feature loop
    - title: "Налаштовувані параметри пошуку"
      content: "Тонко налаштуйте параметри пошуку з опціями, такими як чутливість до регістру, фільтри за діапазоном дат і виключення слів для кращих результатів."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Виконання складних пошукових запитів"
      content: |
        Цей приклад демонструє, як застосувати пошукові запити для документів PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Визначте папку для пошукового індексу
          Index index = new Index("c:/MyIndex");
              
          // Вкажіть шлях до документів
          index.Add("c:/MyDocuments");

          // Введіть пароль для захищених документів
          index.Dictionaries.DocumentPasswords.Add("protected.pdf", "123456");

          // Увімкніть нечіткий пошук для знаходження схожих слів
          SearchOptions options = new SearchOptions();
          options.FuzzySearch.Enabled = true;
          options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8);

          // Отримайте результати пошуку
          SearchResult result = index.Search("Loarem", options);
          
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
            link: "/examples/search/formats/searchdocument.pdf"
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
    title: "Вивчайте ключові можливості"
    exclude: "document"
    description: "Скористайтеся просунутими функціоналом пошуку з високою продуктивністю."
    items: 
          
        # operation loop 1
        - name: "Пошук за умовою"
          operation: "boolean"
          link: "/search/net/boolean/pdf/"
          description: "Знайти інформацію в документах, використовуючи логічні умови"

        # operation loop 2
        - name: "Пошук чутливий до регістру"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pdf/"
          description: "Покращте точність пошуку, враховуючи чутливість до регістру"

        # operation loop 3
        - name: "Індексація документів"
          operation: "document"
          link: "/search/net/document/pdf/"
          description: "Індексуйте документи один раз та повторно використовуйте індекс для кількох пошуків"

        # operation loop 4
        - name: "Фільтри пошуку"
          operation: "filters"
          link: "/search/net/filters/pdf/"
          description: "Використовуйте фільтри для звуження оброблюваних даних"

        # operation loop 5
        - name: "Точна фраза"
          operation: "phrase"
          link: "/search/net/phrase/pdf/"
          description: "Шукайте конкретне речення або фразу"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Пошук у ваших бізнес-документах"
    exclude: "PDF"
    description: "GroupDocs.Search підтримує понад 70 форматів файлів, включаючи офісні документи, що забезпечує швидкий і ефективний пошук з можливостями індексації."
    items: 
        # format loop 1
        - name: "Пошук у документі DOCX"
          format: "DOCX"
          link: "/search/net/document/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Пошук у документі PDF"
          format: "PDF"
          link: "/search/net/document/pdf/"
          description: "Формат Adobe Portable Document"
          
        # format loop 3
        - name: "Пошук у документі PPTX"
          format: "PPTX"
          link: "/search/net/document/pptx/"
          description: "Презентація PowerPoint Open XML"

        # format loop 4
        - name: "Пошук у документі TXT"
          format: "TXT"
          link: "/search/net/document/txt/"
          description: "Текстовий документ"
          
        # format loop 5
        - name: "Пошук у документі XLSX"
          format: "XLSX"
          link: "/search/net/document/xlsx/"
          description: "Таблиця Microsoft Excel Open XML"
  

---