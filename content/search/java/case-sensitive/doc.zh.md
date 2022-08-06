---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "zh/search/java/case-sensitive/doc/"
otherformats: PDF DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB FB2 

############################# Head ############################
head_title: "Java API 在 DOC 文档中执行区分大小写的文本搜索"
head_description: "GroupDocs.Search Java API 使程序员能够通过 Java 执行区分大小写的文本搜索并发现 DOC 文档中单词的确切结构。"

############################# Header ############################
title: "在 Java 应用程序中通过 DOC 文档执行区分大小写的搜索"
description: "GroupDocs.Search Java API 允许软件开发人员在 Java 应用程序中通过各种文档类型（如 PDF、HTML、DOCX、PPTX、XLSX 等）应用区分大小写的文本搜索。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "如何在 Java 应用程序中执行区分大小写的搜索？"
    content: |
      区分大小写是一种非常有用的搜索技术，它描述了程序在网络、数据库或文档搜索中区分大写（大写）和小写（小写）字母的能力。请务必记住，默认情况下搜索引擎不区分大小写，这意味着搜索单词 Computer 将给出具有键名的片段或包含单词 Computer 和 computer 的文本。假设我们需要将搜索结果缩小到带有大写字母“Computer”的搜索结果，这意味着我们需要区分大小写的搜索。 GroupDocs.Search for Java 是一个有效的文档搜索和索引 API，它使软件开发人员能够开发可以完成对一些最流行的文档类型（如 PDF、HTML、Outlook 电子邮件、Microsoft Office Word、Excel 工作表）的文本搜索和索引的应用程序， PowerPoint 演示文稿、Outlook MSG、PST 等等。此外，它可以识别以与您的键盘布局不匹配的语言编写的搜索查询。

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "通过 Java 在 DOC 文档中进行区分大小写的搜索"
      content_left: |
       GroupDocs.Search Java API 结合了对基本和高级搜索功能的完整支持，允许软件开发人员在其 Java 应用程序中进行区分大小写的搜索，只需几行代码。
       
       下面的 Java 代码示例展示了如何通过仅几行代码在 DOC 文件中的文本中进行查询来实现区分大小写的搜索。

      title_right: "在 DOC 文件中执行区分大小写的搜索"
      content_right: |
         * 确定索引文件夹和文档文件夹的路径。
         * 通过调用 [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 类的实例在指定文件夹中创建索引
         * 通过调用 [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1) 类的实例从指定文件夹索引文档
         * 启动 [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) 类的新实例
         * 通过调用 [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch) 方法启用区分大小写的搜索选项
         * 定义搜索查询并开始搜索
         
        
      gisthash: "f5cba2431bcb82d746d2a002b1947d21"
      gistfile: "case-sensitive_in_text_queries_java.java"

    - title_left: "通过 Java 以对象形式进行区分大小写的搜索"
      content_left: |
        GroupDocs.Search Java 使软件开发人员能够在他们自己的应用程序中包含各种文档格式的搜索功能。 以下 Java 代码示例演示了如何通过 DOC 文档对对象形式的查询执行区分大小写的搜索。

      title_right: "在 DOC 文档中应用区分大小写的搜索"
      content_right: |
        * 确定索引文件夹和文档文件夹的路径。
        * 通过调用 [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 类的实例在指定文件夹中创建索引
        * 通过调用 [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1) 类的实例从指定文件夹索引文档
        * 启动 [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) 类的新实例
        * 通过调用 [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch) 方法启用区分大小写的搜索选项
        * 通过调用 [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)) 方法在对象中创建搜索查询
        * 定义搜索查询并开始搜索
     
      gisthash: "9e2aee884e199033f89c2c21cde108b7"
      gistfile: "case-sensitive_search_in_object_form_java.java"

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