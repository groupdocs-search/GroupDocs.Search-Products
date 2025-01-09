---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: uk
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

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
head_title: "Рішення для пошуку та індексації документів Java для PDF, файлів Office та веб-контенту"
head_description: "Потужний пошук тексту та індексація для додатків Java. Зручно шукайте та організовуйте дані у PDF, Word, Excel, презентаціях, електронних листах та веб-форматах."

############################# Header ############################
title: "Ефективний пошук документів та індексація за допомогою API Java"
description: "Надайте додаткам Java потужні функції пошуку тексту в усіх популярних форматах документів."
words:
  for: "для"

actions:
  main: "Завантажте Maven безкоштовно"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-search/"
  alt: "Ліцензування"
  alt_link: "https://purchase.groupdocs.com/pricing/search/java/"
  title: "Розпочніть свою подорож сьогодні!"
  description: "Вивчіть можливості GroupDocs.Search безкоштовно або отримайте ліцензію, щоб розблокувати її повний потенціал."

release:
  title: "Версія {0} випущена"
  notes: "Дивіться, що нового"
  downloads: "Завантаження"

code:
  title: "Знайдіть текст у файлах за допомогою Java"
  more: "Більше прикладів"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-search</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Створіть індекс для ваших документів
    Index index = new Index("c:/MyIndex");

    // Додайте документи до індексу для ефективного пошуку
    index.add("c:/MyDocuments");
    
    // Шукайте конкретні слова або фрази, такі як
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Огляд GroupDocs.Search"
  description: "Досліджуйте потужні можливості пошуку тексту бібліотеки Java Java."
  features:
    # feature loop
    - title: "Операції індексації та пошуку в Java"
      content: "З GroupDocs.Search for Java ви можете ефективно збирати, зберігати та аналізувати дані, щоб створити детальні індекси для швидших і точніших пошуків."

    # feature loop
    - title: "Оптимізуйте пошук шляхом злиття індексів"
      content: "Легко об'єднуйте кілька індексів за допомогою GroupDocs.Search for Java для спрощення пошуку. Зменшіть вплив менших дельта-індексів, об'єднавши їх в один індекс високої продуктивності."

    # feature loop
    - title: "Підтримка багатомовних клавіатурних розкладок"
      content: "Шукайте різними мовами та клавіатурними розкладками за допомогою GroupDocs.Search for Java. Він підтримує 88 мов та 164 конфігурації клавіатур для неперевершеної універсальності."

    # feature loop
    - title: "Морфологічні можливості пошуку"
      content: "Знаходьте різні форми слів, такі як однина/множина і варіації дієслів, використовуючи GroupDocs.Search for Java. Налаштуйте параметри пошуку для англійської та інших мов."

############################# Platforms ############################
platforms:
  enable: true
  title: "Незалежність від платформи"
  description: "GroupDocs.Search for Java сумісний з основними операційними системами та менеджерами пакетів."
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Підтримувані формати файлів"
  description: |
    Працюйте з широким спектром форматів файлів за допомогою GroupDocs.Search for Java. [Ознайомтесь із повним списком](https://docs.groupdocs.com/search/java/supported-document-formats/).
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
  title: "Можливості GroupDocs.Search for Java"
  description: "Ефективно управляйте вмістом документів за допомогою розширених функцій пошуку, що підтримують формати, такі як PDF, DOCX, XLSX, PPTX тощо."

  items:
    # feature loop
    - icon: "document_info"
      title: "Налаштовувані параметри пошуку"
      content: "Уточнюйте пошуки, використовуючи діапазони дат і фільтри чутливості до регістру."

    # feature loop
    - icon: "detect"
      title: "Покращена перевірка правопису"
      content: "Ефективно шукайте з перевіркою правопису, підстановочними знаками та ігноруючи спеціальні символи."

    # feature loop
    - icon: "collect"
      title: "Фільтровані результати пошуку"
      content: "Застосуйте фільтри для зосередження результатів пошуку на основі конкретних типів документів або критеріїв."

    # feature loop
    - icon: "get"
      title: "Імпорт та експорт даних індексу"
      content: "Легко імпортуйте дані для індексації або експортуйте результати у файли для подальшого використання."

    # feature loop
    - icon: "remove"
      title: "Пропустити непотрібні файли"
      content: "Оптимізуйте індексацію, виключаючи певні файли або слова."

    # feature loop
    - icon: "style"
      title: "Обробка HTML та URL"
      content: "Отримуйте HTML-контент у файли та генеруйте URL для навігації через результати пошуку."

    # feature loop
    - icon: "detect"
      title: "Швидкий пошук у великих індексах"
      content: "Прискорте пошукові операції, розділивши великі індекси на керовані частини."

    # feature loop
    - icon: "manipulate"
      title: "Індексація на основі потоків"
      content: "Індексуйте дані безпосередньо з потоків або структур даних."

    # feature loop
    - icon: "compare"
      title: "Обробка з помилками в запитах"
      content: "Виявляйте помилки в написанні та пропонуйте альтернативні слова для покращення точності пошуку."

    # feature loop
    - icon: "unreadable_characters"
      title: "Комплексна підтримка архівів"
      content: "Індексуйте вкладені архіви та отримуйте детальні списки файлів у ZIP-файлах."

    # feature loop
    - icon: "hidden_print"
      title: "Економія місця під час індексації"
      content: "Компактні індекси для економії місця на диску та обробки документів з паролем."

    # feature loop
    - icon: "style"
      title: "Підтримка власних синонімів"
      content: "Розширте словник синонімів для вдосконалення точності пошуку з індивідуальними опціями."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Приклади коду"
  description: "Спробуйте функції GroupDocs.Search for Java за допомогою цих кодових прикладів."
  items:
    # code sample loop
    - title: "Підвищте точність пошуку за допомогою нечіткого співпадіння"
      content: |
        Досліджуйте гнучкість GroupDocs.Search for Java для управління вмістом з використанням вдосконалених можливостей нечіткого пошуку. [Дізнайтеся більше](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="Як обробити результати пошуку">}}
        ```java {style=abap}
        // Створіть індекс
        Index index = new Index("C:/IndexFolder");
        index.add("C:/DocumentFolder");

        // Налаштуйте параметри пошуку
        SearchOptions options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Шукайте документи, що містять слово 'вода' або фразу 'Lorem ipsum'
        String query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.search(query, options);
        
        // Обробіть результати пошуку
        System.out.println("Documents: " + result.getDocumentCount());
        System.out.println("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            System.out.println("Document: " + document.getDocumentInfo().getFilePath());
            System.out.println("Occurrences " + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Уточніть результати за допомогою регулярних виразів"
      content: |
        Використовуйте регулярні вирази в GroupDocs.Search for Java для створення точних і детальних результатів пошуку. [Відкрийте для себе розширені техніки](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="Як шукати за допомогою регулярних виразів">}}
        ```java {style=abap}   
        // Створіть індекс
        Index index = new Index("C:/IndexFolder");
        index.add("c:/DocumentFolder");
 
        // Шукайте фразу у текстовій формі

        // Перший символ каретки на початку вказує, що це запит пошуку регулярного виразу
        String query = "^^(.)\\1{1,}";
        // Шукайте дві або більше ідентичні літери на початку слова
        SearchResult result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
