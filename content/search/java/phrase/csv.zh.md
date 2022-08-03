---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "zh/search/java/phrase/csv/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "在 CSV 文档中搜索和查找准确短语的 Java API"
head_description: "GroupDocs.Search Java API 帮助程序员通过 Java 在 CSV 文档的文本中嵌入短语搜索和发现给定的单词序列或确切的短语。"

############################# Header ############################
title: "如何通过 Java API 在 CSV 文档中搜索和查看准确的句子或短语？"
description: "GroupDocs.Search Java API 提供了对高级搜索功能的完整支持，使软件开发人员能够通过短语搜索或精确句子搜索在 CSV 文档中搜索出精确的句子或短语。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "什么是短语搜索以及如何在 Java 应用程序中使用它？"
    content: |
       短语搜索是在文档或网页中搜索确切句子或短语而不是关键字的一种非常有效的方法。这意味着当用户搜索一个确切的短语时，他们希望以它们出现的特定顺序查找所有搜索词。该网页将分享有关用户如何开发业务应用程序和工具以使用 Java API 进行高效文档和网页搜索的信息。 GroupDocs.Search for Java 是组织良好且高效的 Java API，它使软件开发人员能够在自己的应用程序中操作基本到高级的文本搜索操作，而无需安装任何第三方软件。该 API 包含了许多与文档搜索相关的有价值的功能，例如简单或布尔搜索、模糊搜索、区分大小写搜索、同义词、同音字、通配符、对象类型搜索、设置数据范围和其他类型的查询，以快速优雅地搜索信息。此外，它还支持识别以与您的键盘布局不匹配的语言编写的搜索查询。 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "通过 Java 在 CSV 文档中进行短语搜索"
      content_left: |
       GroupDocs.Search Java API 包含对高级搜索的完整支持，使软件专业人员能够创建具有搜索功能和易用性的强大软件应用程序。 下面的 Java 代码展示了如何用几行代码以文本和对象形式执行短语搜索。

      title_right: "CSV 文件中的精确句子搜索"
      content_right: |
         * 定义索引文件夹和文档文件夹的路径。
         * 通过调用 [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 类的实例在指定文件夹中创建索引
         * 通过调用 [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) 方法从指定文件夹索引文档
         * 通过调用 [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)) 方法进行文本查询搜索
         * 以对象形式搜索短语“短语文本”
         * 通过调用 [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)) 方法创建 word1、word2 和创建子查询 3
         * 通过调用 [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) 组合子查询来创建新的搜索查询方法
         * 开始搜索并显示搜索结果
         
        
      gisthash: "396c41cda822cf79f31dd37c6740fa03"
      gistfile: "phrase_search_in_text_queries_java.java"

    - title_left: "通过 Java 通过 CSV 文件应用通配符短语搜索"
      content_left: |
        GroupDocs.Search for Java 使软件程序员能够在 Java 应用程序中搜索 CSV 文件时添加通配符短语搜索功能。 以下 Java 代码示例演示了如何使用 Java API 在各种文档类型中应用通配符短语搜索。

      title_right: "在 Java 中使用通配符进行短语搜索"
      content_right: |
        * 定义索引文件夹和文档文件夹的路径。
        * 通过调用 [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 类的实例在指定文件夹中创建索引
        * 通过调用 [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) 方法从指定文件夹索引文档
        * 通过调用 [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)) 方法进行文本查询搜索
        * 以对象形式搜索短语“短语文本”
        * 通过调用 [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)) 方法创建 word1 和 word3
        * 通过调用 [createWildcardQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWildcardQuery(int,%20int)) 方法创建通配符2
        * 通过调用 [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) 组合子查询来创建新的短语搜索查询） 方法
        * 开始搜索并显示搜索结果
     
      gisthash: "f21c8c4572883fecc0eeef82c2b814b1"
      gistfile: "use_wildcards_in_phrase_search_java.java"
      
    - title_left: "用于组合短语搜索和其他类型搜索的 Java API"
      content_left: |
        GroupDocs.Search Java API 允许软件程序员轻松地将短语搜索与其他类型的搜索结合起来。 以下 Java 代码显示了如何通过表示单词和单词中字符的通配符执行短语搜索。

      title_right: "如何结合短语搜索和其他搜索"
      content_right: |
        * 定义索引文件夹和文档文件夹的路径。
        * 通过调用 [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 类的实例在指定文件夹中创建索引
        * 通过调用 [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) 方法从指定文件夹索引文档
        * 通过调用 [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)) 方法进行文本查询搜索
        * 以对象形式搜索短语“短语文本”
        * 定义字模式并附加字符串并附加通配符
        * 通过调用 [CreateWordPatternQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordPatternQuery(com.groupdocs.search.common.WordPattern)) 方法创建 wordPattern1 和创建 word3
        * 通过调用 [createWildcardQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWildcardQuery(int,%20int)) 方法创建通配符2
        * 通过调用 [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) 组合子查询来创建新的短语搜索查询） 方法
        * 开始搜索并显示搜索结果
     
      gisthash: "dbd0f2eb292796e63e6213461f080e0c"
      gistfile: "combine_phrase_search_with_others_java.java"

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