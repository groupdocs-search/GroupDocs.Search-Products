---
############################# Static ############################
layout: "landing"
date: 2025-02-03T08:17:12
draft: false

lang: uk
product: "Search"
product_tag: "search"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NET Бібліотека пошуку документів та індексації для PDF, файлів Office та інших"
head_description: "Потужне рішення .NET для пошуку тексту та індексації в документах, таких як PDF, Word, Excel, презентації, електронні листи та вебформати."

############################# Header ############################
title: "Розширений пошук документів та індексація з API .NET"
description: "Покращте програми .NET за допомогою сучасних можливостей пошуку тексту у популярних форматах документів."
words:
  for: "для"

actions:
  main: "Завантажте Nuget безкоштовно"
  main_link: "https://www.nuget.org/packages/GroupDocs.Search"
  alt: "Ліцензування"
  alt_link: "https://purchase.groupdocs.com/pricing/search/net/"
  title: "Розпочніть свою подорож сьогодні!"
  description: "Вивчіть можливості GroupDocs.Search безкоштовно або отримайте ліцензію, щоб розблокувати її повний потенціал."

release:
  title: "Версія {0} випущена"
  notes: "Дивіться, що нового"
  downloads: "Завантаження"

code:
  title: "Пошук тексту в файлах у директорії"
  more: "Більше прикладів"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
  install: "dotnet add package GroupDocs.Search"
  content: |
    ```csharp {style=abap}   
    // Створіть індекс для ваших документів
    Index index = new Index("c:/MyIndex");

    // Додайте документи до індексу для ефективного пошуку
    index.Add("c:/MyDocuments");
    
    // Шукайте конкретні слова або фрази, такі як
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.Search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Огляд GroupDocs.Search"
  description: "Досліджуйте бібліотеку .NET C# для надійного пошуку тексту та індексації."
  features:
    # feature loop
    - title: "Можливості індексації та пошуку .NET"
      content: "Ефективно індексуйте, зберігайте та обробляйте дані документів за допомогою GroupDocs.Search for .NET для максимально точних і швидких операцій пошуку."

    # feature loop
    - title: "Об'єднуйте індекси для покращення швидкості пошуку"
      content: "GroupDocs.Search for .NET дозволяє об'єднувати кілька індексів для оптимізації продуктивності. Зменшіть вплив дельта-індексів, об'єднавши їх в один комплексний індекс для більш плавного пошуку."

    # feature loop
    - title: "Пошук через різні клавіатурні розкладки"
      content: "Просто обробляйте пошукові запити в 88 мовах та 164 клавіатурних розкладках за допомогою інтелектуального розпізнавання GroupDocs.Search for .NET."

    # feature loop
    - title: "Морфологічні пошуки слів"
      content: "GroupDocs.Search for .NET підтримує пошуки за варіаціями слів, такими як однина/множина та різні форми дієслів, налаштовувані для різних мов."

############################# Platforms ############################
platforms:
  enable: true
  title: "Незалежність від платформи"
  description: "GroupDocs.Search for .NET безперешкодно працює на основних операційних системах та менеджерах пакетів."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Підтримувані формати файлів"
  description: |
    Обробляйте широкий спектр форматів файлів з GroupDocs.Search for .NET. [Перегляньте всі підтримувані формати](https://docs.groupdocs.com/search/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Популярні офісні формати
        * **Портативний:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **Текст:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### Медіа формати
        * **Популярні формати зображень:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **Багатосторінкові зображення:** GIF, WEBP, TIFF
        * **Аудіо:** MP3, WAV
        * **Відео:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### Інші
        * **Електронна пошта:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **Веб:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Інші:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "Ключові можливості GroupDocs.Search for .NET"
  description: "Спрощуйте управління документами з розширеними можливостями пошуку в популярних форматах, таких як PDF, DOCX, XLSX, PPTX тощо."

  items:
    # feature loop
    - icon: "document_info"
      title: "Гнучкі параметри пошуку"
      content: "Використовуйте фільтри, такі як діапазони дат і чутливість до регістру, для уточнення вашого пошуку."

    # feature loop
    - icon: "detect"
      title: "Розумна перевірка правопису"
      content: "Шукайте фрази з виправленням помилок, підстановочними знаками та проігнорованими спеціальними символами."

    # feature loop
    - icon: "collect"
      title: "Фільтровані результати пошуку"
      content: "Налаштуйте та фільтруйте результати пошуку за типом документа або критеріями."

    # feature loop
    - icon: "get"
      title: "Імпорт та експорт індексу"
      content: "Імпортуйте дані, змініть налаштування індексації та експортуйте проіндексовані результати."

    # feature loop
    - icon: "remove"
      title: "Виключення нерелевантних даних"
      content: "Оптимізуйте індексацію, пропускаючи певні файли або слова."

    # feature loop
    - icon: "style"
      title: "Витягування URL"
      content: "Перетворюйте текст у форматі HTML на файли та генеруйте посилання для результатів пошуку."

    # feature loop
    - icon: "detect"
      title: "Швидкий пошук"
      content: "Розділіть великі індекси на менші частини для швидшої обробки."

    # feature loop
    - icon: "manipulate"
      title: "Упорядкована обробка даних"
      content: "Індексуйте документи безпосередньо з потоків даних і структур."

    # feature loop
    - icon: "compare"
      title: "Виявлення помилок у написанні"
      content: "Пропонуйте альтернативні слова та відстежуйте вживання для поліпшення точності."

    # feature loop
    - icon: "unreadable_characters"
      title: "Підтримка архівів"
      content: "Індексуйте вкладені ZIP-архіви та отримуйте відомості про файли всередині них."

    # feature loop
    - icon: "hidden_print"
      title: "Ефективна індексація"
      content: "Економте місце на диску за допомогою компактної індексації та обробляйте документи з паролем."

    # feature loop
    - icon: "style"
      title: "Власні синоніми"
      content: "Додайте та керуйте синонімами для індивідуальних результатів пошуку."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Приклади коду"
  description: "Вивчайте потужні можливості GroupDocs.Search for .NET за допомогою практичних прикладів."
  items:
    # code sample loop
    - title: "Підвищте продуктивність за допомогою нечіткого пошуку"
      content: |
        Скористайтеся GroupDocs.Search for .NET для гнучкого та точного контролю вмісту через розширені алгоритми пошуку. [Досліджуйте більше](https://docs.groupdocs.com/search/net/search-results/).
        {{< landing/code title="Як обробити результати пошуку">}}
        ```csharp {style=abap}
        // Створіть індекс
        Index index = new Index("C:/IndexFolder");
        index.Add("C:/DocumentFolder");

        // Налаштуйте параметри пошуку
        SearchOptions options = new SearchOptions();
        options.FuzzySearch.Enabled = true;
        options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3);

        // Шукайте документи, що містять слово 'вода' або фразу 'Lorem ipsum'
        string query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.Search(query, options);
        
        // Обробіть результати пошуку
        Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
        Console.WriteLine("Occurrences: " + document.OccurrenceCount);
        for (int i = 0; i < result.DocumentCount; i++) {
            FoundDocument document = result.GetFoundDocument(i);
            Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
            Console.WriteLine("Occurrences: " + document.OccurrenceCount);
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Розширений пошук з використанням регулярних виразів"
      content: |
        GroupDocs.Search for .NET підтримує регулярні вирази для точних пошуків. [Дізнайтеся про розширені техніки](https://docs.groupdocs.com/search/net/regular-expression-search/).
        {{< landing/code title="Як шукати за допомогою регулярних виразів">}}
        ```csharp {style=abap}   
        // Створіть індекс
        Index index = new Index("c:/IndexFolder");
        index.Add("c:/DocumentFolder");
 
        // Шукайте фразу у текстовій формі

        // Перший символ каретки на початку вказує, що це запит пошуку регулярного виразу
        string query = "^^(.)\\1{1,}";
        // Шукайте дві або більше ідентичні літери на початку слова
        SearchResult result = index.Search(query);
 
        ```
        {{< /landing/code >}}

---
