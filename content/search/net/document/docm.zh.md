---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "zh/search/net/document/docm/"
otherformats: PDF DOC DOT DOCX DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "在 .NET 应用程序中创建和添加文档搜索和索引"
head_description: "GroupDocs.Search .NET API 允许在 .NET 应用程序中添加即时文档搜索支持格式，如 PDF DOC、DOCX、RTF、XLSX、CSV、PPTX 和电子邮件消息。"

############################# Header ############################
title: "如何通过 C# .NET API 将即时文档搜索添加到 DOCM"
description: "GroupDocs.Search .NET API 允许开发人员向他们的应用程序添加强大的文档搜索和索引功能。 它支持 PDF DOC、DOCX、RTF、XLSX、CSV、PPT、PPTX、MSG、EML 等文档。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "如何使用 .NET API 创建和添加文档搜索和索引？"
    content: |
       此页面将帮助用户了解如何在自己的应用程序中添加文档搜索和索引功能，而无需付出任何努力和成本。索引是搜索引擎使用的过程，通过该过程组织和结构化数据，以便生成相关的搜索结果。目的是快速准确地查找和显示与用户查询相关的信息。 GroupDocs.Search for .NET 是功能强大的高性能文档搜索 API，它使软件开发人员能够在他们自己的应用程序中基于模糊和同义词算法执行高级搜索和索引操作。它不需要在用户的机器上安装任何第三方工具或外部软件。它支持一些最常用的文档格式，例如 PDF、HTML、Outlook 电子邮件、Microsoft Office Word、Excel 工作表、PowerPoint 演示文稿、Outlook MSG、PST 等等。支持简单词、布尔、正则表达式搜索、区分大小写搜索、灵活模糊、同义词、同音字、通配符、分块搜索、对象类型搜索、设置数据范围等多种搜索。

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "通过 .NET API 为 DOCM 文档创建搜索索引"
      content_left: |
       GroupDocs.Search .NET API 为在您自己的应用程序中创建新索引或打开现有搜索索引提供了完整支持。 下面的 C# 代码示例展示了如何仅使用几行代码来创建新索引和打开现有索引。 

      title_right: "如何创建新的或打开现有的搜索索引"
      content_right: |
         * 首先，您需要指定索引文件夹的路径
         * 创建 [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 类的实例
         * 以上将在内存或磁盘上创建索引，也可以打开现有索引。
       
      gisthash: "9651c19a9436afee860b7f39197f8399"
      gistfile: "create_or_open_new_search_index.cs"

    - title_left: "如何将 DOCM 文档同步添加到搜索索引"
      content_left: |
       GroupDocs.Search .NET 允许软件开发人员在他们自己的 .NET 应用程序中同步执行文档索引。 下面的 C# .NET 代码示例展示了如何轻松地同步执行索引。

      title_right: "通过 C# 同步文档索引"
      content_right: |
        * 首先，您需要指定索引文件夹的路径
        * 指定包含要搜索的文档的文件夹的路径
        * 创建 [Index(indexFolder)](https://apireference.groupdocs.com/search/net/groupdocs.search.indexrepository/search/methods/2) 类的实例
        * 以上将在内存或磁盘上创建索引或打开现有索引。
        * 从指定文件夹同步索引文档
     
      gisthash: "1c5f672c83e741280fd24c58fe51f707"
      gistfile: "add_files_synchronously_to_indexing.cs"
      
    - title_left: "通过 .NET 异步执行文档索引"
      content_left: |
        GroupDocs.Search .NET 使计算机程序员能够在他们自己的 .NET 应用程序中执行异步文档索引。 下面的 .NET 代码示例展示了如何通过几行代码实现异步文档索引。

      title_right: "通过 C# 异步 DOCM 文档索引"
      content_right: |
        * 首先，您需要指定索引文件夹的路径
        * 指定包含要搜索的文档的文件夹的路径
        * 创建 [Index(indexFolder)](https://apireference.groupdocs.com/search/net/groupdocs.search.indexrepository/search/methods/2) 类的实例
        * 订阅活动
        * 需要编写代码指示操作完成
        * 设置异步索引的标志
        * 从指定文件夹异步索引文档
     
      gisthash: "1c5f672c83e741280fd24c58fe51f707"
      gistfile: "add_files_asynchronously_to_indexing.cs"

    - title_left: "如何在 DOCM Docs .NET 中使用和突出显示搜索结果"
      content_left: |
       GroupDocs.Search .NET API 允许程序员解释搜索结果并通过找到的文档的简单列表或找到的单词和短语来显示结果。 您还可以轻松突出显示文档的文本。 以下 .NET 代码示例展示了如何仅用几行代码列出找到的文档并突出显示搜索结果。

      title_right: "通过 C# 在 DOCM 文件中突出显示搜索结果 "
      content_right: |
        * 在索引中执行搜索
        * 搜索成功后，打印结果
        * 遍历文档并显示找到的文档
        * 突出显示文本中的出现
        * 生成带有突出显示的搜索结果的输出 HTML 格式文档
     
      gisthash: "a5d1ad6eedd2acf12a33b541e763cdb4"
      gistfile: "how_to_list_search_result.cs"

    - title_left: "系统要求"
      content_left: |
       所有主要平台和操作系统都支持 GroupDocs.Search for .NET。 如需完整的系统要求指南，请在执行以下代码之前访问 [系统要求](https://docs.groupdocs.com/search/net/system-requirements/)，请确保您已安装以下先决条件 系统：
         * 操作系统：Microsoft Windows、Linux、MacOS
         * 开发环境：Visual Studio、Xamarin、MonoDevelop 等
         * 框架：.NET Framework、.NET Standard、.NET Core、Mono
         * 获取最新版本的 GroupDocs。从 [NuGet](https://www.nuget.org/packages/GroupDocs.search/) 搜索 .NET API
        
      title_right: "为什么使用 GroupDocs.Assembly"
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