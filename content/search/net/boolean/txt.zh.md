
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:30
draft: false
lang: zh
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "在 .NET 中使用布尔运算符搜索 TXT"
head_description: "GroupDocs.Search for .NET API 允许 C# 开发者使用 AND、OR 和 NOT 等布尔运算符搜索文档内容。"

############################# Header ############################
title: "布尔逻辑文本搜索" 
description: "GroupDocs.Search for .NET 使在 .NET 应用程序中使用布尔运算符（AND、OR、NOT）创建高级搜索查询变得简单。"
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
    title: "GroupDocs.Search 是什么？"
    link: "/search/net/"
    link_title: "了解更多"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) 是一个全面的文档文本搜索和索引库。它支持超过 70 种文件格式，如 PDF、Word、PowerPoint、Excel、图像和 ZIP 文件，从而实现对大量信息的高效处理。

############################# Steps ############################
steps:
    enable: true
    title: "如何使用布尔逻辑搜索 TXT 文档内容"
    content: |
      [GroupDocs.Search](/search/net/) 使搜索 TXT 文档内容变得简单。它提供布尔逻辑搜索条件以在 .NET 应用程序中细化结果。
      
      1. 指定存储搜索索引的文件夹。
      2. 选择包含 TXT 文件的文件夹。
      3. 运行搜索并获取结果。
      4. 处理结果。
   
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
        // 设置索引文件夹的路径
        Index index = new Index("c:/MyIndex");

        // 指定包含要搜索的文档的文件夹
        index.Add("c:/MyDocuments");

        // 使用复杂的查询运行搜索
        SearchResult result = index.Search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "探索文档搜索和索引的高级功能"
  description: "GroupDocs.Search for .NET 库简化了对 70 多种文件格式的文本搜索和索引。借助高级搜索工具，轻松定位和管理信息。"
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "GroupDocs.Search 的主要功能"
  features:
    # feature loop
    - title: "强大的文本搜索"
      content: "跨各种文件类型（包括 PDF、Word 文档、PowerPoint 演示文稿和电子表格）搜索文本。使用精确匹配、模糊搜索和通配符等功能来细化结果。"

    # feature loop
    - title: "索引大型数据集"
      content: "创建和维护索引以加快搜索速度。索引结构化和组织数据，使搜索大量文档集合变得更容易。"

    # feature loop
    - title: "支持多种语言"
      content: "支持 80 多种语言的文档搜索，支持不同的键盘布局和形态学词形，以提高搜索准确性。"

    # feature loop
    - title: "可自定义的搜索选项"
      content: "通过区分大小写、日期范围过滤器和在索引期间排除特定单词或数据的功能调整搜索设置。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "使用高级布尔搜索查询"
      content: |
        本示例演示如何应用布尔查询搜索 TXT 文档。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 设置搜索索引的文件夹
          Index index = new Index("c:/MyIndex");
              
          // 指定要搜索的文档的路径
          index.Add("c:/MyDocuments");

          // 使用布尔逻辑创建搜索查询
          SearchQuery wordQuery1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.CreateWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.CreateAndQuery(wordQuery1, wordQuery2);

          // 获取搜索结果
          SearchResult result = index.Search(booleanQuery);
          
          // 处理搜索结果
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
            link: "/examples/search/formats/searchboolean.txt"
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
    title: "发现关键特性"
    exclude: "boolean"
    description: "探索先进和高效的搜索功能。"
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/txt/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/txt/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/txt/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/txt/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/txt/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "跨流行文档格式搜索"
    exclude: "TXT"
    description: "GroupDocs.Search 支持超过 70 种文件格式。自定义搜索规则并利用索引来节省时间和精力。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/boolean/docx/"
          description: "Microsoft Word Open XML 文档"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/boolean/pdf/"
          description: "Adobe 便携式文档格式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/boolean/pptx/"
          description: "PowerPoint Open XML 演示文稿"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/boolean/txt/"
          description: "文本文档"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/boolean/xlsx/"
          description: "Microsoft Excel Open XML 电子表格"
  

---