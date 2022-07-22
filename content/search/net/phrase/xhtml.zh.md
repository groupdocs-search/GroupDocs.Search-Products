---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "zh/search/net/phrase /xhtml/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP  MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "如何在 .NET 应用程序的 XHTML 文档中添加短语搜索？"
head_description: "GroupDocs.Search .NET API 使软件专业人士能够通过 .NET API 添加短语搜索并在 XHTML 文档中找到确切的短语或提供的单词序列。"

############################# Header ############################
title: "在 .NET 应用程序内的 XHTML 文档中添加精确句子或短语搜索？"
description: "GroupDocs.Search .NET API 允许程序员通过短语搜索或 .NET 应用程序中的精确句子搜索来找出 XHTML 文档中提供的单词序列。 "

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "如何在 .NET 应用程序中使用精确的句子或短语搜索？"
    content: |
       精确句子或短语搜索是一种搜索，它使用户能够搜索出具有精确句子或短语的文档、网络或数据库，其中包含由消费者定义的特定顺序和单词组合。 它是搜索引擎术语中非常常见的术语，允许用户在索引文档的文本中搜索指定单词序列的文档。 GroupDocs.Search for .NET 是一个非常有用的高性能文档和文本搜索 API，它为开发文本搜索和索引应用程序提供了完整的功能，支持一些最常见的文档类型，如 PDF、HTML、Outlook 电子邮件、Microsoft Office Word、 Excel 工作表、PowerPoint 演示文稿、Outlook MSG、PST 等。 它包括对与短语搜索相关的多项功能的支持，例如以文本和对象形式搜索查询、在短语搜索中使用通配符等。 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "如何通过 .NET 在 XHTML 文档中执行短语搜索"
      content_left: |
       GroupDocs.Search .NET API 使软件开发人员能够在他们自己的 C# .NET 应用程序中添加短语搜索功能。 下面的 .NET 代码示例演示了如何仅用几行代码在文本和对象中执行短语搜索。

      title_right: "XHTML 文档中的精确短语搜索"
      content_right: |
         * 首先，您需要指定索引文件夹和文档文件夹的路径。
         * 通过调用 [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 类的实例在指定文件夹中创建索引
         * 通过调用[Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)方法从指定文件夹索引文档
         * 以文本形式搜索词组查询“词组文本”
         * 以对象形式搜索短语“短语文本”
         * 通过调用 [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery) 方法创建 word1、word2 和创建子查询 3
         * 通过调用 [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery) 方法组合子查询创建新的搜索查询
         * 开始搜索并显示搜索结果
        
      gisthash: "a5696884acf504acc319ba97465248cd"
      gistfile: "phrase_search_in_text_queries_dotnet.cs"

    - title_left: "通过 .NET 在 XHTML 文档中搜索通配符短语"
      content_left: |
        GroupDocs.Search for .NET 使软件程序员能够在 C# .NET 应用程序中使用通配符添加短语搜索功能。 以下 .NET 代码示例展示了如何在 C# 应用程序中的 XHTML 文档中应用通配符短语搜索。
      title_right: "在 XHTML 文件中应用通配符短语搜索"
      content_right: |
        * 首先，您需要指定索引文件夹和文档文件夹的路径。
        * 通过调用 [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 类的实例在指定文件夹中创建索引
        * 通过调用[Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)方法从指定文件夹索引文档
        * 以文本形式搜索词组查询“词组文本”
        * 以对象形式搜索短语“短语文本”
        * 通过调用 [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery) 方法创建 word1 和创建子查询 3
        * 通过调用 [CreateWildcardQuery](https://apireference.groupdocs.com/search/net/groupdocs.search.searchquery/createwildcardquery/methods/1) 方法创建通配符2
        * 通过调用 [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery) 方法组合子查询创建新的搜索查询
        * 开始搜索并显示搜索结果
     
      gisthash: "3ff2bf9f8ba902d8d7ebead67a934654"
      gistfile: "use_wildcards_in_phrase_search_dotnet.cs"
      
    - title_left: "通过 .NET 将短语搜索与其他类型的搜索相结合"
      content_left: |
        GroupDocs.Search .NET 使软件程序员能够将短语搜索与 .NET 应用程序内的其他类型的搜索结合起来。 以下 .NET 代码示例显示了如何应用表示单词和单词中字符的通配符。

      title_right: ".NET API 将短语搜索与其他搜索结合起来"
      content_right: |
        * 首先，您需要指定索引文件夹和文档文件夹的路径。
        * 通过调用 [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 类的实例在指定文件夹中创建索引
        * 通过调用[Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)方法从指定文件夹索引文档
        * 以文本形式搜索词组
        * 以对象形式搜索短语
        * 定义字模式并附加字符串。
        * 通过调用 [CreateWordPatternQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordpatternquery) 方法创建 wordPattern1 和创建 word3
        * 通过调用 [CreateWildcardQuery](https://apireference.groupdocs.com/search/net/groupdocs.search.searchquery/createwildcardquery/methods/1) 方法创建通配符2
        * 通过调用 [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery) 方法组合子查询创建新的搜索查询
        * 开始搜索并显示搜索结果
     
      gisthash: "db5c32ed21237f3e1cd7cdbde0778c29"
      gistfile: "combine_phrase_search_with_others_dotnet.cs"

    - title_left: "系统要求"
      content_left: |
       所有主要平台和操作系统都支持 GroupDocs.Search for .NET。 如需完整的系统要求指南，请在执行以下代码之前访问 [系统要求](https://docs.groupdocs.com/search/net/system-requirements/)，请确保您已安装以下先决条件 系统：
         * 操作系统：Microsoft Windows、Linux、MacOS
         * 开发环境：Visual Studio、Xamarin、MonoDevelop 等
         * 框架：.NET Framework、.NET Standard、.NET Core、Mono
         * 获取最新版本的 GroupDocs.Search 从 [NuGet](https://www.nuget.org/packages/GroupDocs.search/) 搜索 .NET API
        
      title_right: "为什么使用 GroupDocs.Search"
      content_right: |
        * 在内存和磁盘上创建搜索索引。
        * 从文件、流或结构索引的能力。
        * 受密码保护的文档索引支持。
        * 支持合并多个索引。
        * 在搜索索引期间过滤文档。
        * 搜索期间的拼写检查支持。
        * 完全支持混合字符
        * 将不同类型的搜索组合到一个搜索查询中。
        * 简单的单词和正则表达式搜索支持
        * 完全支持搜索查询中的别名替换。

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---