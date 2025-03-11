
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:35
draft: false
lang: zh
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "在 .NET 中使用 GroupDocs.Search 搜索 XLSX 文档"
head_description: "使用 GroupDocs.Search for .NET 在各种文档格式中进行高效文本搜索，支持 C#."

############################# Header ############################
title: "先进的文档文本搜索" 
description: "GroupDocs.Search for .NET 简化了热门文档格式中的文本搜索，使您能够在 .NET 应用程序中创建强大的搜索查询。"
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费下载"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "什么是 GroupDocs.Search?"
    link: "/search/net/"
    link_title: "了解更多"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) 是一个强大的库，专为文档中的全文搜索和索引设计。它支持超过 70 种文件格式，包括 PDF、Word、PowerPoint、Excel、图像和 ZIP 文件，确保快速且精确的搜索结果。

############################# Steps ############################
steps:
    enable: true
    title: "如何在 XLSX 文档中执行文本搜索"
    content: |
      [GroupDocs.Search](/search/net/) 在 XLSX 文档中启用高级内容搜索操作，使您能够在 .NET 应用程序中获得更精确的搜索结果。
      
      1. 设置用于存储搜索索引的文件夹。
      2. 选择包含 XLSX 文件的文件夹。
      3. 配置其他搜索选项。
      4. 运行搜索并查看结果。
   
    code:
      platform: "net"
      copy_title: "复制"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "点击以复制"
        copy_done: "已复制"
      links:
        #  loop
        - title: "更多示例"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "文档"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // 定义搜索索引的路径
        Index index = new Index("c:/MyIndex");

        // 选择包含待搜索文档的文件夹
        index.Add("c:/MyDocuments");

        // 启用同音异义词搜索以查找发音相似的单词
        SearchOptions options = new SearchOptions();
        options.UseHomophoneSearch = true;

        // 执行复杂的搜索查询
        SearchResult result = index.Search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高级搜索和索引功能"
  description: "GroupDocs.Search for .NET 提升了超过 70 种文件格式中的文本搜索和索引，提供高效的工具用于定位和管理信息。"
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "GroupDocs.Search 的关键特性"
  features:
    # feature loop
    - title: "强大的文本搜索"
      content: "在多种文档类型中搜索文本，包括 PDF、Word 文档、PowerPoint 演示文稿和电子表格。使用精确匹配、模糊搜索和通配符等功能来细化搜索结果。"

    # feature loop
    - title: "大数据集的快速索引"
      content: "创建和管理搜索索引，以便快速检索信息。索引操作优化了广泛文档集合的搜索速度."

    # feature loop
    - title: "多语言支持"
      content: "支持超过 80 种语言进行搜索，支持不同的键盘布局和单词变体，以提高搜索准确性。"

    # feature loop
    - title: "可自定义的搜索设置"
      content: "通过诸如大小写敏感性、日期范围过滤和单词排除等选项来微调搜索参数，以获得更好的搜索结果。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "执行高级搜索查询"
      content: |
        此示例演示了如何针对 XLSX 文档应用搜索查询。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 定义搜索索引的文件夹
          Index index = new Index("c:/MyIndex");
              
          // 指定文档文件的路径
          index.Add("c:/MyDocuments");

          // 为受保护的文档提供密码
          index.Dictionaries.DocumentPasswords.Add("protected.xlsx", "123456");

          // 启用模糊搜索以查找相似单词
          SearchOptions options = new SearchOptions();
          options.FuzzySearch.Enabled = true;
          options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8);

          // 获取搜索结果
          SearchResult result = index.Search("Loarem", options);
          
          // 处理搜索输出
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "复制"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "点击以复制"
          copy_done: "已复制"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchdocument.xlsx"
        links:
          #  loop
          - title: "更多示例"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "文档"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "准备好开始了吗？"
  description: "免费试用 GroupDocs.Search 的功能或请求许可证"
  items:
    #  loop
    - title: "Nuget 下载"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "许可证"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "探索关键功能"
    exclude: "document"
    description: "利用先进且高性能的搜索功能."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "跨越您的业务文档进行搜索"
    exclude: "XLSX"
    description: "GroupDocs.Search 支持超过 70 种文件格式，包括办公文档，实现快速和高效的搜索及索引功能。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/document/docx/"
          description: "Microsoft Word Open XML 文档"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/document/pdf/"
          description: "Adobe 便携式文档格式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/document/pptx/"
          description: "PowerPoint Open XML 演示文稿"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/document/txt/"
          description: "文本文档"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/document/xlsx/"
          description: "Microsoft Excel Open XML 电子表格"
  

---