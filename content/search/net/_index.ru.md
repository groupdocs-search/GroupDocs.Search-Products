---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C# .NET Text Search & Индексация API for Word Excel PDF Email HTML"
head_description: "API поиска текста C# .NET для интеллектуального индексирования и извлечения данных из PDF, Microsoft Office Word, Excel, презентаций, OneNote, электронной почты, ZIP, EPUB и веб-файлов."

############################# Header ############################
title: ".NET API для поиска и индексирования документов"
description: "API для индексации данных и выполнения текстового поиска во всех популярных форматах документов с использованием приложений .NET."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Search for .NET"
        image: "/border/groupdocs-search-net.svg"
        product: "GroupDocs.Search"
        platform: ".NET"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Обзор"

            # button loop
            - link: "#features"
              text: "Функции"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/search"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/search/net"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/search"
        link_learn: "https://docs.groupdocs.com/search/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Обзор ############################
overview:
    enable: true
    content: |
      GroupDocs.Search для .NET — это API поиска документов и текста для бизнес-приложений, разработанных на C#, ASP.NET и других технологиях .NET. Этот .NET API поддерживает базовые и расширенные функции поиска, например, создание и объединение нескольких индексов, поиск в индексах с использованием Простой, Логических, Нечетких, Регулярных выражений (regex) и других типов запросов для извлечения необходимых данных из файлов, документов и электронной почты, через интеллектуальный поиск. Если вы хотите создать для конечных пользователей быстрое, надежное, интеллектуальное и многофункциональное поисковое приложение, поддерживающее все популярные форматы файлов, GroupDocs.Search для .NET — это все, что вам нужно.

    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Ниже приведен обзор GroupDocs.Search для .NET:
      
        left:
          enable: true
          icon: "fas fa-search"
          title: "Индексация"
          content: |
            * Создание и управление
            * Объединить несколько индексов
            * Multi-Threading Async Индексация
            * Compact Индексация
            * Archived Files Индексация
        
        right:
          enable: true
          icon: "fas fa-search-plus"
          title: "Расширенный поиск и поисковые запросы"
          content: |
            * Нечеткий поиск
            * Поиск синонимов
            * Поиск по электронной почте
            * Обращение с омофоническими терминами
            * Поиск защищенных файлов
            * Простой
            * Дикая карта
            * Регулярное выражение (регулярное выражение)
            * Граненый и логический
            * Деликатный случай
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Search для .NET поддерживает следующие [форматы файлов документов](https://docs.groupdocs.com/search/net/supported-document-formats/):

        left:
          enable: true
          table:
            # table loop
            - title: "Форматы Microsoft Office"
              content: |
                * **Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM
                * **Excel**: XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
                * **PowerPoint**: PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
                * **Project**: MPP
                * **Diagram**: VSD, VSS
                * **Microsoft Compiled HTML**: CHM
                * **OneNote**: ONE

        right:
          enable: true
          table:
            # table loop
            - title: "OpenDocument & Другие форматы"
              content: |
                * **Переносимый формат документа**: PDF
                * **OpenDocument**: ODT, OTT, ODS, OTS, ODP
                * **Электронная почта**: PST, OST, MSG, EML, EMLX
                * **Форматы веб-файлов**: XML, HTM, HTML, XHTML, MHT, MHTML
                * **Аудио**: MP3, WAV
                * **Видео**: AVI, MOV, QT, FLV, ASF
                * **Текст**: TXT
                * **Расширенный текстовый формат**: RTF
                * **Файл документации Markdown**: MD
                * **Изображения**: BMP, GIF, JP2, PNG, WEBP, TIFF, EMF, WMF, JPG, PSD
                * **Другие**: TORRENT, ZIP, DCM, DJVU, EPUB, FB2

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Search for .NET поддерживает следующие Операционные системы Менеджер пакетовs:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Операционные системы"
              content: |
                * Рабочий стол Windows
                * Windows-сервер
                * Windows Azure
                * линукс

            # table loop
            - icon: "fas fa-code"
              title: "Поддерживаемые платформы"
              content: |
                * .NET Framework 2.0 или выше
                * Монофреймворк 1.2 или выше
                * .NET Стандарт 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Менеджер пакетов"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Среды разработки"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * МоноДевелопмент

############################# Функции ############################
features:
    enable: true
    title: "GroupDocs.Search for .NET Функции"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Создать индекс в памяти или на диске и выполнить многопоточную индексацию и слияние"

      # feature loop
      - icon: "fas fa-eye"
        content: "Предотвратить индексацию уже проиндексированных файлов или с определенной строкой в ​​имени"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Просмотрите процент выполнения создания и обновления индекса и получите отчет о поиске"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Более быстрая индексация за счет исключения определенных слов и уведомления о статусе индекса для недавно обработанных файлов"

      # feature loop
      - icon: "fas fa-code"
        content: "Индексируйте ZIP-архивы в ZIP-архивах и получайте список проиндексированных файлов, содержащихся в архиве"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Используйте список или импорт для замены символов во время индексации и экспорта их в файл"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Индексация и поиск файлов, защищенных паролем, и компактная индексация для экономии места на диске"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Извлечение текста из индекса или исходного файла и автоматическое сохранение кодировки текстового файла в индексе"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Добавляйте произвольные дополнительные поля в каждый документ во время индексации"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Настройте фильтрацию документов в результатах поиска"

      # feature loop
      - icon: "fas fa-columns"
        content: "Индексировать документы из потоков и структур данных"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Поиск полной фразы со стоп-словами и объединение фасетного поиска с логическим поиском"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Search based on Homophonic Terms, Synonyms, Date Range, Дикая картаs & Case Sensitivity"

      # feature loop
      - icon: "fas fa-print"
        content: "Индексируйте и ищите электронные письма из Outlook и просматривайте с помощью Aspose.Email API"

      # feature loop
      - icon: "fas fa-lock"
        content: "Ограничение результатов для каждого термина в поисковом запросе, а также для всех результатов"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Извлечение текста HTML в файл и создание URL-адреса для навигации по результатам поиска в формате HTML"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Объединение нескольких запросов в единое дерево объектов"

      # feature loop
      - icon: "fas fa-heading"
        content: "Включите точное количество вхождений для каждого найденного слова, чтобы предлагать альтернативные варианты слов в случае орфографической ошибки"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Добавляйте текстовые атрибуты в проиндексированные документы без переиндексации"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Указатель метаданных нетекстовых форматов документов"

    больше_функций:
      # more_feature_loop
      - title: "Индексация & Search"
        content: |
          GroupDocs.Search for .NET API часто использует индекс для выполнения поиска. Индексы используются для сбора, анализа или хранения данных для быстрого и точного поиска.

          * **Создать индекс**: создайте папку индекса и добавьте/индексируйте документы в эту папку.
          * **Загрузить индекс**: загрузить существующий индекс.
          * **Добавить документы в индекс**: добавьте документы в существующий индекс асинхронно.
          * **Обновить индекс**: Обновлять существующий индекс всякий раз, когда документ изменяется, добавляется или удаляется. Это поддерживает актуальность результатов поиска.

          ```cs
          Index  index = new Index(@"c:\MyIndex");
          index.AddToIndex(@"c:\MyDocuments");
          SearchResults searchResults =  index.Search("searchTerm");
          ```
      # more_feature_loop
      - title: "Объединение нескольких индексов для повышения эффективности поиска"
        content: "GroupDocs.Search для .NET может объединять несколько индексов в единый индекс. Если индекс часто обновляется, он имеет несколько дельта-индексов, но такой подход снижает производительность поиска. GroupDocs.Search for .NET API объединяет все дельта-индексы в один сводный индекс. Первичный объединенный индекс будет содержать всю информацию из объединенных дельта-индексов; однако дельта-индексы останутся без изменений. Такой подход, используемый нашим API, значительно повышает эффективность поиска. Функция слияния индексов предоставляет множество функций для дальнейшей настройки этого процесса."

      # more_feature_loop
      - title: "Сохраните текст в индексе для создания HTML-разметки"
        content: "GroupDocs.Search для .NET может кэшировать текст проиндексированных документов в индексе. Затем этот кэшированный текст используется для быстрого создания HTML-разметки путем выделения результатов поиска. Этот подход намного быстрее, чем извлечение текста непосредственно из файлов. Извлечение текста из кеша будет доступно, даже если исходные файлы больше не доступны. Кэшированный текст можно сохранить, применяя различные уровни сжатия, чтобы занимать меньше места на диске и быстрее индексировать время."

      # more_feature_loop
      - title: "Получить связанные документы с помощью нечеткого и регулярного поиска"
        content: "Когда вы выполняете нечеткий или регулярный поиск, вы можете получить список документов, которые точно соответствуют введенным вами данным. Однако вы также получите список документов, содержащих слова или термины, похожие на введенные вами. Например, если с помощью GroupDocs.Search для .NET выполнить нечеткий поиск по запросу «стоимость», вы получите документы, содержащие слово «стоимость», и документы, содержащие похожие слова, такие как «пальто». Результаты будут зависеть от того, какой уровень нечеткости вы настроили с помощью этого API."

      # more_feature_loop
      - title: "Распознавание поисковых запросов с различной раскладкой клавиатуры"
        content: "GroupDocs.Search for .Net может распознавать поисковые запросы, написанные на языке, который не соответствует вашей раскладке клавиатуры. В настоящее время этот .NET API может успешно распознавать 88 языков и 164 различных раскладки клавиатуры.."

      # more_feature_loop
      - title: "Поиск с использованием морфологической формы слова"
        content: "GroupDocs.Search for .NET API позволяет выполнять поиск по различным словоформам. Например, для существительного вы можете искать его формы единственного и множественного числа. Для глагола вы можете искать все формы этого глагола. Вы также можете искать корень, единственное число от третьего лица, простое прошедшее время и различные другие формы. Для языков, отличных от английского, вы можете реализовать настраиваемые словоформы.."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Search предлагает API для просмотра документов для других популярных сред разработки."

    solution:
        # solution loop
        - img_alt: "GroupDocs.Search for Java"
          image: "/border/groupdocs-search-java.svg"
          product: "GroupDocs.Search"
          platform: "Java"
          link: "/search/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---
