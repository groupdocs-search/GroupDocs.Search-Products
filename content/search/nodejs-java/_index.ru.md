---
############################# Static ############################
layout: "landing"
date: 2024-07-03T19:47:25
draft: false

lang: ru
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js Библиотека текстового поиска и индексирования для документов, PDF, Office и Интернета"
head_description: "Расширенное решение для текстового поиска для приложений Node.js для поиска, индексирования и сбора данных из документов: PDF, Word, Excel, презентаций, файлов электронной почты и веб-форматов."

############################# Header ############################
title: "Поиск и индексирование документов с использованием API Node.js"
description: "Улучшите приложения Node.js, внедрив текстовый поиск во всех популярных форматах документов."
words:
  for: "для"

actions:
  main: "Бесплатная загрузка НПМ"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "Лицензирование"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "Готовы начать?"
  description: "Попробуйте функции GroupDocs.Search бесплатно или запросите лицензию."

release:
  title: "Версия {0} выпущена"
  notes: "Посмотрите, что нового"
  downloads: "Загрузки"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "Искать в папке с помощью JavaScript"
  more: "Больше примеров"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    // Создание индекса
    var index = new Index("c:\\MyIndex");

    // Добавление документов в индекс
    index.addToIndex("c:\\MyDocuments");
    
    // Поиск различных слов, таких как
    // 'affect', 'effect', 'principles', 'principally'
    var results = index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search с первого взгляда"
  description: "Библиотека Node.js JavaScript для текстового поиска"
  features:
    # feature loop
    - title: "Node.js Операции индексирования и поиска"
      content: "Индексирование в GroupDocs.Search for Node.js via Java собирает, хранит и анализирует данные для точных и эффективных операций поиска. Эти индексы часто используются для выполнения поиска."

    # feature loop
    - title: "Объединение нескольких индексов для повышения эффективности поиска"
      content: "API GroupDocs.Search for Node.js via Java позволяет объединить несколько индексов в один. Частые модификации создают несколько дельта-индексов, что может замедлить производительность поиска. Наше решение объединяет эти дельта-индексы в общий индекс, содержащий всю информацию из объединенных дельта-индексов, что значительно повышает эффективность поиска, сохраняя при этом дельта-индексы неизменными. Для точной настройки этого процесса можно настроить различные функции."

    # feature loop
    - title: "Распознавание поисковых запросов из разных раскладок клавиатуры"
      content: "GroupDocs.Search for Node.js via Java распознает поисковые запросы, которые не соответствуют раскладке клавиатуры. На данный момент поддерживается 88 языков и 164 различных раскладки клавиатуры."

    # feature loop
    - title: "Поиск с использованием морфологических словоформ"
      content: "С помощью GroupDocs.Search for Node.js via Java вы можете искать различные формы слов, например существительные в единственном и множественном числе, а также все формы глагола. Английский и неанглийские языки можно настроить для определенных словоформ."

