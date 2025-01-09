---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
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
head_title: "Библиотека текстового поиска и индексирования Node.js для документов, PDF, офисных и веб"
head_description: "Расширенное решение для текстового поиска для приложений Node.js для поиска, индексирования и сбора данных из документов: PDF, Word, Excel, презентации, электронной почты и веб-форматов."

############################# Header ############################
title: "Поиск и индексирование документов с помощью API Node.js"
description: "Улучшите приложения Node.js, реализуя текстовый поиск во всех популярных форматах документов."
words:
  for: "для"

actions:
  main: "Бесплатное скачивание NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "Лицензирование"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "Начните ваше путешествие сегодня!"
  description: "Изучите возможности GroupDocs.Search бесплатно или получите лицензию, чтобы разблокировать его полный потенциал."

release:
  title: "Версия {0} выпущена"
  notes: "Смотрите, что нового"
  downloads: "Скачивания"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "Выполнение текстового поиска в папке с JavaScript"
  more: "Больше примеров"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    const searchLib = require('@groupdocs/groupdocs.search');

    // Создайте индекс для ваших документов
    const index = new searchLib.Index('c:/MyIndex');

    // Добавьте документы в индекс для эффективного поиска
    index.add('c:/MyDocuments');
    
    // Ищите конкретные слова или фразы, такие как
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Обзор GroupDocs.Search"
  description: "Библиотека Node.js JavaScript для текстового поиска."
  features:
    # feature loop
    - title: "Индексирование и операции поиска Node.js"
      content: "Индексирование в GroupDocs.Search for Node.js via Java собирает, хранит и обрабатывает данные для точных и эффективных операций поиска. Эти индексы часто используются для выполнения поиска."

    # feature loop
    - title: "Объединение нескольких индексов для повышения эффективности поиска"
      content: "GroupDocs.Search for Node.js via Java API позволяет объединять несколько индексов в один. Частые изменения создают несколько дельта-индексов, что может замедлить работу поиска. Наше решение объединяет эти дельта-индексы в общий индекс, содержащий всю информацию из объединенных дельта-индексов, значительно увеличивая эффективность поиска и сохраняя дельта-индексы неизменными. Различные функции могут быть настроены для точной настройки данного процесса."

    # feature loop
    - title: "Распознавание запросов поиска с разных раскладок клавиатуры"
      content: "GroupDocs.Search for Node.js via Java распознает запросы поиска, которые не соответствуют раскладке клавиатуры. В настоящее время поддерживаются 88 языков и 164 разные раскладки клавиатуры."

    # feature loop
    - title: "Поиск с использованием морфологических форм слов"
      content: "С GroupDocs.Search for Node.js via Java вы можете искать разные формы слов, такие как единственное и множественное число существительных, или все формы глагола. Английский и неанглийские языки могут быть настроены для определенных форм слов."

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
    GroupDocs.Search for Node.js via Java позволяет обрабатывать широкий спектр форматов файлов. [Изучите полный список](https://docs.groupdocs.com/search/nodejs-java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Популярные офисные форматы
        * **Портативный:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **Текст:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### Медийные форматы
        * **Популярные форматы изображений:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **Многостраничные изображения:** GIF, WEBP, TIFF
        * **Аудио:** MP3, WAV
        * **Видео:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### Другие
        * **Электронная почта:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **Веб:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Другие:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "Функции GroupDocs.Search for Node.js via Java"
  description: "Контролируйте содержимое бизнес-документов с помощью нашего продвинутого поискового движка, поддерживающего популярные форматы файлов, включая PDF, DOCX, XLSX, PPTX и другие."

  items:
    # feature loop
    - icon: "document_info"
      title: "Гибкие параметры"
      content: "Используйте диапазон даты и чувствительность к регистру в качестве параметров поиска."

    # feature loop
    - icon: "detect"
      title: "Поиск с проверкой правописания"
      content: "Используйте поисковые фразы с проверкой правописания и подстановочными знаками, пропуская специальные символы в запросах."

    # feature loop
    - icon: "collect"
      title: "Фильтрация результатов"
      content: "Настройте фильтрацию документов в результатах поиска."

    # feature loop
    - icon: "get"
      title: "Импорт и экспорт"
      content: "Выполните импорт или используйте список для изменения символов во время индексирования и экспорта в файл."

    # feature loop
    - icon: "remove"
      title: "Пропуск ненужных данных"
      content: "Избирательно избегайте индексирования для конкретных файлов и пропускайте конкретные слова, чтобы индексировать быстрее."

    # feature loop
    - icon: "style"
      title: "Обработка URL"
      content: "Извлеките текст, отформатированный HTML, в файл и создайте URL для навигации по результатам поиска в HTML."

    # feature loop
    - icon: "detect"
      title: "Быстрый поиск"
      content: "Разделите поиск на меньшие части для быстрого поиска в больших индексах."

    # feature loop
    - icon: "manipulate"
      title: "Обработка потоков"
      content: "Индексируйте документы из потоков и структур данных."

    # feature loop
    - icon: "compare"
      title: "Обработка опечаток"
      content: "Обеспечьте точное количество вхождений для каждого найденного слова, предлагая альтернативные слова в случае опечаток."

    # feature loop
    - icon: "unreadable_characters"
      title: "Поддержка архивов"
      content: "Индексируйте ZIP-архивы внутри других ZIP-архивов и извлекайте список индексированных файлов в архиве."

    # feature loop
    - icon: "hidden_print"
      title: "Экономия дискового пространства"
      content: "Экономьте пространство с помощью компактного индексирования и индексируйте файлы, защищенные паролем."

    # feature loop
    - icon: "style"
      title: "Настраиваемые синонимы"
      content: "Добавляйте английские синонимы в словарь синонимов по умолчанию."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Примеры кода"
  description: "Изучите функциональные возможности GroupDocs.Search for Node.js via Java с примерами."
  items:
    # code sample loop
    - title: "Используйте 'нечеткий' поиск для повышения продуктивности"
      content: |
        Наслаждайтесь гибкой функциональностью GroupDocs.Search for Node.js via Java для повышения контроля над содержимым документов с помощью сложных поисковых алгоритмов. [Узнайте больше](https://docs.groupdocs.com/search/nodejs-java/search-results/).
        {{< landing/code title="Как обработать результат поиска">}}
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search');

        // Создайте индекс
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // Настройте параметры поиска
        const options = new searchLib.SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Ищите документы, содержащие слово 'вода' или фразу 'Lorem ipsum'
        const query = 'water OR "Lorem ipsum"';
        const result = index.search(query, options);
        
        // Обработайте результат поиска
        console.log('Documents: ' + result.getDocumentCount());
        console.log('Total occurrences: ' + result.getOccurrenceCount());
        for (let i = 0; i < result.getDocumentCount(); i++) {
            const document = result.getFoundDocument(i);
            console.log('Document: ' + document.getDocumentInfo().getFilePath());
            console.log('Occurrences:  + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Регулярные выражения доступны для расширенных сценариев поиска"
      content: |
        GroupDocs.Search for Node.js via Java позволяет использовать регулярные выражения, чтобы уточнить результат поиска. [Погрузитесь в продвинутые техники поиска](https://docs.groupdocs.com/search/nodejs-java/regular-expression-search/).
        {{< landing/code title="Как искать с использованием регулярных выражений">}}
        ```javascript {style=abap}   
        const searchLib = require('@groupdocs/groupdocs.search');

        // Создайте индекс
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // Ищите фразу в текстовом формате

        // Первый символ ^ в начале указывает, что это поисковый запрос с использованием регулярного выражения
        const query = '^^(.)\\1{1,}';
        // Ищите два или более одинаковых символа в начале слова
        const result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
