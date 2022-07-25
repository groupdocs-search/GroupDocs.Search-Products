---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ru/search/net/boolean/pptx/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Добавление логических операторов поиска (И, ИЛИ, НЕ) в поисковые запросы через .NET"
head_description: "GroupDocs.Search .NET API позволяет разработчикам программного обеспечения добавлять логический поиск или разрабатывать новые запросы с использованием логических операторов И, ИЛИ, НЕ внутри своих приложений .NET."

############################# Header ############################
title: "Разработка сложных поисковых запросов с использованием логических операторов И, ИЛИ, НЕ в приложениях .NET"
description: "GroupDocs.Search .NET API позволяет программистам разрабатывать сложные поисковые запросы с использованием логических операторов (И, ИЛИ, НЕ) внутри своих .NET-приложений. "

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Что такое логический поиск и как использовать логические операторы?"
    content: |
       Логический поиск — очень полезная процедура поиска, которая позволяет пользователям комбинировать различные ключевые слова с оператором для связывания, расширения и определения результатов поиска. Логические операторы, такие как И, ИЛИ, НЕ, РЯДОМ и т. д., помогают пользователям получить более широкий диапазон результатов или уменьшить количество несвязанных результатов поиска, определив ограничения. GroupDocs.Search для .NET — это мощный высокопроизводительный API для поиска документов, который позволяет разработчику программного обеспечения разрабатывать приложения, которые могут выполнять текстовый поиск и индексацию в некоторых из наиболее распространенных форматов файлов документов, таких как PDF, HTML, электронная почта Outlook, Microsoft Office Word, листы Excel. , презентации PowerPoint, Outlook MSG, PST и многое другое. Булев оператор И может использоваться для отображения результатов для всех введенных вами слов, оператор ИЛИ дает результаты для любого из введенных вами слов, оператор НЕ может использоваться для отображения результатов поиска для отсутствия вхождений и так далее. Одна замечательная функция заключается в том, что он может распознавать поисковые запросы, написанные на языке, который не соответствует вашей раскладке клавиатуры.  

############################# content ############################
steps:
    enable: true
    block:
    - title_left: «Используйте логический оператор И в поисковых запросах через .NET"
      content_left: |
       GroupDocs.Search .NET API обеспечивает полную поддержку добавления возможностей логического поиска внутри своего .NET-приложения. В приведенном ниже примере кода C# показано, как создать логический оператор "И" в текстовых и объектных запросах в их собственных приложениях .NET.

      title_right: " Поиск PPTX документов с помощью логического оператора AND"
      content_right: |
         * Сначала вам нужно указать путь к папке индекса и папке документов.
         * Создание индекса в указанной папке путем вызова экземпляра класса [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
         * Индексирование документов из указанной папки вызовом метода [Поиск](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
         * Создание подзапроса 1 и создание подзапроса 2 путем вызова класса [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery)
         * Объединение подзапросов в один запрос путем вызова метода [CreateAndQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
         * Начать поиск и отображать результаты поиска
         
        
      gisthash: "fa9773cd8d0f379a638e495ad2541a5b"
      gistfile: "use_boolean_and_operator_dotnet.cs"

    - title_left: "Как использовать логический оператор ИЛИ через .NET"
      content_left: |
       GroupDocs.Search для .NET — это мощный API, который позволяет программистам выполнять поиск во многих популярных форматах документов. В приведенных ниже примерах кода C# .NET показано, как использовать логический оператор «ИЛИ» в запросах текстовых и объектных форм внутри приложений C#.

      title_right: "Используйте логический оператор ИЛИ для поиска PPTX файлов"
      content_right: |
        * Сначала вам нужно указать путь к папке индекса и папке документов.
        * Создание индекса в указанной папке путем вызова экземпляра класса [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
        * Индексирование документов из указанной папки вызовом метода [Поиск](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
        * Создание подзапроса 1 и создание подзапроса 2 путем вызова класса [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery)
        * Объединение подзапросов в один запрос путем вызова метода [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery)
        * Начать поиск и отображать результаты поиска
     
      gisthash: "c0b22e80f881f8dbc0da17f92c01efc7"
      gistfile: "use_boolean_or_operator_dotnet.cs"
      
    - title_left: "Создание сложных поисковых запросов с использованием логических операторов"
      content_left: |
        GroupDocs.Search .NET позволяет программистам комбинировать различные логические операторы для создания сложных поисковых запросов в своих собственных приложениях .NET. В следующих примерах кода .NET показано, как усложнить поиск документов без установки какого-либо внешнего программного обеспечения или инструментов.

      title_right: "Поиск PPTX документов с помощью сложных поисковых запросов"
      content_right: |
        * Сначала вам нужно указать путь к папке индекса и папке документов.
        * Создание индекса в указанной папке путем вызова экземпляра класса [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
        * Индексирование документов из указанной папки вызовом метода [Поиск](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
        * Начать поиск и отобразить текстовый запрос результатов поиска
        * Поиск с запросом объекта
        * Создание WordQuery и relativityWordQuery путем вызова класса [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery).
        * Объединение подзапросов в один запрос путем вызова метода [CreateAndQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
        * Создание einsteinWordQuery и albertWordQuery путем вызова класса [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery).
        * Объединение подзапросов в один запрос путем вызова метода [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery)
        * Объединение подзапросов в один запрос путем вызова метода [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery)
        * Начать поиск и отображать результаты поиска
     
      gisthash: "216af02ebdd08331fdd05faf8c39e528"
      gistfile: "create_complex_queries_boolean_operator_dotnet.cs"

    - title_left: "Системные Требования"
      content_left: |
       GroupDocs.Search для .NET поддерживается на всех основных платформах и операционных системах. Чтобы ознакомиться с полным руководством по системным требованиям, посетите [системные требования](https://docs.groupdocs.com/search/net/system-requirements/) перед выполнением приведенного ниже кода. Убедитесь, что на вашем компьютере установлены следующие предварительные требования. система:
         * Операционные системы: Microsoft Windows, Linux, MacOS
         * Среда разработки: Visual Studio, Xamarin, MonoDevelop и т. д.
         * Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
         * Получите последнюю версию GroupDocs.Search для .NET API из [NuGet](https://www.nuget.org/packages/GroupDocs.search/)
        
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