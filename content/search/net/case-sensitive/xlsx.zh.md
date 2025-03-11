
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:32
draft: false
lang: zh
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "在XLSX中使用.NET进行区分大小写的搜索"
head_description: "GroupDocs.Search for .NET API使得C#开发者能够对各种文档执行区分大小写的搜索。"

############################# Header ############################
title: "区分大小写的搜索" 
description: "GroupDocs.Search for .NET使您能够在.NET应用程序中创建高级的区分大小写搜索查询。"
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
    title: "什么是GroupDocs.Search？"
    link: "/search/net/"
    link_title: "了解更多"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) 是一个强大的库，用于文档中的文本搜索和索引。它支持70多种文件格式，包括PDF、Word、PowerPoint、Excel、图像和ZIP文件，确保有效处理大数据量。

############################# Steps ############################
steps:
    enable: true
    title: "如何在XLSX文档中执行区分大小写的搜索"
    content: |
      [GroupDocs.Search](/search/net/)简化了在XLSX文档中的区分大小写搜索。可用于在.NET应用程序中细化结果。
      
      1. 定义用于存储搜索索引的文件夹。
      2. 选择包含XLSX文件的文件夹。
      3. 运行搜索并检索结果。
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

        // 在选项中启用区分大小写的搜索
        SearchOptions options = new SearchOptions();
        options.UseCaseSensitiveSearch = true;

        // 运行搜索
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "文档搜索和索引的高级功能"
  description: "GroupDocs.Search for .NET库简化了70多种文件格式的文本搜索和索引。使用强大的搜索工具轻松定位和管理信息。"
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "GroupDocs.Search的主要特性"
  features:
    # feature loop
    - title: "高级文本搜索"
      content: "在各种文件格式中搜索文本，包括PDF、Word文档、电子表格和演示文稿。使用精确匹配、模糊搜索和通配符等选项以获得准确的结果。"

    # feature loop
    - title: "索引大型数据集"
      content: "构建和维护索引以加快搜索速度。组织良好的索引简化了对大量文档的搜索。"

    # feature loop
    - title: "多语言支持"
      content: "在80多种语言的文档中进行搜索，支持不同的键盘布局和单词形式以获得更准确的结果。"

    # feature loop
    - title: "可定制的搜索选项"
      content: "通过区分大小写、日期范围过滤器以及在索引期间排除特定单词或数据的能力来定制搜索设置。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "使用区分大小写的搜索查询"
      content: |
        该示例展示了如何为搜索XLSX文档使用区分大小写的查询。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 设置搜索索引的文件夹
          Index index = new Index("c:/MyIndex");
              
          // 指定要搜索的文档路径
          index.Add("c:/MyDocuments");

          // 创建搜索查询
          SearchQuery wordQuery = SearchQuery.CreateWordQuery("Lorem");

          // 启用区分大小写的搜索选项
          SearchOptions options = new SearchOptions();
          options.UseCaseSensitiveSearch = true;

          // 在文档中搜索文本
          SearchResult result = index.Search(wordQuery, options);
          
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
            link: "/examples/search/formats/searchcase-sensitive.xlsx"
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
    title: "探索主要功能"
    exclude: "case-sensitive"
    description: "发现高级和高效的搜索功能。"
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
    title: "搜索流行的文档格式"
    exclude: "XLSX"
    description: "GroupDocs.Search支持70多种文件格式。自定义搜索规则并使用索引来节省时间和精力。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/case-sensitive/docx/"
          description: "Microsoft Word Open XML 文档"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/case-sensitive/pdf/"
          description: "Adobe 便携式文档格式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/case-sensitive/pptx/"
          description: "PowerPoint Open XML 演示文稿"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/case-sensitive/txt/"
          description: "文本文档"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Microsoft Excel Open XML 电子表格"
  

---