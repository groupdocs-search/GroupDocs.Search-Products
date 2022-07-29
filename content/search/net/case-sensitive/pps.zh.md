---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "zh/search/net/case-sensitive/pps/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "通过 .NET 通过 PPS 文档应用区分大小写的文本搜索"
head_description: "GroupDocs.Search .NET API 使软件程序员能够应用区分大小写的文本搜索并通过 .NET API 查找 PPS 文档中的确切单词序列。"

############################# Header ############################
title: "如何通过 .NET 应用程序中的 PPS 文档应用区分大小写的搜索？"
description: "GroupDocs.Search .NET API 允许软件开发人员在 .NET 应用程序中通过各种文档类型（如 PDF、HTML、DOCX、PPTX、XLSX 等）应用区分大小写的文本搜索。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "W帽子是区分大小写的搜索以及如何通过.NET 实现它？"
    content: |
      有许多有用的搜索技术可以帮助用户在各种类型的文档中搜索单词或其他数据的特定组合。区分大小写搜索是一种非常有用的技术，它允许用户搜索文档和网页，无论大小写字母被视为不同还是相同。例如，“Computer”、“computer”和“COMPUTER”将被视为不同的单词，因为字母“C”在第一个实例中是大写的，第二个是小写的，第三个是全部大写的。 GroupDocs.Search for .NET 是方便的高性能文档搜索 API，它使软件创建者能够制作软件应用程序和工具，以轻松完成文本搜索和文档索引。 API 支持一些最常用的文件格式，例如 PDF、HTML、Outlook 电子邮件、Microsoft Office Word、Excel 工作表、PowerPoint 演示文稿、Outlook MSG、PST 等等。另一个有用的功能是它可以识别以与您的键盘布局不匹配的语言编写的搜索查询。

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "通过 .NET 在 PPS 文档中执行区分大小写的搜索"
      content_left: |
       GroupDocs.Search .NET API 使软件程序员能够在他们自己的 C# .NET 应用程序中添加区分大小写的搜索功能。 下面的 .NET 代码示例说明了如何使用 PPS 文件中的文本形式的查询来实现区分大小写的搜索，只需几行代码。

      title_right: "在 PPS 文档中应用区分大小写的搜索"
      content_right: |
         * 确定索引文件夹和文档文件夹的路径。
         * 通过调用[Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)类的实例在指定文件夹中生成索引
         * 通过调用 [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1) 类的实例从指定文件夹索引文档
         * 初始化 [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) 类的新实例
         * 通过调用 [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch) 方法启用区分大小写的搜索
         * 定义搜索字符串并开始搜索
         
        
      gisthash: "805df69ebb1145d5c15c212431de1395"
      gistfile: "case-sensitive_in_text_queries_dotnet.cs"

    - title_left: "通过 .NET 以对象形式执行区分大小写的搜索"
      content_left: |
        GroupDocs.Search .NET 使软件开发人员能够在 .NET 应用程序中发现记住大写和小写字母的单词。 以下 .NET 代码示例说明了如何在 PPS 文档中对对象形式的查询应用区分大小写的搜索。 

      title_right: "在 PPS 文档中进行区分大小写的搜索"
      content_right: |
        * 确定索引文件夹和文档文件夹的路径。
        * 通过调用[Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)类的实例在指定文件夹中生成索引
        * 通过调用 [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1) 类的实例从指定文件夹索引文档
        * 初始化 [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) 类的新实例
        * 通过调用 [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch) 方法启用区分大小写的搜索
        * 通过调用 [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery) 方法以对象形式创建搜索查询
        * 开始搜索并显示搜索结果
     
      gisthash: "846d0dd11f88a59d62f083e33e84286b"
      gistfile: "case-sensitive_search_in_object_queries_dotnet.cs"

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