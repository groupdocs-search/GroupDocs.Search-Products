---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "zh/search/java/document/eml"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "在 Java 应用程序中添加文档索引和搜索操作"
head_description: "GroupDocs.Search Java API 支持 PDF DOC、DOCX、RTF、XLSX、CSV、PPTX、EML、MSG 等文档格式的文档索引和搜索操作。"

############################# Header ############################
title: "EML 文档索引和搜索操作的 java API"
description: "GroupDocs.Search Java API 允许开发人员将强大的文档搜索和索引操作集成到他们的应用程序中。 它支持 PDF DOC、DOCX、RTF、XLSX、CSV、PPTX MSG、EML 等文件格式。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "如何在 Java APP 中添加文档索引和搜索操作"
    content: |
       数据和信息量与日俱增。因此，以最小的成本和努力及时检索正确的信息非常重要。该网页将提供有关用户如何开发高效文档搜索功能并将其添加到其业务应用程序的信息。 .目的是快速准确地查找和显示与用户查询相关的信息。 GroupDocs.Search for Java 是非常高效且易于使用的 Java API，可帮助软件开发人员在自己的应用程序中操作基本到高级的文本搜索操作，而无需安装任何第三方软件。 Java API 提供了一些与搜索相关的有用功能，例如将多个索引合并为一个公共索引、对不同键盘布局的搜索查询识别、形态学 Word Form 支持等。它支持简单、布尔、正则表达式（Regex）、模糊、区分大小写搜索、同义词、同音字、通配符、对象类型搜索、设置数据范围等类型的查询，快速优雅地搜索出信息。

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "通过 Java 创建新的搜索索引或加载现有索引"
      content_left: |
       GroupDocs.Search Java 使软件开发人员能够生成新的搜索索引或在他们自己的 Java 应用程序中加载现有的搜索索引。 下面的 Java 代码示例显示了创建新索引以及仅使用几行 Java 代码加载现有索引。

      title_right: "通过 Java 创建新的或加载现有的搜索索引"
      content_right: |
         * 首先您需要指定索引文件夹的路径
         * 创建 [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 类的实例
         * 以上将在内存或磁盘上创建索引，也可以加载现有索引。
       
      gisthash: "02615fe51a919acdc5363d46c181dc7f"
      gistfile: "create_or_load_search_index.java"

    - title_left: "通过 Java 同步 EML 文档索引"
      content_left: |
       GroupDocs.Search Java API 帮助软件程序员在他们自己的 Java 应用程序中只用几行代码就可以同步索引文档。 下面的 Java 代码示例演示了如何轻松地同步执行文档索引。 

      title_right: "将 EML 文档添加到同步搜索索引"
      content_right: |
        * 首先您需要指定索引文件夹的路径
        * 指定包含要搜索的文档的文件夹的路径
        * 创建 [Index(indexFolder)](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 类的实例
        * 以上将在内存或磁盘上创建索引或打开现有索引。
        * 从指定文件夹同步索引文档
     
      gisthash: "7079bf3c06128a69b842150d080e5e0b"
      gistfile: "Add_files_synchronously_to_indexing.java"
      
    - title_left: "通过 Java 执行异步文档索引"
      content_left: |
        GroupDocs.Search Java API 允许软件专业人员在他们自己的 Java 应用程序中执行异步文档索引。 下面的 java 代码演示了开发人员如何只用几行 java 代码就可以异步索引文档。

      title_right: "异步添加 EML 文档到搜索索引"
      content_right: |
        * 首先您需要指定索引文件夹的路径
        * 指定包含要搜索的文档的文件夹的路径
        * 创建 [Index(indexFolder)](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 类的实例
        * 订阅活动
        * 需要编写代码指示操作完成
        * 设置异步索引的标志
        * 从指定文件夹异步索引文档
     
      gisthash: "7079bf3c06128a69b842150d080e5e0b"
      gistfile: "Add_files_asynchronously_to_indexing.java"

    - title_left: "如何在 Java 应用程序中突出显示搜索结果"
      content_left: |
       GroupDocs.Search Java API 允许开发人员解释搜索结果并列出找到的文档以及单词和短语。 也可以突出显示 EML 文档的文本。 下面的 Java 代码示例演示了如何仅用几行代码列出找到的文档并突出显示搜索结果。

      title_right: "通过 Java 突出显示搜索结果"
      content_right: |
        * 在索引中执行搜索
        * 搜索成功后，打印结果
        * 遍历文档并显示找到的文档
        * 突出显示文本中的出现
        * 生成带有突出显示的搜索结果的输出 HTML 格式文档
     
      gisthash: "cc88d485f007d6da0d943043c8e13a52"
      gistfile: "how_to_highlight_search_result.java"

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