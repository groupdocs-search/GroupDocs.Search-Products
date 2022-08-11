---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "zh/search/net/filters/one/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "通过在 .NET 应用程序中设置文档过滤来自定义搜索结果"
head_description: "GroupDocs.Search .NET API 允许软件开发人员搜索 ONE Documents 文档并通过在 .NET 应用程序中应用文档过滤来自定义搜索结果。"

############################# Header ############################
title: "设置文档过滤以自定义 .NET 应用程序中的搜索结果"
description: "GroupDocs.Search .NET API 帮助软件专业人士添加文档搜索功能并通过在其 .NET 应用程序中应用文档过滤来自定义搜索结果。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "如何通过 .NET 在搜索结果中应用文档过滤？"
    content: |
       过滤是一种非常有用的技术，它使用户能够检查和处理功能。 文档过滤为用户提供了一种轻松导航结果和查找所需内容的方法。 它还赋予用户将搜索限制在特定部分或特定文档类型的权力。 GroupDocs.Search for .NET 是功能丰富的高性能文档搜索 API，使软件开发人员能够构建可以实现文本搜索和索引的应用程序。 它支持一些最流行的文档格式，例如 PDF、HTML、Outlook 电子邮件、Microsoft Office Word、Excel 工作表、PowerPoint 演示文稿、Outlook MSG、PST 等等。 API 完全支持为搜索结果设置文档归档。 您可以使用多种文件管理器来自定义搜索结果，例如文件路径过滤器、文件扩展名过滤器、属性过滤器等等。 也可以通过使用布尔运算符 AND、OR & NOT 等来组合搜索文档过滤器。

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "在通过 .NET 搜索 ONE 文档时设置文档过滤器"
      content_left: |
       GroupDocs.Search .NET API 帮助软件开发人员在他们的 .NET 应用程序中添加搜索功能。 下面的 .NET 代码示例演示了如何应用文档过滤器来搜索各种类型的文档，只需几行代码。

      title_right: "在搜索 ONE 文档时应用文档过滤器"
      content_right: |
       * 首先，您需要指定索引文件夹和文档文件夹的路径。
       * 通过调用 [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 类的实例在指定文件夹中创建索引
       * 通过调用[Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)方法从指定文件夹索引文档
       * 创建搜索选项对象 [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions)
       * 通过调用[SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter) 设置文档过滤器
       * 开始搜索并显示搜索结果
        
      gisthash: "77cafabe4e9c9256217b4326e26a59d0"
      gistfile: "set_document_filter_in_search_dotnet.cs"

    - title_left: "如何通过 .NET 组合搜索文档过滤器"
      content_left: |
        GroupDocs.Search for .NET 允许软件程序员在搜索时组合搜索文档过滤器，以控制在 C# .NET 应用程序内部搜索时应返回找到的哪些文档。 以下 .NET 代码示例展示了如何在 C# 应用程序中使用布尔运算符 AND、OR、NOT 等组合搜索文档过滤器。 

      title_right: "在搜索 ONE 文件时组合搜索文档过滤器"
      content_right: |
       * 首先，您需要指定索引文件夹和文档文件夹的路径。
       * 创建一个 AND 复合过滤器，返回所有在其完整路径中包含单词“Einstein”的 FB2 和 EPUB 文档
       * 通过调用[SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter) 创建filter1
       * 通过调用[SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter) 创建filter2
       * 通过调用 [andFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createand) 方法组合过滤器
       * 创建一个 OR 复合过滤器，返回所有 DOC、DOCX、PDF 和所有在其完整路径中包含单词 Einstein 的文档
       * 通过调用[SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter) 创建filter3
       * 通过调用[SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter) 创建filter4
       * 通过调用 [orFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createor) 方法组合过滤器
       * 创建一个过滤器，返回除 TXT 文档之外的所有找到的文档
       * 通过调用[SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter) 创建filter4
       * Appy 不通过调用 [notFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createnot) 方法进行过滤

      gisthash: "db4efe513cbd34925231be10a992f23c"
      gistfile: "combine_document_filter_in_search_dotnet.cs"
      
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