############################# Platforms ############################
platforms:
  enable: true
  title: "Независимость от платформы"
  description: "GroupDocs.Search for Node.js via Java поддерживает все популярные операционные системы и менеджеры пакетов."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Поддерживаемые форматы файлов"
  description: |
    GroupDocs.Search for Node.js via Java позволяет обрабатывать широкий спектр форматов файлов. [Изучите полный список](https://docs.groupdocs.com/search/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Популярные форматы офиса
        * **Портативный:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **Текст:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### Медиа-форматы
        * **Популярные форматы изображений:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **Многостраничные изображения:** GIF, WEBP, TIFF
        * **Аудио:** MP3, WAV
        * **видео:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### Другой
        * **Электронная почта:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **Интернет:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Другие:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "Функции GroupDocs.Search for Node.js via Java"
  description: "Управляйте содержимым деловых документов с помощью нашей усовершенствованной поисковой системы, поддерживающей популярные форматы файлов, включая PDF, DOCX, XLSX, PPTX и другие."

  items:
    # feature loop
    - icon: "document_info"
      title: "Гибкие параметры"
      content: "Используйте диапазон дат и чувствительность к регистру в качестве параметров поиска"

    # feature loop
    - icon: "detect"
      title: "Проверка орфографии Поиск"
      content: "Используйте поисковые фразы с проверкой орфографии и подстановочными знаками и пропускайте специальные символы в запросах"

    # feature loop
    - icon: "collect"
      title: "Фильтрация результатов"
      content: "Настройка фильтрации документов в результатах поиска"

    # feature loop
    - icon: "get"
      title: "Импорт Экспорт"
      content: "Выполните импорт или используйте список для изменения символов во время индексирования и экспорта в файл."

    # feature loop
    - icon: "remove"
      title: "Пропустить ненужные данные"
      content: "Выборочно пропустить индексирование определенных файлов и пропустить определенные слова для ускорения индексации"

    # feature loop
    - icon: "style"
      title: "Обработка URL-адресов"
      content: "Извлеките текст в формате HTML в файл и сгенерируйте URL-адрес для навигации по результатам поиска в HTML"

    # feature loop
    - icon: "detect"
      title: "Быстрый поиск"
      content: "Разделите поиск на более мелкие фрагменты для быстрого поиска в больших индексах"

    # feature loop
    - icon: "manipulate"
      title: "Потоковая обработка"
      content: "Индексируйте документы из потоков и структур данных"

    # feature loop
    - icon: "compare"
      title: "Обработка орфографических ошибок"
      content: "Включите точное количество вхождений для каждого найденного слова, чтобы предлагать альтернативные варианты слов в случае орфографической ошибки."

    # feature loop
    - icon: "unreadable_characters"
      title: "Поддержка архива"
      content: "Индексируйте ZIP-архивы внутри других ZIP-архивов и получайте список проиндексированных файлов в архиве"

    # feature loop
    - icon: "hidden_print"
      title: "Экономия дискового пространства"
      content: "Экономьте место с помощью компактного индексирования и индексирования документов, защищенных паролем"

    # feature loop
    - icon: "style"
      title: "Пользовательские синонимы"
      content: "Добавить английские синонимы в словарь синонимов по умолчанию"

############################# Code samples ############################
code_samples:
  enable: true
  title: "Примеры кода"
  description: "Изучите функциональные возможности GroupDocs.Search for Node.js via Java на примерах."
  items:
    # code sample loop
    - title: "Используйте нечеткий поиск для повышения производительности"
      content: |
        Воспользуйтесь гибкой функциональностью GroupDocs.Search for Node.js via Java, позволяющей улучшить контроль над содержимым документов с помощью сложных алгоритмов поиска. [Подробнее](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="Как обработать результат поиска">}}
        ```javascript {style=abap}
        // Создать индекс
        var index = new Index("C:\\IndexFolder");
        index.add("C:\\DocumentFolder");

        // Настройка параметров поиска
        var options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Поиск документов, содержащих слово «вода» или фразу «Lorem ipsum».
        var query = "water OR \"Lorem ipsum\"";
        var result = index.search(query, options);
        
        // Обработать результат поиска
        console.log("Documents: " + result.getDocumentCount());
        console.log("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            console.log('Document: ${document.getDocumentInfo().getFilePath()}');
            console.log('Occurrences: ${document.getOccurrenceCount()}');
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Регулярные выражения доступны для сценариев расширенного поиска."
      content: |
        GroupDocs.Search for Node.js via Java позволяет нам использовать регулярные выражения для сужения результатов поиска. [Погрузитесь в методы расширенного поиска](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="Как искать с помощью регулярных выражений">}}
        ```javascript {style=abap}   
        // Создать индекс
        var index = new Index("C:\\IndexFolder");
        index.add("C:\\DocumentFolder");
 
        // Поиск фразы в текстовой форме

        // Первый символ каретки в начале указывает, что это поисковый запрос по регулярному выражению.
        var query = "^^(.)\\1{1,}";
        // Поиск двух и более одинаковых символов в начале слова
        var result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
