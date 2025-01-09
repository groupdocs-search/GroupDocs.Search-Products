---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: ru
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
head_title: "Решение для поиска и индексирования документов Java для PDF, офисных файлов и веб-содержимого"
head_description: "Мощный поиск текста и индексирование для приложений Java. Находите и организовывайте данные в PDF, Word, Excel, презентациях, электронных письмах и веб-форматах."

############################# Header ############################
title: "Эффективный поиск и индексирование документов с API Java"
description: "Удостоверьте приложения Java с надежными функциями текстового поиска во всех популярных форматах документов."
words:
  for: "для"

actions:
  main: "Скачайте Maven бесплатно"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-search/"
  alt: "Лицензирование"
  alt_link: "https://purchase.groupdocs.com/pricing/search/java/"
  title: "Начните ваше путешествие сегодня!"
  description: "Изучите возможности GroupDocs.Search бесплатно или получите лицензию, чтобы разблокировать его полный потенциал."

release:
  title: "Версия {0} выпущена"
  notes: "Смотрите, что нового"
  downloads: "Скачивания"

code:
  title: "Поиск текста в файлах с использованием Java"
  more: "Больше примеров"
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
    // Создайте индекс для ваших документов
    Index index = new Index("c:/MyIndex");

    // Добавьте документы в индекс для эффективного поиска
    index.add("c:/MyDocuments");
    
    // Ищите конкретные слова или фразы, такие как
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Обзор GroupDocs.Search"
  description: "Откройте для себя мощные возможности текстового поиска библиотеки Java Java."
  features:
    # feature loop
    - title: "Индексирование и операции поиска в Java"
      content: "С GroupDocs.Search for Java вы можете эффективно собирать, хранить и анализировать данные, создавая детализированные индексы для более быстрых и точных поисков."

    # feature loop
    - title: "Оптимизация поиска путем объединения индексов"
      content: "Легко объединяйте несколько индексов с помощью GroupDocs.Search for Java для оптимизации поиска. Уменьшите влияние небольших дельта-индексов, консолидировав их в один высокопроизводительный индекс."

    # feature loop
    - title: "Поддержка многоязычных раскладок клавиатуры"
      content: "Ищите на разных языках и раскладках клавиатуры с GroupDocs.Search for Java. Он поддерживает 88 языков и 164 конфигурации клавиатуры для непревзойденной универсальности."

    # feature loop
    - title: "Морфологические возможности поиска"
      content: "Находите различные формы слов, такие как единственное и множественное число существительных или варианты глаголов с помощью GroupDocs.Search for Java. Настройте параметры поиска для английского и других языков."

############################# Platforms ############################
platforms:
  enable: true
  title: "Независимость от платформы"
  description: "GroupDocs.Search for Java совместим с основными операционными системами и менеджерами пакетов."
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
  title: "Поддерживаемые форматы файлов"
  description: |
    Работайте с широким спектром форматов файлов с помощью GroupDocs.Search for Java. [Смотрите полный список](https://docs.groupdocs.com/search/java/supported-document-formats/).
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
  title: "Функции GroupDocs.Search for Java"
  description: "Эффективно управляйте содержимым документов с помощью расширенных возможностей поиска, поддерживающих форматы, такие как PDF, DOCX, XLSX, PPTX и другие."

  items:
    # feature loop
    - icon: "document_info"
      title: "Настраиваемые параметры поиска"
      content: "Уточняйте поиск с использованием фильтров по диапазону дат и чувствительности к регистру."

    # feature loop
    - icon: "detect"
      title: "Усиленная проверка правописания"
      content: "Эффективно ищите с исправлением правописания, подстановочными знаками и игнорированием специальных символов."

    # feature loop
    - icon: "collect"
      title: "Фильтрация результатов поиска"
      content: "Применяйте фильтры для уточнения результатов поиска по типам документов или критериям."

    # feature loop
    - icon: "get"
      title: "Импорт и экспорт данных индекса"
      content: "Легко импортируйте данные для индексирования или экспортируйте результаты в файлы для дальнейшего использования."

    # feature loop
    - icon: "remove"
      title: "Пропуск ненужных файлов"
      content: "Оптимизируйте индексирование, исключая определенные файлы или слова."

    # feature loop
    - icon: "style"
      title: "Обработка HTML и URL"
      content: "Извлекайте содержимое HTML в файлы и генерируйте URL для навигации по результатам поиска."

    # feature loop
    - icon: "detect"
      title: "Быстрый поиск в больших индексах"
      content: "Ускорьте операции поиска, разделяя большие индексы на управляемые части."

    # feature loop
    - icon: "manipulate"
      title: "Индексирование на основе потоков"
      content: "Индексируйте данные непосредственно из потоков или структур данных."

    # feature loop
    - icon: "compare"
      title: "Обработка ошибочных запросов"
      content: "Обнаруживайте опечатки и предлагайте альтернативные слова для повышения точности поиска."

    # feature loop
    - icon: "unreadable_characters"
      title: "Полноценная поддержка архивов"
      content: "Индексируйте вложенные архивы и извлекайте детализированные списки файлов внутри ZIP-файлов."

    # feature loop
    - icon: "hidden_print"
      title: "Компактное индексирование"
      content: "Экономьте место на диске с помощью компактного индексирования и обрабатывайте зашифрованные файлы."

    # feature loop
    - icon: "style"
      title: "Поддержка временных синонимов"
      content: "Расширяйте словарь синонимов для повышения точности поиска с использованием адаптированных опций."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Примеры кода"
  description: "Попробуйте функции GroupDocs.Search for Java с помощью этих примеров кода."
  items:
    # code sample loop
    - title: "Повышение точности поиска с помощью нечеткого соответствия"
      content: |
        Изучите возможности GroupDocs.Search for Java для управления содержимым с помощью передовых возможностей нечеткого поиска. [Узнайте больше](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="Как обработать результат поиска">}}
        ```java {style=abap}
        // Создайте индекс
        Index index = new Index("C:/IndexFolder");
        index.add("C:/DocumentFolder");

        // Настройте параметры поиска
        SearchOptions options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Ищите документы, содержащие слово 'вода' или фразу 'Lorem ipsum'
        String query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.search(query, options);
        
        // Обработайте результат поиска
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
    - title: "Уточнение результатов с помощью регулярных выражений"
      content: |
        Используйте регулярные выражения в GroupDocs.Search for Java для создания точных и детализированных результатов поиска. [Узнайте о передовых методах](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="Как искать с использованием регулярных выражений">}}
        ```java {style=abap}   
        // Создайте индекс
        Index index = new Index("C:/IndexFolder");
        index.add("c:/DocumentFolder");
 
        // Ищите фразу в текстовом формате

        // Первый символ ^ в начале указывает, что это поисковый запрос с использованием регулярного выражения
        String query = "^^(.)\\1{1,}";
        // Ищите два или более одинаковых символа в начале слова
        SearchResult result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
