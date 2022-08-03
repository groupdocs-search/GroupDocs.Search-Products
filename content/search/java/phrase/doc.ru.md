---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ru/search/java/phrase/doc/"
otherformats: PDF DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB FB2 

############################# Head ############################
head_title: "API Java для поиска и поиска точной фразы в документах DOC"
head_description: "GroupDocs.Search Java API помогает программистам внедрить поиск по фразе и обнаружить заданную последовательность слов или точную фразу в тексте документов DOC с помощью Java."

############################# Header ############################
title: "Как искать и просматривать точное предложение или фразу в документах DOC через Java API?"
description: "GroupDocs.Search Java API обеспечивает полную поддержку расширенных возможностей поиска, позволяя разработчикам программного обеспечения находить точное предложение или фразу в документах DOC с помощью поиска по фразе или точного поиска по предложению."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Что такое поиск по фразе и как его использовать в приложениях Java?"
    content: |
       Поиск по фразе — это очень эффективный способ поиска внутри документов или веб-страниц точного предложения или фразы, а не ключевого слова. Это означает, что когда пользователь ищет точную фразу, он хочет найти все условия поиска в том порядке, в котором они появились. Эта веб-страница будет делиться информацией о том, как пользователи могут разрабатывать бизнес-приложения и инструменты для эффективного поиска документов и веб-страниц с использованием Java API. GroupDocs.Search для Java — это очень хорошо организованный и эффективный Java API, который позволяет разработчикам программного обеспечения выполнять операции текстового поиска от базового до продвинутого уровня в своих собственных приложениях без установки какого-либо стороннего программного обеспечения. API включает в себя множество полезных функций, связанных с поиском документов, таких как простой или логический поиск, нечеткий поиск, поиск с учетом регистра, синоним, омофон, подстановочный знак, поиск по типу объекта, установка диапазона данных и другие типы запросов для быстрого и элегантного поиска информации. Более того, он также поддерживает распознавание поисковых запросов, написанных на языке, который не соответствует вашей раскладке клавиатуры.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Поиск по фразе в документах DOC с помощью Java"
      content_left: |
       GroupDocs.Search Java API включает полную поддержку расширенного поиска, что позволяет специалистам по программному обеспечению создавать мощные программные приложения с возможностями поиска и простотой использования. Приведенный ниже код Java показывает, как выполнить поиск по фразе в текстовой и объектной форме с помощью всего нескольких строк кода.

      title_right: "Точный поиск предложения в файлах DOC"
      content_right: |
         * Определите путь к папке индекса и папке документов.
         * Создание индекса в указанной папке путем вызова экземпляра класса [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String))
         * Индексирование документов из указанной папки путем вызова метода [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String))
         * Поиск с помощью текстового запроса путем вызова метода [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery))
         * Поиск фразы «текст фразы» в объектной форме
         * Создание word1, word2 и создание подзапроса 3 путем вызова метода [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String))
         * Объединение подзапросов для создания нового поискового запроса путем вызова [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) метод
         * Начать поиск и отображать результаты поиска
         
        
      gisthash: "396c41cda822cf79f31dd37c6740fa03"
      gistfile: "phrase_search_in_text_queries_java.java"

    - title_left: "Применение поиска фраз с подстановочными знаками в файлах DOC с помощью Java"
      content_left: |
        GroupDocs.Search for Java дает программистам возможность добавлять функции поиска по фразам с подстановочными знаками при поиске файлов DOC внутри приложения Java. В следующих примерах кода Java показано, как применять поиск фраз с подстановочными знаками в различных типах документов с помощью Java API.

      title_right: "Поиск по фразе с подстановочными знаками в Java"
      content_right: |
        * Определите путь к папке индекса и папке документов.
        * Создание индекса в указанной папке путем вызова экземпляра класса [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String))
        * Индексирование документов из указанной папки путем вызова метода [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String))
        * Поиск с помощью текстового запроса путем вызова метода [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery))
        * Поиск фразы «текст фразы» в объектной форме
        * Создание word1 и word3 путем вызова метода [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String))
        * Создание подстановочного знака2 путем вызова метода [createWildcardQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWildcardQuery(int,%20int))
        * Объединение подзапросов для создания нового поискового запроса по фразе путем вызова [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) метод
        * Начать поиск и отображать результаты поиска
     
      gisthash: "f21c8c4572883fecc0eeef82c2b814b1"
      gistfile: "use_wildcards_in_phrase_search_java.java"
      
    - title_left: "API Java для объединения поиска по фразе и других типов поиска"
      content_left: |
        GroupDocs.Search Java API позволяет программистам легко комбинировать фразовый поиск с другими типами поиска. В следующем коде Java показано, как выполнять поиск по фразе с помощью подстановочных знаков, представляющих слова и символы в словах.

      title_right: "Как совместить поиск по фразе и другие поиски"
      content_right: |
        * Определите путь к папке индекса и папке документов.
        * Создание индекса в указанной папке путем вызова экземпляра класса [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String))
        * Индексирование документов из указанной папки путем вызова метода [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String))
         * Поиск с помощью текстового запроса путем вызова метода [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery))
         * Поиск фразы «текст фразы» в объектной форме
        * Определите шаблон Word и добавьте строку и добавьте к ней подстановочный знак
        * Создание wordPattern1 и Word3 путем вызова метода [CreateWordPatternQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordPatternQuery(com.groupdocs.search.common.WordPattern))
        * Создание подстановочного знака2 путем вызова метода [createWildcardQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWildcardQuery(int,%20int))
        * Объединение подзапросов для создания нового поискового запроса по фразе путем вызова [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) метод
        * Начать поиск и отображать результаты поиска
     
      gisthash: "dbd0f2eb292796e63e6213461f080e0c"
      gistfile: "combine_phrase_search_with_others_java.java"

    - title_left: "Системные Требования"
      content_left: |
        GroupDocs.Search для Java поддерживается на всех основных платформах и операционных системах. Чтобы ознакомиться с полным руководством по системным требованиям, посетите [системные требования](https://docs.groupdocs.com/search/java/system-requirements/) перед выполнением приведенного ниже кода. Убедитесь, что на вашем компьютере установлены следующие предварительные требования. система:
          * Операционные системы: Microsoft Windows, Linux, MacOS
          * Поддержка версий Java: J2SE 7.0 (1.7), J2SE 8.0 (1.8) или выше
          * Получите последнюю версию GroupDocs.Search для Java API из GroupDocs  [репозитория](https://repository.groupdocs.com/repo/com/groupdocs/groupdocs-search/)
        
      title_right: "Зачем использовать GroupDocs.Search"
      content_right: |
        * Создание поискового индекса как в памяти, так и на диске.
        * Возможность индексации из файла, потока или структуры.
        * Поддержка индексирования защищенных паролем документов.
        * Поддержка слияния нескольких индексов.
        * Фильтровать документ во время поисковой индексации.
        * Поддержка проверки орфографии во время поиска.
        * Смешанные символы полностью поддерживаются
        * Объединение различных типов поиска в один поисковый запрос.
        * Поддержка простого поиска слов и регулярных выражений
        * Полная поддержка замены псевдонимов в поисковых запросах.

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---