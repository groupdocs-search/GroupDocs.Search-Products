---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ru/search/java/case-sensitive/xhtml/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP  MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "API Java для выполнения поиска текста с учетом регистра в документах XHTML"
head_description: "GroupDocs.Search Java API позволяет программистам выполнять текстовый поиск с учетом регистра и определять точную структуру слов в документах XHTML с помощью Java."

############################# Header ############################
title: "Выполнение поиска с учетом регистра в документах XHTML в приложениях Java"
description: "GroupDocs.Search Java API позволяет разработчикам программного обеспечения применять текстовый поиск с учетом регистра по различным типам документов, таким как PDF, HTML, DOCX, PPTX, XLSX и другим, в приложениях Java."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Как выполнить поиск с учетом регистра в приложениях Java?"
    content: |
      Чувствительность к регистру — это очень полезный метод поиска, который описывает способность программы различать прописные (заглавные) и строчные (строчные) буквы при поиске в Интернете, базе данных или документе. Очень важно помнить, что по умолчанию поисковая система нечувствительна к регистру, а это означает, что поиск по слову Компьютер выдаст как фрагменты, имеющие имя ключа, так и текст со словами Компьютер и компьютер. Предположим, нам нужно сузить результаты поиска до тех, которые имеют заглавную букву «Компьютер», что означает, что нам нужен поиск с учетом регистра. GroupDocs.Search для Java — это эффективный API для поиска и индексирования документов, который позволяет разработчику программного обеспечения разрабатывать приложения, которые могут выполнять текстовый поиск и индексирование для некоторых наиболее популярных типов документов, таких как PDF, HTML, электронная почта Outlook, Microsoft Office Word, рабочие листы Excel, Презентации PowerPoint, Outlook MSG, PST и многое другое. Более того, он может идентифицировать поисковые запросы, написанные на языке, который не соответствует вашей раскладке клавиатуры.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Поиск с учетом регистра в документах XHTML через Java"
      content_left: |
       GroupDocs.Search Java API включает в себя полную поддержку как базовых, так и расширенных функций поиска, что позволяет разработчикам программного обеспечения выполнять поиск с учетом регистра внутри своих Java-приложений, написав всего пару строк кода.
       
       В следующем примере кода Java показано, как добиться поиска с учетом регистра с запросом в тексте в файлах XHTML всего за пару строк кода.

      title_right: "Выполнение поиска с учетом регистра в файлах XHTML"
      content_right: |
         * Определите путь к индексной папке, а также к папке документов.
         * Создание индекса в указанной папке путем вызова экземпляра класса [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String))
         * Индексирование документов из указанной папки путем вызова экземпляра класса [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1)
         * Инициировать новый экземпляр класса [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions).
         * Включение параметра поиска с учетом регистра путем вызова метода [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch)
         * Определить поисковый запрос и начать поиск
         
        
      gisthash: "f5cba2431bcb82d746d2a002b1947d21"
      gistfile: "case-sensitive_in_text_queries_java.java"

    - title_left: "Сделать поиск с учетом регистра в форме объекта через Java"
      content_left: |
        GroupDocs.Search Java дает разработчикам программного обеспечения возможность включать функции поиска документов различных форматов в свои собственные приложения. В следующем примере кода Java показано, как выполнять поиск с учетом регистра с помощью запроса в форме объекта в документах XHTML.

      title_right: "Применить поиск с учетом регистра в документах XHTML"
      content_right: |
        * Определите путь к индексной папке, а также к папке документов.
        * Создание индекса в указанной папке путем вызова экземпляра класса [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String))
        * Индексирование документов из указанной папки путем вызова экземпляра класса [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1)
        * Инициировать новый экземпляр класса [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions).
        * Включение параметра поиска с учетом регистра путем вызова метода [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch)
        * Создание поискового запроса в объекте путем вызова метода [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String))
        * Определить поисковый запрос и начать поиск
     
      gisthash: "9e2aee884e199033f89c2c21cde108b7"
      gistfile: "case-sensitive_search_in_object_form_java.java"

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