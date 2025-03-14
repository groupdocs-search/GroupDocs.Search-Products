
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: zh
format: Pptx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "使用适用于Java的GroupDocs.Search在PPTX文档中查找文本"
head_description: "GroupDocs.Search for Java 帮助 Java 开发者快速在各种文档格式中搜索文本。"

############################# Header ############################
title: "智能文档文本搜索" 
description: "使用 GroupDocs.Search for Java，您可以在您的 Java 应用程序中无缝搜索和提取多种文档类型的文本。"
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "获取免费试用"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search 是做什么的？"
    link: "/search/java/"
    link_title: "了解更多"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) 是一个强大的文档搜索和索引库，支持超过 70 种文件格式，包括 PDF、Word、PowerPoint、Excel、图像和 ZIP 压缩档案。它为大规模文档集合提供快速、精确和可扩展的搜索功能。

############################# Steps ############################
steps:
    enable: true
    title: "在 PPTX 文件中执行文本搜索"
    content: |
      [GroupDocs.Search](/search/java/) 使得在 PPTX 文件中使用复杂的逻辑和索引进行搜索变得简单，从而提高 Java 应用程序中的搜索准确性。
      
      1. 设置一个目录以存储搜索索引。
      2. 选择一个包含 PPTX 文件的文件夹。
      3. 定义额外的搜索选项。
      4. 执行搜索并分析结果。
   
    code:
      platform: "java"
      copy_title: "复制"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "搜索结果"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-search</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "点击复制"
        copy_done: "已复制"
      links:
        #  loop
        - title: "更多示例"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "文档"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // 设置用于存储搜索索引的目录
        Index index = new Index("c:/MyIndex");

        // 指定包含可搜索文档的文件夹
        index.add("c:/MyDocuments");

        // 启用同音词搜索以匹配发音相似的单词
        SearchOptions options = new SearchOptions();
        options.setUseHomophoneSearch(true);

        // 执行高级搜索查询
        SearchResult result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "增强的搜索和索引能力"
  description: "GroupDocs.Search for Java 简化了跨 70 多种文档格式的文本搜索和索引，提供高效工具以快速管理和检索信息。"
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "GroupDocs.Search 的核心功能"
  features:
    # feature loop
    - title: "全面的文本搜索"
      content: "在多种文档格式中查找文本，例如 PDF、Word 文档、PowerPoint 演示文稿和电子表格。使用精确匹配、模糊搜索和通配符运算符以获得细致的搜索结果。"

    # feature loop
    - title: "针对大型数据的优化索引"
      content: "创建结构化索引以加速搜索，使您能够高效地浏览大量文档库。"

    # feature loop
    - title: "支持多种语言"
      content: "在 80 多种语言中进行搜索，内置支持不同的键盘布局和词语形态变化，提高精确度。"

    # feature loop
    - title: "灵活的搜索设置"
      content: "通过选项如大小写敏感、基于日期的过滤以及排除特定单词的能力来自定义搜索，以获得精确结果。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "实现高级搜索查询"
      content: |
        此示例演示如何有效地使用搜索查询在 PPTX 文档中进行搜索。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 定义搜索索引的目录
          Index index = new Index("c:/MyIndex");
              
          // 提供文档的文件路径
          index.add("c:/MyDocuments");

          // 输入加密文档的密码
          index.getDictionaries().getDocumentPasswords().add("protected.pptx", "123456");

          // 启用模糊搜索以检测相似单词
          SearchOptions options = new SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8));

          // 获取搜索结果
          SearchResult result = index.Search("Loarem", options);
          
          // 处理和分析搜索结果
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "复制"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-search</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "点击复制"
          copy_done: "已复制"
        top_links:
          #  loop
          - title: "下载结果"
            icon: "download"
            link: "/examples/search/formats/searchdocument.pptx"
        links:
          #  loop
          - title: "更多示例"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "文档"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "准备好开始了吗？"
  description: "免费试用 GroupDocs.Search 的功能或申请许可证"
  items:
    #  loop
    - title: "Maven 下载"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "许可"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "主要功能概述"
    exclude: "document"
    description: "探索旨在提高效率和精确度的高性能文本搜索功能。"
    items: 
          
        # operation loop 1
        - name: "条件搜索"
          operation: "boolean"
          link: "/search/java/boolean/pptx/"
          description: "使用布尔条件在文档中查找信息"

        # operation loop 2
        - name: "区分大小写搜索"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pptx/"
          description: "通过考虑大小写敏感性提高搜索准确性"

        # operation loop 3
        - name: "文档索引"
          operation: "document"
          link: "/search/java/document/pptx/"
          description: "一次索引文档，然后为多次搜索重用索引"

        # operation loop 4
        - name: "搜索过滤器"
          operation: "filters"
          link: "/search/java/filters/pptx/"
          description: "使用过滤器缩小处理的数据范围"

        # operation loop 5
        - name: "精确短语"
          operation: "phrase"
          link: "/search/java/phrase/pptx/"
          description: "搜索特定的句子或短语"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "使用 GroupDocs.Search 在 PPTX 文档中查找信息"
    exclude: "PPTX"
    description: "GroupDocs.Search 支持超过 70 种格式，包括办公文件，启用快速搜索和高级索引功能。"
    items: 
        # format loop 1
        - name: "在 DOCX 文档中搜索"
          format: "DOCX"
          link: "/search/java/document/docx/"
          description: "Microsoft Word Open XML 文档"
          
        # format loop 2
        - name: "在 PDF 文档中搜索"
          format: "PDF"
          link: "/search/java/document/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 3
        - name: "在 PPTX 文档中搜索"
          format: "PPTX"
          link: "/search/java/document/pptx/"
          description: "PowerPoint Open XML 演示文稿"

        # format loop 4
        - name: "在 TXT 文档中搜索"
          format: "TXT"
          link: "/search/java/document/txt/"
          description: "文本文件"
          
        # format loop 5
        - name: "在 XLSX 文档中搜索"
          format: "XLSX"
          link: "/search/java/document/xlsx/"
          description: "Microsoft Excel Open XML 电子表格"
  

---