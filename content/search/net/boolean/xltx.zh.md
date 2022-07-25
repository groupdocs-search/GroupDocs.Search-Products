---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "zh/search/net/boolean/xltx/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "通过 .NET 在搜索查询中添加布尔搜索运算符（AND、OR、NOT）"
head_description: "GroupDocs.Search .NET API 使软件开发人员能够在其 .NET 应用程序中添加布尔搜索或使用布尔运算符 AND、OR、NOT 开发新查询。"

############################# Header ############################
title: "在 .NET 应用程序中使用布尔运算符 AND、OR、NOT 开发复杂的搜索查询"
description: "GroupDocs.Search .NET API 允许计算机程序员在其 .NET 应用程序中使用布尔运算符（AND、OR、NOT）开发复杂的搜索查询。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "什么是布尔搜索以及如何使用布尔运算符？"
    content: |
       布尔搜索是一个非常有用的搜索过程，它允许用户将不同的关键字与运算符结合起来，以绑定、扩大和定义搜索结果。 AND、OR、NOT 和 NEAR 等布尔运算符可帮助用户获得更广泛的结果，或通过定义限制来减少不相关的搜索结果的数量。 GroupDocs.Search for .NET 是功能强大的高性能文档搜索 API，它使软件开发人员能够开发可以在一些最常见的文档文件格式（如 PDF、HTML、Outlook 电子邮件、Microsoft Office Word、Excel 工作表）上完成文本搜索和索引的应用程序、PowerPoint 演示文稿、Outlook MSG、PST 等等。布尔 AND 运算符可用于显示您输入的所有单词的结果，OR 运算符为您输入的任何单词提供结果，NOT 运算符可用于显示没有出现的搜索结果等等。一个很棒的功能是它可以识别以与您的键盘布局不匹配的语言编写的搜索查询。

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "通过 .NET 在搜索查询中使用布尔 AND 运算符"
      content_left: |
       GroupDocs.Search .NET API 完全支持在其 .NET 应用程序中添加布尔搜索功能。 下面的 C# 代码示例显示了如何在他们自己的 .NET 应用程序中的文本和对象表单查询中创建布尔“AND”运算符。

      title_right: "通过布尔运算符 AND 搜索 XLTX 文档"
      content_right: |
         * 首先，您需要指定索引文件夹和文档文件夹的路径。
         * 通过调用 [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 类的实例在指定文件夹中创建索引
         * 通过调用 [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)方法从指定文件夹索引文档
         * 通过调用 [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery) 类创建子查询 1 和创建子查询 2
         * 通过调用 [CreateAndQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) 方法将子查询合并为一个查询
         * 开始搜索并显示搜索结果
         
        
      gisthash: "fa9773cd8d0f379a638e495ad2541a5b"
      gistfile: "use_boolean_and_operator_dotnet.cs"

    - title_left: "如何使用布尔运算符或通过 .NET"
      content_left: |
       GroupDocs.Search for .NET 是一个强大的 API，它使软件程序员能够搜索许多流行的文档格式。 下面的 C# .NET 代码示例展示了如何在 C# 应用程序内的文本和对象表单查询中使用布尔“或”运算符。

      title_right: "使用布尔 OR 运算符搜索 XLTX 文件"
      content_right: |
        * 首先，您需要指定索引文件夹和文档文件夹的路径。
        * 通过调用 [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 类的实例在指定文件夹中创建索引
        * 通过调用 [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)方法从指定文件夹索引文档
        * 通过调用 [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery) 类创建子查询 1 和创建子查询 2
        * 通过调用 [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery) 方法将子查询合并为一个查询
        * 开始搜索并显示搜索结果
     
      gisthash: "c0b22e80f881f8dbc0da17f92c01efc7"
      gistfile: "use_boolean_or_operator_dotnet.cs"
      
    - title_left: "使用布尔运算符创建复杂的搜索查询"
      content_left: |
       GroupDocs.Search .NET 使计算机程序员能够结合不同的布尔运算符在他们自己的 .NET 应用程序中创建复杂的搜索查询。 以下 .NET 代码示例展示了如何在不安装任何外部软件或工具的情况下实现复杂的文档搜索功能。

      title_right: "通过复杂的搜索查询搜索 XLTX 文档"
      content_right: |
        * 首先，您需要指定索引文件夹和文档文件夹的路径。
        * 通过调用 [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 类的实例在指定文件夹中创建索引
        * 通过调用 [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)方法从指定文件夹索引文档
        * 开始搜索并显示搜索结果文本查询
        * 使用对象查询进行搜索
        * 通过调用 [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery) 类创建 WordQuery 和 relativityWordQuery
        * 通过调用 [CreateAndQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) 方法将子查询合并为一个查询
        * 通过调用 [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery) 类创建 einsteinWordQuery 和 albertWordQuery
        * 通过调用 [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery) 方法将子查询合并为一个查询
        * 通过调用 [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery) 方法将子查询合并为一个查询
        * 开始搜索并显示搜索结果
     
      gisthash: "216af02ebdd08331fdd05faf8c39e528"
      gistfile: "create_complex_queries_boolean_operator_dotnet.cs"

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