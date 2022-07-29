---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ru/search/net/case-sensitive/xlsm/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Применить поиск текста с учетом регистра в документах XLSM через .NET"
head_description: "GroupDocs.Search .NET API позволяет программистам применять текстовый поиск с учетом регистра и находить точную последовательность слов в документах XLSM через .NET API."

############################# Header ############################
title: "Как применить поиск с учетом регистра в документах XLSM внутри приложений .NET?"
description: "GroupDocs.Search .NET API позволяет разработчикам программного обеспечения применять текстовый поиск с учетом регистра в различных типах документов, таких как PDF, HTML, DOCX, PPTX, XLSX и других, внутри приложений .NET."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Что такое поиск с учетом регистра и как его добиться с помощью .NET?"
    content: |
     Существует множество полезных методов поиска, которые могут помочь пользователям искать в различных типах документов определенную комбинацию слов или других данных. Поиск с учетом регистра — это очень полезный метод, который позволяет пользователям искать документы и веб-страницы независимо от того, считаются ли прописные и строчные буквы разными или одинаковыми. Например, «Компьютер», «компьютер» и «КОМПЬЮТЕР» будут рассматриваться как разные слова, потому что буква «С» в первом случае заглавная, во втором — строчная, а в третьем — все прописные. GroupDocs.Search для .NET — это удобный высокопроизводительный API для поиска документов, который позволяет разработчикам программного обеспечения создавать программные приложения и инструменты для выполнения текстового поиска, а также с легкостью индексировать документы. API обеспечивает поддержку некоторых из наиболее часто используемых форматов файлов, таких как PDF, HTML, электронная почта Outlook, Microsoft Office Word, листы Excel, презентации PowerPoint, Outlook MSG, PST и многие другие. Еще одна полезная функция заключается в том, что он может идентифицировать поисковые запросы, написанные на языке, который не соответствует вашей раскладке клавиатуры.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Выполнение поиска с учетом регистра в документах XLSM через .NET"
      content_left: |
       GroupDocs.Search .NET API позволяет программистам добавлять функции поиска с учетом регистра в свои собственные приложения C# .NET. В следующем примере кода .NET показано, как добиться поиска с учетом регистра с помощью запроса в текстовой форме в файлах XLSM всего за пару строк кода.

      title_right: "Применить поиск с учетом регистра в документах XLSM"
      content_right: |
         * Определите путь к индексной папке, а также к папке документов.
         * Создайте индекс в указанной папке, вызвав экземпляр класса [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2).
         * Индексирование документов из указанной папки путем вызова экземпляра класса [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1)
         * Инициализирует новый экземпляр класса [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions).
         * Включение поиска с учетом регистраb путем вызова метода [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch)
         * Определить строку поиска и начать поиск
         
        
      gisthash: "805df69ebb1145d5c15c212431de1395"
      gistfile: "case-sensitive_in_text_queries_dotnet.cs"

    - title_left: "Выполнение поиска с учетом регистра в форме объекта через .NET"
      content_left: |
        GroupDocs.Search .NET дает разработчикам программного обеспечения возможность находить слова с учетом прописных и строчных букв внутри приложения .NET. В следующем примере кода .NET показано, как применять поиск с учетом регистра с запросом в форме объекта в документах XLSM.

      title_right: "Сделать поиск с учетом регистра в документах XLSM"
      content_right: |
        * Определите путь к индексной папке, а также к папке документов.
        * Создайте индекс в указанной папке, вызвав экземпляр класса [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2).
        * Индексирование документов из указанной папки путем вызова экземпляра класса [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1)
        * Инициализирует новый экземпляр класса [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions).
        * Включение поиска с учетом регистраb путем вызова метода [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch)
        * Создание поискового запроса в объектной форме путем вызова метода [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery)
        * Начать поиск и отображать результаты поиска
     
      gisthash: "846d0dd11f88a59d62f083e33e84286b"
      gistfile: "case-sensitive_search_in_object_queries_dotnet.cs"

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