---
############################# Static ############################
layout: "landing"
date: 2025-02-03T08:17:12
draft: false

lang: ru
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
head_title: "Библиотека поиска и индексирования документов .NET для PDF, офисных файлов и других форматов"
head_description: "Мощное решение .NET для поиска текста и индексирования в документах, таких как PDF, Word, Excel, презентации, электронные письма и веб-форматы."

############################# Header ############################
title: "Расширенный поиск и индексирование документов с API .NET"
description: "Улучшите приложения .NET с помощью передовых возможностей текстового поиска в популярных форматах документов."
words:
  for: "для"

actions:
  main: "Скачайте Nuget бесплатно"
  main_link: "https://www.nuget.org/packages/GroupDocs.Search"
  alt: "Лицензирование"
  alt_link: "https://purchase.groupdocs.com/pricing/search/net/"
  title: "Начните ваше путешествие сегодня!"
  description: "Изучите возможности GroupDocs.Search бесплатно или получите лицензию, чтобы разблокировать его полный потенциал."

release:
  title: "Версия {0} выпущена"
  notes: "Смотрите, что нового"
  downloads: "Скачивания"

code:
  title: "Поиск текста в файлах директории"
  more: "Больше примеров"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
  install: "dotnet add package GroupDocs.Search"
  content: |
    ```csharp {style=abap}   
    // Создайте индекс для ваших документов
    Index index = new Index("c:/MyIndex");

    // Добавьте документы в индекс для эффективного поиска
    index.Add("c:/MyDocuments");
    
    // Ищите конкретные слова или фразы, такие как
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.Search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Обзор GroupDocs.Search"
  description: "Изучите библиотеку .NET C# для надежного текстового поиска и индексирования."
  features:
    # feature loop
    - title: "Функции индексирования и поиска .NET"
      content: "Эффективно индексируйте, храните и обрабатывайте данные документов с помощью GroupDocs.Search for .NET для очень точных и быстрых операций поиска."

    # feature loop
    - title: "Объединение индексов для повышения скорости поиска"
      content: "GroupDocs.Search for .NET позволяет объединять несколько индексов для оптимизации работы. Уменьшите влияние дельта-индексов, комбинируя их в обширный индекс для более гладкого поиска."

    # feature loop
    - title: "Поиск по различным раскладкам клавиатуры"
      content: "Легко обрабатывайте запросы поиска на 88 языках и 164 раскладках клавиатуры с помощью интеллектуального распознавания GroupDocs.Search for .NET."

    # feature loop
    - title: "Морфологический поиск слов"
      content: "GroupDocs.Search for .NET поддерживает поиск вариантов слов, таких как единственное/множественное число существительных и разные формы глаголов, настраиваемые для различных языков."

############################# Platforms ############################
platforms:
  enable: true
  title: "Независимость от платформы"
  description: "GroupDocs.Search for .NET работает без проблем на основных операционных системах и менеджерах пакетов."
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
  title: "Поддерживаемые форматы файлов"
  description: |
    Обрабатывайте широкий спектр форматов файлов с помощью GroupDocs.Search for .NET. [Смотрите все поддерживаемые форматы](https://docs.groupdocs.com/search/net/supported-document-formats/).
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
  title: "Ключевые функции GroupDocs.Search for .NET"
  description: "Упорядочите управление документами с помощью расширенных возможностей поиска в популярных форматах, таких как PDF, DOCX, XLSX, PPTX и других."

  items:
    # feature loop
    - icon: "document_info"
      title: "Гибкие параметры поиска"
      content: "Используйте фильтры, такие как диапазоны дат и чувствительность к регистру для уточнения поиска."

    # feature loop
    - icon: "detect"
      title: "Умная проверка правописания"
      content: "Ищите фразы с исправлением правописания, подстановочными знаками и игнорированием специальных символов."

    # feature loop
    - icon: "collect"
      title: "Фильтрация результатов поиска"
      content: "Настройте и фильтруйте результаты поиска по типу документа или критериям."

    # feature loop
    - icon: "get"
      title: "Импорт и экспорт индексов"
      content: "Импортируйте данные, изменяйте параметры индексирования и экспортируйте индексированные результаты."

    # feature loop
    - icon: "remove"
      title: "Исключение нерелевантных данных"
      content: "Оптимизируйте индексирование, пропуская определенные файлы или слова."

    # feature loop
    - icon: "style"
      title: "Извлечение URL"
      content: "Преобразуйте текст в формате HTML в файлы и создавайте ссылки для результатов поиска."

    # feature loop
    - icon: "detect"
      title: "Поиск высокой скорости"
      content: "Разделите большие индексы на более мелкие части для более быстрой обработки."

    # feature loop
    - icon: "manipulate"
      title: "Упрощенная обработка данных"
      content: "Индексируйте документы непосредственно из потоков данных и структур."

    # feature loop
    - icon: "compare"
      title: "Обнаружение опечаток"
      content: "Предлагайте альтернативные слова и отслеживайте их появление для улучшения точности."

    # feature loop
    - icon: "unreadable_characters"
      title: "Поддержка архивов"
      content: "Индексируйте вложенные ZIP-архивы и извлекайте детали файлов внутри них."

    # feature loop
    - icon: "hidden_print"
      title: "Эффективное индексирование"
      content: "Экономьте место на диске с помощью компактного индексирования и обрабатывайте зашифрованные документы."

    # feature loop
    - icon: "style"
      title: "Настраиваемые синонимы"
      content: "Добавляйте и управляйте синонимами для адаптированных результатов поиска."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Примеры кода"
  description: "Откройте для себя мощные возможности GroupDocs.Search for .NET с практическими примерами."
  items:
    # code sample loop
    - title: "Повышение продуктивности с помощью нечеткого поиска"
      content: |
        Используйте GroupDocs.Search for .NET для гибкого и точного управления содержанием с помощью передовых поисковых алгоритмов. [Изучите больше](https://docs.groupdocs.com/search/net/search-results/).
        {{< landing/code title="Как обработать результат поиска">}}
        ```csharp {style=abap}
        // Создайте индекс
        Index index = new Index("C:/IndexFolder");
        index.Add("C:/DocumentFolder");

        // Настройте параметры поиска
        SearchOptions options = new SearchOptions();
        options.FuzzySearch.Enabled = true;
        options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3);

        // Ищите документы, содержащие слово 'вода' или фразу 'Lorem ipsum'
        string query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.Search(query, options);
        
        // Обработайте результат поиска
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
    - title: "Расширенный поиск с использованием регулярных выражений"
      content: |
        GroupDocs.Search for .NET поддерживает регулярные выражения для точных поисков. [Изучите передовые методы](https://docs.groupdocs.com/search/net/regular-expression-search/).
        {{< landing/code title="Как искать с использованием регулярных выражений">}}
        ```csharp {style=abap}   
        // Создайте индекс
        Index index = new Index("c:/IndexFolder");
        index.Add("c:/DocumentFolder");
 
        // Ищите фразу в текстовом формате

        // Первый символ ^ в начале указывает, что это поисковый запрос с использованием регулярного выражения
        string query = "^^(.)\\1{1,}";
        // Ищите два или более одинаковых символа в начале слова
        SearchResult result = index.Search(query);
 
        ```
        {{< /landing/code >}}

---
