
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:40
draft: false
lang: zh
format: Pptx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "在PPTX中搜索短语，使用.NET"
head_description: "GroupDocs.Search for .NET 为C# 应用程序增强了强大的文档内容短语搜索功能。"

############################# Header ############################
title: "在文档中搜索短语" 
description: "通过GroupDocs.Search for .NET快速查找特定短语。将高效的搜索功能集成到您的.NET应用程序中。"
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "下载"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search 功能"
    link: "/search/net/"
    link_title: "了解更多"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) 是一个强大的库，用于索引和搜索文档中的文本。它支持70多种文件格式，包括PDF、Word文档、Excel表格、图像和ZIP文件，从而实现快速准确的搜索结果。

############################# Steps ############################
steps:
    enable: true
    title: "如何在PPTX文档中搜索短语"
    content: |
      [GroupDocs.Search](/search/net/)简化了PPTX文档中的搜索。使用各种选项在.NET应用程序中细化搜索结果。
      
      1. 设置搜索索引文件夹。
      2. 指定包含PPTX文件的文件夹。
      3. 配置搜索设置。
      4. 获取并处理搜索结果。
   
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
        // 存储搜索索引的路径
        Index index = new Index("c:/MyIndex");

        // 包含文档的文件夹
        index.Add("c:/MyDocuments");

        // 配置搜索选项
        SearchQuery word1 = SearchQuery.CreateWordQuery("lorem");
        SearchQuery word2 = SearchQuery.CreateWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.CreateWordQuery("dolor");

        SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, word2, word3);

        // 执行搜索
        SearchResult result = index.Search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "探索.NET文档搜索引擎"
  description: "GroupDocs.Search for .NET支持在70多种文件格式中进行短语搜索。使用先进的搜索功能轻松定位和管理数据。"
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "GroupDocs.Search的关键特性"
  features:
    # feature loop
    - title: "短语搜索"
      content: "在商业文档中搜索确切短语，包括PDF、Word文件、演示文稿和电子表格。如果确切短语未知，可以使用通配符和其他选项。"

    # feature loop
    - title: "高效的数据索引"
      content: "创建和重用搜索索引以加快文档搜索。索引结构有效地组织数据，使短语搜索更快。"

    # feature loop
    - title: "多语言支持"
      content: "在80多种语言的文档中进行搜索。支持不同的键盘布局和形态单词形式，以提高搜索精度。"

    # feature loop
    - title: "灵活的搜索选项"
      content: "通过区分大小写、模糊搜索和同音异义词搜索、文档过滤等功能自定义搜索。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "使用高级搜索技术"
      content: |
        了解如何为PPTX中的搜索创建查询。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 指定搜索索引的文件夹
          Index index = new Index("c:/MyIndex");
              
          // 设置文档搜索的路径
          index.Add("c:/MyDocuments");

          // 为特定短语创建查询
          SearchQuery word1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.CreateWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.CreateWordQuery("dolor");

          SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, wildcard, word2);

          // 检索搜索结果
          SearchResult result = index.Search(query);
          
          // 处理并利用结果
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
            link: "/examples/search/formats/searchphrase.pptx"
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
    title: "高级特性"
    exclude: "phrase"
    description: "利用强大而高效的搜索功能。"
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "在商业文档中进行短语搜索"
    exclude: "PPTX"
    description: "GroupDocs.Search支持在70多种文档格式中进行搜索。利用高级选项和索引来简化搜索流程。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/phrase/docx/"
          description: "Microsoft Word Open XML 文档"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/phrase/pdf/"
          description: "Adobe 便携式文档格式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/phrase/pptx/"
          description: "PowerPoint Open XML 演示文稿"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/phrase/txt/"
          description: "文本文档"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/phrase/xlsx/"
          description: "Microsoft Excel Open XML 电子表格"
  

---