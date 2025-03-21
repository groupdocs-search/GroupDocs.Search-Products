
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:46
draft: false
lang: uk
format: Docx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Пошук DOCX в .NET за допомогою булевих операторів"
head_description: "API GroupDocs.Search for .NET дозволяє розробникам C# здійснювати пошук вмісту документів за допомогою булевих операторів, таких як AND, OR, та NOT."

############################# Header ############################
title: "Булева логіка текстового пошуку" 
description: "GroupDocs.Search for .NET спрощує створення складних запитів пошуку, використовуючи булеві оператори (AND, OR, NOT) у ваших додатках .NET."
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
       [GroupDocs.Search for .NET](/search/net/) - це комплексна бібліотека для пошуку та індексації тексту в документах. Вона підтримує понад 70 форматів файлів, таких як PDF, Word, PowerPoint, Excel, зображення та ZIP-файли, що дозволяє ефективно обробляти великі обсяги інформації.

############################# Steps ############################
steps:
    enable: true
    title: "Як шукати вміст документів DOCX за допомогою булевої логіки"
    content: |
      [GroupDocs.Search](/search/net/) робить пошук вмісту документів DOCX зрозумілим. Він надає умови пошуку за булевою логікою для уточнення результатів у додатках .NET.
      
      1. Вкажіть папку для зберігання індексу пошуку.
      2. Оберіть папку, що містить файли DOCX.
      3. Виконайте пошук та отримайте результати.
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
        // Вкажіть шлях до папки з індексом
        Index index = new Index("c:/MyIndex");

        // Вкажіть папку, що містить документи для пошуку
        index.Add("c:/MyDocuments");

        // Виконайте пошук за допомогою складного запиту
        SearchResult result = index.Search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Досліджуйте розширені можливості для пошуку та індексації документів"
  description: "Бібліотека GroupDocs.Search for .NET спрощує пошук тексту та індексацію для більш ніж 70 форматів файлів. Легко знаходьте та управляйте інформацією за допомогою розширених інструментів пошуку."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Основні функції GroupDocs.Search"
  features:
    # feature loop
    - title: "Потужний текстовий пошук"
      content: "Шукайте текст в різних типах файлів, включаючи PDF, документи Word, презентації PowerPoint і електронні таблиці. Використовуйте функції, такі як точні відповідності, нечіткий пошук та підстановочні знаки для уточнення результатів."

    # feature loop
    - title: "Індексація великих наборів даних"
      content: "Створюйте та підтримуйте індекси для швидших пошуків. Індексація організовує дані, полегшуючи пошук великих колекцій документів."

    # feature loop
    - title: "Підтримка кількох мов"
      content: "Шукайте документи більш ніж 80 мовами з підтримкою різних розкладок клавіатури та морфологічних форм слів для покращення точності пошуку."

    # feature loop
    - title: "Налаштовувані параметри пошуку"
      content: "Відрегулюйте налаштування пошуку за допомогою таких функцій, як чутливість до регістру, фільтри за діапазоном дат та можливість виключення певних слів або даних під час індексації."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Використання розширених булевих запитів пошуку"
      content: |
        Цей приклад демонструє, як застосувати булеві запити для пошуку документів DOCX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Встановіть папку для індексу пошуку
          Index index = new Index("c:/MyIndex");
              
          // Вкажіть шлях до документів, що підлягають пошуку
          index.Add("c:/MyDocuments");

          // Створіть запит пошуку за допомогою булевої логіки
          SearchQuery wordQuery1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.CreateWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.CreateAndQuery(wordQuery1, wordQuery2);

          // Отримайте результати пошуку
          SearchResult result = index.Search(booleanQuery);
          
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
            link: "/examples/search/formats/searchboolean.docx"
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
    title: "Відкрийте для себе ключові особливості"
    exclude: "boolean"
    description: "Досліджуйте розширені та ефективні функціональні можливості пошуку."
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
    title: "Пошук у популярних форматах документів"
    exclude: "DOCX"
    description: "GroupDocs.Search підтримує понад 70 форматів файлів. Налаштуйте правила пошуку та використовуйте індексацію для економії часу і зусиль."
    items: 
        # format loop 1
        - name: "Логічний пошук у DOCX"
          format: "DOCX"
          link: "/search/net/boolean/docx/"
          description: "Документ Microsoft Word Open XML"
          
        # format loop 2
        - name: "Логічний пошук у PDF"
          format: "PDF"
          link: "/search/net/boolean/pdf/"
          description: "Формат Adobe Portable Document"
          
        # format loop 3
        - name: "Логічний пошук у PPTX"
          format: "PPTX"
          link: "/search/net/boolean/pptx/"
          description: "Презентація PowerPoint Open XML"

        # format loop 4
        - name: "Логічний пошук у TXT"
          format: "TXT"
          link: "/search/net/boolean/txt/"
          description: "Текстовий документ"
          
        # format loop 5
        - name: "Логічний пошук у XLSX"
          format: "XLSX"
          link: "/search/net/boolean/xlsx/"
          description: "Таблиця Microsoft Excel Open XML"
  

---