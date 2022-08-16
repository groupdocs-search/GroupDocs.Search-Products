---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "zh/search/java/filters/ppsm/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "通过 Java API 在搜索结果中集成 PPSM 文档过滤？"
head_description: "GroupDocs.Search Java API 帮助软件开发人员添加 PPSM 文档搜索功能并应用文档过滤以通过 Java API 自定义搜索结果。"

############################# Header ############################
title: "如何集成文档过滤以自定义 Java 应用程序中的搜索结果"
description: "GroupDocs.Search Java API 允许程序员集成高级 PPSM 文档搜索功能，并通过在其 Java 应用程序中设置文档过滤来自定义搜索结果。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "如何集成文档过滤以自定义 Java 应用程序中的搜索结果"
    content: |
       文档过滤是一项非常有用的活动，它使软件应用程序能够根据用户在索引文档文本中输入的相关单词序列来搜索和检索文档。过滤器包含一组规则，这些规则定义了用于选择记录的标准。文档过滤使用户能够将他们的搜索限制在特定部分或特定文档类型，以及浏览结果并找到他们正在寻找的内容。 GroupDocs.Search for Java 是功能丰富的高性能文档索引和搜索 API，使软件开发人员能够创建可以实现文本索引和搜索一些最流行的文档文件格式的应用程序。它完全支持各种文档类型，如 PDF、HTML、Outlook 电子邮件、Microsoft Office Word、Excel 工作表、PowerPoint 演示文稿、Outlook MSG、PST 等。有多种过滤器可供用户自定义搜索结果，例如文件路径过滤器、文件扩展名过滤器、属性过滤器等等。

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "在通过 Java 搜索 PPSM 文档时应用文档过滤器"
      content_left: |
       GroupDocs.Search Java API 帮助软件开发人员使用 Java API 创建具有搜索功能的强大应用程序。 下面的 Java 代码示例展示了如何应用文档过滤器来搜索各种类型的文档，只需几行代码。

      title_right: "搜索 PPSM 文档中的文档过滤器设置"
      content_right: |
       * 首先，您需要指定索引文件夹和文档文件夹的路径。
       * 通过调用 [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 类的实例在指定文件夹中创建索引
       * 通过调用 [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) 方法从指定文件夹索引文档
       * 通过调用 [earchOptions](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions) 类创建搜索选项对象
       * 通过调用 [setSearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter)) 方法设置文档过滤器
       * 开始搜索并显示文本文档（如果找到）
        
      gisthash: "6ad4038623777576484491239ce17125"
      gistfile: "set_document_filter_in_search_java.java"

    - title_left: "组合搜索文档过滤器以通过 Java 创建复合过滤器"
      content_left: |
        GroupDocs.Search for Java 允许软件程序员添加高级搜索功能并在其 Java 应用程序内应用自定义过滤器进行文档搜索。 用户可以通过组合各种类型的搜索过滤器来创建复合过滤器。 以下 Java 代码演示了如何使用布尔运算符 AND、OR、NOT 等组合搜索文档过滤器以创建复合过滤器，只需几行代码。

      title_right: "创建复合过滤器以搜索 PPSM 文件"
      content_right: |
       * 首先，您需要指定索引文件夹和文档文件夹的路径。
       * 创建一个 AND 复合过滤器，返回所有在其完整路径中包含单词“Einstein”的 FB2 和 EPUB 文档
       * 通过调用 [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter)) 创建 filter1
       * 通过调用 [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter)) 创建 filter2
       * 通过调用 [createAnd](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createAnd(com.groupdocs.search.options.ISearchDocumentFilter...)) 方法组合过滤器
       * 创建一个 OR 复合过滤器，返回所有 DOC、DOCX、PDF 和所有在其完整路径中包含单词 Einstein 的文档
       * 通过调用 [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter)) 创建 filter3
       * 通过调用 [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter)) 创建 filter4
       * 通过调用 [createOr](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createOr(com.groupdocs.search.options.ISearchDocumentFilter...)) 方法组合过滤器
       * 创建一个过滤器，返回除 TXT 文档之外的所有找到的文档
       * 通过调用 [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter)) 创建 filter4
       * Appy 不通过调用 [createNot](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createNot(com.groupdocs.search.options.ISearchDocumentFilter)) 方法进行过滤

      gisthash: "db9ab9384dcacb90c5bbdad98a2d2cba"
      gistfile: "combine_document_filter_in_search_java.java"
      
    - title_left: "系统要求"
      content_left: |
       所有主要平台和操作系统都支持 GroupDocs.Search for Java。 如需完整的系统要求指南，请在执行以下代码之前访问 [系统要求](https://docs.groupdocs.com/search/java/system-requirements/)，请确保您已安装以下先决条件 系统：
        * 操作系统：Microsoft Windows、Linux、MacOS
        * Java 版本支持：J2SE 7.0 (1.7)、J2SE 8.0 (1.8) 或以上
        * 获取最新版本的 GroupDocs.Search for Java APIs from GroupDocs [Repository](https://repository.groupdocs.com/repo/com/groupdocs/groupdocs-search/)
        
      title_right: "为什么使用 GroupDocs.Search"
      content_right: |
        * 在内存和磁盘上创建搜索索引。
        * 从文件、流或结构索引的能力。
        *受密码保护的文档索引支持。
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