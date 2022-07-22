---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ru/search/net/phrase /ppsx/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Как добавить фразовый поиск в документы PPSX в приложениях .NET?"
head_description: "GroupDocs.Search .NET API позволяет программистам добавлять фразовый поиск и находить точную фразу или указанную последовательность слов в документах PPSX через .NET API."

############################# Header ############################
title: "Добавить точное предложение или фразу для поиска в документах PPSX внутри приложений .NET?"
description: "GroupDocs.Search .NET API позволяет программистам находить указанную последовательность слов в документах PPSX с помощью поиска по фразе или точного поиска по предложению в приложениях .NET. "

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Как использовать поиск по точному предложению или фразе в приложениях .NET?"
    content: |
       Поиск точного предложения или фразы — это вид поиска, который позволяет пользователям искать документы, Интернет или базу данных, содержащие точное предложение или фразу, содержащую определенный порядок и комбинацию слов, определенных потребителями. Это очень распространенный термин в терминологии поисковых систем, который позволяет пользователям искать документы по заданной последовательности слов в тексте проиндексированных документов. GroupDocs.Search для .NET — это очень полезный высокопроизводительный API для поиска документов и текста, предоставляющий полную функциональность для разработки приложений для текстового поиска и индексирования, поддерживающих некоторые из наиболее распространенных типов документов, таких как PDF, HTML, электронная почта Outlook, Microsoft Office Word, Таблицы Excel, презентации PowerPoint, Outlook MSG, PST и так далее. Он включает поддержку нескольких функций, связанных с поиском по фразе, таких как поисковый запрос в текстовой и объектной форме, использование подстановочных знаков при поиске по фразе и так далее.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Как выполнить поиск по фразе в документах PPSX через .NET"
      content_left: |
       GroupDocs.Search .NET API позволяет разработчикам программного обеспечения добавлять функции поиска фраз в свои собственные приложения C# .NET. В следующем примере кода .NET показано, как выполнить поиск по фразе в тексте и объекте, используя всего пару строк кода.

      title_right: "Точный поиск по фразе в документах PPSX"
      content_right: |
         * Сначала вам нужно указать путь к папке индекса и папке документов.
         * Создание индекса в указанной папке путем вызова экземпляра класса [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
         * Индексирование документов из указанной папки вызовом метода [Поиск](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
         * Поиск фразового запроса «фразовый текст» в текстовой форме
         * Поиск фразы «текст фразы» в объектной форме
         * Создание word1, word2 и создание подзапроса 3 путем вызова метода [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery)
         * Объединение подзапросов для создания нового поискового запроса путем вызова метода [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery)
         * Начать поиск и отображать результаты поиска
         
        
      gisthash: "a5696884acf504acc319ba97465248cd"
      gistfile: "phrase_search_in_text_queries_dotnet.cs"

    - title_left: "Поиск подстановочных фраз в документах PPSX через .NET"
      content_left: |
        GroupDocs.Search для .NET позволяет программистам добавлять функции поиска по фразам с помощью подстановочных знаков внутри приложения C# .NET. В следующих примерах кода .NET показано, как применять поиск фраз с подстановочными знаками в документах PPSX внутри приложений C#.

      title_right: "Применить поиск фраз с подстановочными знаками в файле PPSX"
      content_right: |
        * Сначала вам нужно указать путь к папке индекса и папке документов.
        * Создание индекса в указанной папке путем вызова экземпляра класса [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
        * Индексирование документов из указанной папки вызовом метода [Поиск](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
        * Поиск фразового запроса «фразовый текст» в текстовой форме
        * Поиск фразы «текст фразы» в объектной форме
        * Создание word1 и создание подзапроса 3 путем вызова метода [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery)
        * Создание подстановочного знака2 путем вызова метода [CreateWildcardQuery](https://apireference.groupdocs.com/search/net/groupdocs.search.searchquery/createwildcardquery/methods/1)
        * Объединение подзапросов для создания нового поискового запроса путем вызова метода [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery)
        * Начать поиск и отображать результаты поиска
     
      gisthash: "3ff2bf9f8ba902d8d7ebead67a934654"
      gistfile: "use_wildcards_in_phrase_search_dotnet.cs"
      
    - title_left: "Комбинируйте поиск по фразе с другими типами поиска через .NET"
      content_left: |
        GroupDocs.Search .NET дает программистам возможность сочетать поиск по фразе с другими типами поиска внутри приложения .NET. В следующих примерах кода .NET показано, как применять как подстановочные знаки, представляющие слова, так и символы в словах.

      title_right: ".NET API для объединения поиска по фразе с другими поисками"
      content_right: |
        * Сначала вам нужно указать путь к папке индекса и папке документов.
        * Создание индекса в указанной папке путем вызова экземпляра класса [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
        * Индексирование документов из указанной папки вызовом метода [Поиск](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
        * Поиск фразы в текстовом виде
        * Поиск фразы в объектной форме
        * Определите шаблон Word и добавьте строку.
        * Создание wordPattern1 и Word3 путем вызова метода [CreateWordPatternQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordpatternquery)
        * Создание подстановочного знака2 путем вызова метода [CreateWildcardQuery](https://apireference.groupdocs.com/search/net/groupdocs.search.searchquery/createwildcardquery/methods/1)
        * Объединение подзапросов для создания нового поискового запроса путем вызова метода [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery)
        * Начать поиск и отображать результаты поиска
     
      gisthash: "db5c32ed21237f3e1cd7cdbde0778c29"
      gistfile: "combine_phrase_search_with_others_dotnet.cs"

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