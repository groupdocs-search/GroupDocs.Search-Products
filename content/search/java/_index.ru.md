---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Text Search & Индексация API для документов, PDF, Office и Интернета"
head_description: "Расширенный API текстового поиска для приложений Java для поиска, индексации и извлечения данных из документов: форматы PDF, Word, Excel, презентации, электронная почта и веб-файлы."

############################# Header ############################
title: "Поиск и индексирование документов через Java API"
description: "Создавайте приложения Java для выполнения манипуляций с текстовым поиском во всех популярных форматах документов."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Search for Java"
        image: "/border/groupdocs-search-java.svg"
        product: "GroupDocs.Search"
        platform: "Java"

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
            - link: "https://purchase.groupdocs.com/pricing/search/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/search"
        link_learn: "https://docs.groupdocs.com/search/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Обзор ############################
overview:
    enable: true
    content: |
      GroupDocs.Search для Java позволяет создавать бизнес-приложения, которые позволяют вашим конечным пользователям выполнять операции поиска, как никогда раньше. Наш Java API позволяет пользователям использовать функции текстового поиска от базового до расширенного уровня. Создание и объединение нескольких индексов. Используйте простые, логические, регулярные выражения (регулярные выражения), нечеткие и другие типы запросов для быстрого и эффективного поиска по индексам. Вы можете получить необходимую информацию из файлов, документов, электронных писем и архивов, поскольку GroupDocs.Search for Java поддерживает все популярные форматы файлов.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          Ниже приводится обзор GroupDocs.Search для Java:

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
          GroupDocs.Search для Java поддерживает все популярные [форматы файлов документов](https://docs.groupdocs.com/search/java/supported-document-formats/), включая: Microsoft Office, изображения, диаграммы и многие другие.

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
          GroupDocs.Search for Java поддерживает следующие Операционные системы, фреймворки и менеджеры пакетов:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Операционные системы"
              content: |
                * Рабочий стол Microsoft Windows
                * Сервер Microsoft Windows
                * линукс
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Поддерживаемые платформы"
              content: |
                * Java 7 (1.7) и выше

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Среды разработки"
              content: |
                * NetBeans
                * IntelliJ ИДЕЯ
                * Затмение
            # table loop
            - icon: "fas fa-tools"
              title: "Инструмент автоматизации сборки"
              content: |
                * Мавен

############################# Функции ############################
features:
    enable: true
    title: "GroupDocs.Search for Java Функции"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Создайте индекс на диске или в памяти с помощью асинхронной многопоточности"

      # feature loop
      - icon: "fas fa-eye"
        content: "Просмотр хода создания и обновления индекса"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Выборочно пропускать индексацию для определенных файлов и пропускать определенные слова для более быстрого индексирования"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Выполнить импорт или использовать список для изменения символов во время индексации и экспорта в файл"

      # feature loop
      - icon: "fas fa-code"
        content: "Перезагрузить индекс в случае ошибки Индексация и предупредить пользователя о противоречивых настройках"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Уведомление о статусе индекса относительно последних обработанных файлов"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Индексируйте заархивированные архивы внутри других ZIP-архивов и получайте список проиндексированных файлов в архиве"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Экономьте место благодаря компактной индексации и защищенным паролем документам Индексация"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Document Извлечение текста из индекса или исходного файла"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Извлечение текста в формате HTML в файл и создание URL-адреса для навигации по результатам поиска в HTML"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Добавляйте произвольные дополнительные поля в каждый документ во время Индексация"

      # feature loop
      - icon: "fas fa-columns"
        content: "Настроить уровень сходства для Нечеткий поиск и показать лучшие результаты"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Интеллектуальное управление опечатками через Нечеткий поиск"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Use Граненый и логический Искать одновременно"

      # feature loop
      - icon: "fas fa-print"
        content: "Настройте и выполняйте поиск синонимов и разумно работайте с омофоническими терминами"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Использовать диапазон дат и чувствительность к регистру в качестве параметров поиска"

      # feature loop
      - icon: "fas fa-lock"
        content: "Сделать индекс для поиска и просмотра сообщений электронной почты через Aspose.Email API"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Используйте поисковые фразы с проверкой орфографии и Дикие карты и пропускайте специальные символы в запросах"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Создание единого дерева объектов путем объединения нескольких запросов"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Разделите поиск на более мелкие фрагменты для быстрого поиска в огромных индексах"

      # feature loop
      - icon: "fas fa-heading"
        content: "Индексировать документы из потоков и структур данных"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Настройте фильтрацию документов в результатах поиска"

      # feature loop
      - icon: "fas fa-cube"
        content: "Добавить английские синонимы в словарь синонимов по умолчанию"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Включите точное количество вхождений для каждого найденного слова, чтобы предлагать альтернативные варианты слов в случае орфографической ошибки"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Добавляйте текстовые атрибуты в проиндексированные документы без переиндексации"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Выполнение операций индексации и поиска по символам"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Указатель метаданных нетекстовых форматов документов"

    больше_функций:
      # more_feature_loop
      - title: "Индексация and Search Operation"
        content: |
         Индексация используется GroupDocs.Search for Java для сбора данных, а также их хранения и анализа для точных и эффективных операций поиска. GroupDocs.Search for Java часто использует такие индексы для выполнения поиска.

          * **Создать индекс**: создайте папку индекса и добавьте/индексируйте документы в эту папку.
          * **Загрузить индекс**: загрузить существующий индекс.
          * **Добавить документы в индекс**: добавьте документы в существующий индекс асинхронно.
          * **Обновить индекс**: Обновлять существующий индекс всякий раз, когда документ изменяется, добавляется или удаляется. Это поддерживает актуальность результатов поиска.
          
          ```java
          Index index = new Index("c:\\index");
          index.addToIndex("c:\\document");
          SearchResults result = index.search("?effet & principe?(2~4)");
          ```
      # more_feature_loop
      - title: "Объединение нескольких индексов для повышения эффективности поиска"
        content: "GroupDocs.Search for Java API предоставляет возможность объединять несколько индексов в общий индекс. Для часто изменяемого индекса создается несколько дельта-индексов. Однако такой подход снижает производительность поиска. GroupDocs.Search для Java преодолевает это узкое место, создавая один общий индекс путем слияния различных дельта-индексов. Этот общий объединенный индекс содержит всю информацию объединенных дельта-индексов. Такой подход сохраняет дельта-индексы неизменными, при этом значительно повышая эффективность поиска. Вы можете настроить различные функции для дальнейшей настройки этого процесса."

      # more_feature_loop
      - title: "Распознавание поисковых запросов с различной раскладкой клавиатуры"
        content: "GroupDocs.Search for Java распознает поисковые запросы, не соответствующие вашей раскладке клавиатуры. На данный момент GroupDocs.Search for Java успешно распознает 88 языков и 164 различных раскладки клавиатуры."

      # more_feature_loop
      - title: "Поиск с использованием морфологической формы слова"
        content: "Используя GroupDocs.Search for Java, вы можете свободно искать различные словоформы. Вы можете искать форму единственного и множественного числа конкретного существительного. Или вы можете выбрать поиск по всем формам глагола. Также можно искать корень, единственное число от третьего лица и простое прошедшее время, а также различные другие формы. Для языков, отличных от английского, вы можете настроить индивидуальные словоформы.."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Search предлагает API для просмотра документов для других популярных сред разработки."

    solution:
        # solution loop
        - img_alt: "GroupDocs.Search for .NET"
          image: "/border/groupdocs-search-net.svg"
          product: "GroupDocs.Search"
          platform: ".NET"
          link: "/search/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---