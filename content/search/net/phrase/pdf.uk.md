
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: uk
format: Pdf
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Пошук фраз у PDF з використанням .NET"
head_description: "GroupDocs.Search for .NET покращує застосунки C# потужними можливостями пошуку фраз для вмісту документів."

############################# Header ############################
title: "Пошук фраз у документах" 
description: "Швидко знаходьте конкретні фрази з GroupDocs.Search for .NET. Інтегруйте ефективну функціональність пошуку в ваші застосунки .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Завантажити"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Особливості GroupDocs.Search"
    link: "/search/net/"
    link_title: "Дізнатися більше"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) — потужна бібліотека для індексації та пошуку тексту в документах. Вона підтримує більше 70 форматів файлів, включаючи PDF, документи Word, таблиці Excel, зображення та ZIP-файли, забезпечуючи швидкі та точні результати пошуку.

############################# Steps ############################
steps:
    enable: true
    title: "Як шукати фрази в документах PDF"
    content: |
      [GroupDocs.Search](/search/net/) спрощує пошук у документах PDF. Використовуйте різноманітні опції для уточнення результатів пошуку в застосунках .NET.
      
      1. Налаштуйте папку для пошукового індексу.
      2. Вкажіть папку, що містить файли PDF.
      3. Налаштуйте параметри пошуку.
      4. Отримайте та обробіть результати пошуку.
   
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
        // Шлях для зберігання пошукового індексу
        Index index = new Index("c:/MyIndex");

        // Папка, що містить документи
        index.Add("c:/MyDocuments");

        // Налаштувати параметри пошуку
        SearchQuery word1 = SearchQuery.CreateWordQuery("lorem");
        SearchQuery word2 = SearchQuery.CreateWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.CreateWordQuery("dolor");

        SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, word2, word3);

        // Виконати пошук
        SearchResult result = index.Search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Відкрийте для себе пошукову систему документів .NET"
  description: "GroupDocs.Search for .NET дозволяє здійснювати пошук фраз у понад 70 форматах файлів. Швидко знаходьте і керуйте даними з розширеними можливостями пошуку."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Ключові особливості GroupDocs.Search"
  features:
    # feature loop
    - title: "Пошук фраз"
      content: "Шукайте точні фрази в ділових документах, включаючи PDF, файли Word, презентації та електронні таблиці. Використовуйте підстановочні знаки та інші параметри, якщо точна фраза невідома."

    # feature loop
    - title: "Ефективна індексація даних"
      content: "Створюйте та повторно використовуйте пошукові індекси для прискорення пошуку документів. Індексація структуризує дані ефективно, роблячи пошук фраз швидшим."

    # feature loop
    - title: "Підтримка багатьох мов"
      content: "Шукайте документи більше ніж 80 мовами. Підтримує різні розкладки клавіатури та морфологічні форми слів для підвищення точності пошуку."

    # feature loop
    - title: "Гнучкі опції пошуку"
      content: "Налаштуйте пошук за допомогою таких функцій, як чутливість до регістру, нечутливий та гомофонний пошук, фільтрація документів і багато іншого."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Використання розширених технік пошуку"
      content: |
        Дізнайтеся, як створити запити для пошуку в PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Вкажіть папку для пошукового індексу
          Index index = new Index("c:/MyIndex");
              
          // Встановіть шлях до документів для пошуку
          index.Add("c:/MyDocuments");

          // Створіть запит для конкретної фрази
          SearchQuery word1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.CreateWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.CreateWordQuery("dolor");

          SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, wildcard, word2);

          // Отримайте результати пошуку
          SearchResult result = index.Search(query);
          
          // Обробіть та використайте результати
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
            link: "/examples/search/formats/searchphrase.pdf"
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
    title: "Розширені функції"
    exclude: "phrase"
    description: "Використовуйте потужні та ефективні функціональності пошуку."
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
    title: "Пошук фраз у ділових документах"
    exclude: "PDF"
    description: "GroupDocs.Search підтримує пошук у понад 70 форматах документів. Використовуйте розширені опції та індексацію для оптимізації вашого процесу пошуку."
    items: 
        # format loop 1
        - name: "Пошук фрази у DOCX"
          format: "DOCX"
          link: "/search/net/phrase/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Пошук фрази у PDF"
          format: "PDF"
          link: "/search/net/phrase/pdf/"
          description: "Формат Adobe Portable Document"
          
        # format loop 3
        - name: "Пошук фрази у PPTX"
          format: "PPTX"
          link: "/search/net/phrase/pptx/"
          description: "Презентація PowerPoint Open XML"

        # format loop 4
        - name: "Пошук фрази у TXT"
          format: "TXT"
          link: "/search/net/phrase/txt/"
          description: "Текстовий документ"
          
        # format loop 5
        - name: "Пошук фрази у XLSX"
          format: "XLSX"
          link: "/search/net/phrase/xlsx/"
          description: "Таблиця Microsoft Excel Open XML"
  

---