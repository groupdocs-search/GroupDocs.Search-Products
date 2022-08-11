---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ru/search/net/filters/ods/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Настройка результатов поиска путем настройки фильтрации документов в приложениях .NET"
head_description: "GroupDocs.Search .NET API позволяет разработчикам программного обеспечения искать документы ODS Documents и настраивать результаты поиска, применяя фильтрацию документов в приложениях .NET."

############################# Header ############################
title: "Установите фильтрацию документов для настройки результатов поиска в приложениях .NET"
description: "GroupDocs.Search .NET API помогает программистам добавлять возможности поиска документов и настраивать результаты поиска, применяя фильтрацию документов в своих приложениях .NET."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Как применить фильтрацию документов в результатах поиска через .NET?"
    content: |
       Фильтрация — очень полезный метод, который позволяет пользователям проверять и обрабатывать функциональные возможности. Фильтрация документов предлагает пользователям простой способ навигации по результатам и поиска того, что они ищут. Это также дает пользователям возможность ограничить свой поиск определенным разделом или определенным типом документа. GroupDocs.Search для .NET — это многофункциональный высокопроизводительный API-интерфейс поиска документов, который позволяет разработчику программного обеспечения создавать приложения, поддерживающие текстовый поиск и индексирование. Он поддерживает некоторые из самых популярных форматов документов, таких как PDF, HTML, электронная почта Outlook, Microsoft Office Word, листы Excel, презентации PowerPoint, Outlook MSG, PST и многие другие. API полностью поддерживает настройку файлов документов для результатов поиска. Вы можете использовать несколько типов файловых систем для настройки результатов поиска, таких как фильтры пути к файлу, фильтр расширения файла, фильтр атрибута и многое другое. Также возможно комбинировать поисковые фильтры документов с помощью логических операторов AND, OR & NOT и т. д.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Установить фильтр документов при поиске ODS документов через .NET"
      content_left: |
       GroupDocs.Search .NET API помогает разработчикам программного обеспечения добавлять возможности поиска в свои приложения .NET. В следующем примере кода .NET показано, как применить фильтр документов при поиске различных типов документов с помощью всего пары строк кода.

      title_right: "Применить фильтр документов при поиске ODS документов"
      content_right: |
       * Сначала вам нужно указать путь к папке индекса и папке документов.
       * Создание индекса в указанной папке путем вызова экземпляра класса [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
       * Индексирование документов из указанной папки вызовом метода [Поиск](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
       * Создание объекта параметров поиска [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions)
       * Установите фильтр документов, вызвав [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Начать поиск и отображать результаты поиска
        
      gisthash: "77cafabe4e9c9256217b4326e26a59d0"
      gistfile: "set_document_filter_in_search_dotnet.cs"

    - title_left: "Как объединить фильтры документов поиска через .NET"
      content_left: |
        GroupDocs.Search для .NET позволяет программистам комбинировать поисковые фильтры документов при поиске, чтобы контролировать, какие из найденных документов должны быть возвращены в результате поиска внутри приложения C# .NET. В следующих примерах кода .NET показано, как объединить фильтры документов поиска с помощью логических операторов И, ИЛИ, НЕ и т. д. в приложениях C#.

      title_right: "Объединить фильтры поисковых документов при поиске файлов ODS"
      content_right: |
       * Сначала вам нужно указать путь к папке индекса и папке документов.
       * Создание составного фильтра И, который возвращает все документы FB2 и EPUB, полные пути которых содержат слово «Эйнштейн».
       * Создайте filter1, вызвав [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Создайте filter2, вызвав [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Комбинируйте фильтры, вызывая метод [andFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createand).
       * Создание составного фильтра ИЛИ, который возвращает все документы DOC, DOCX, PDF и все документы, в полных путях которых есть слово Einstein.
       * Создайте filter3, вызвав [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Создайте filter4, вызвав [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Комбинируйте фильтры, вызывая метод [orFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createor).
       * Создание фильтра, который возвращает все найденные документы, кроме документов TXT
       * Создайте filter4, вызвав [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Фильтр Appy Not путем вызова метода [notFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createnot)

      gisthash: "db4efe513cbd34925231be10a992f23c"
      gistfile: "combine_document_filter_in_search_dotnet.cs"
      
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