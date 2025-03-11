
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:37
draft: false
lang: zh
format: Docx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "在 DOCX 文档中搜索，使用 .NET"
head_description: "GroupDocs.Search for .NET 通过高效的文本搜索增强 C# 应用程序，以支持各种商业文档格式。"

############################# Header ############################
title: "在商务文档中搜索文本" 
description: "GroupDocs.Search for .NET 使您能够在文档中进行强大且灵活的文本搜索。将搜索功能无缝集成到 .NET 应用程序中。"
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
       [GroupDocs.Search for .NET](/search/net/) 是一个强大的库，用于高效的文本搜索和文档索引。它支持超过 70 种文件格式，包括行业标准的文档，如 PDF、Word、Excel 和 PowerPoint。提高搜索性能，获得快速且准确的结果。

############################# Steps ############################
steps:
    enable: true
    title: "如何在 DOCX 数据中搜索"
    content: |
      [GroupDocs.Search](/search/net/) 使在 DOCX 文档中进行高效文本搜索成为可能，非常适合 .NET 应用程序。
      
      1. 设置一个用于存储搜索索引的文件夹。
      2. 选择包含您文件的文件夹。
      3. 配置搜索选项，仅处理 DOCX 文档。
      4. 执行搜索并检索结果。
   
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
        // 存储可重用搜索索引的路径
        Index index = new Index("c:/MyIndex");

        // 包含文档的文件夹
        index.Add("c:/MyDocuments");

        // 仅在特定文件格式中搜索
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".docx");

        // 检索搜索结果
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高级搜索功能"
  description: "GroupDocs.Search for .NET 使您能够在超过 70 种文件格式中进行复杂的文本搜索。索引提高搜索效率，帮助有效管理文档内容。"
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "GroupDocs.Search 的主要功能"
  features:
    # feature loop
    - title: "高级文本搜索"
      content: "从流行的商业文档中提取相关文本，包括 PDF、Word 文件、演示文稿和电子表格。支持多种搜索技术，如模糊搜索、同音词检测和通配符。"

    # feature loop
    - title: "优化的索引以加快搜索"
      content: "构建和重用搜索索引以提高搜索速度。索引在搜索大型文档集合时优化性能。"

    # feature loop
    - title: "支持多种语言"
      content: "在超过 80 种语言编写的文档中进行搜索。自动检测不同的键盘布局和单词变体，以提高准确性。"

    # feature loop
    - title: "灵活的搜索设置"
      content: "通过可自定义的选项（包括过滤器、正则表达式和大小写敏感性设置）来细化搜索结果。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "过滤待处理的文档"
      content: |
        了解如何使用过滤器缩小文档搜索范围
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 设置索引以排除某些文件格式
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.CreateFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter);
          settings.DocumentFilter = invertedFilter;

          Index index = new Index("c:/MyIndex", settings);
              
          // 指定文档目录
          index.Add("c:/MyDocuments");

          // 检索搜索结果
          SearchResult result = index.Search("Lorem");
          
          // 处理并使用搜索输出
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
            link: "/examples/search/formats/searchfilters.docx"
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
    title: "关键功能"
    exclude: "filters"
    description: "执行准确高效的数据搜索。"
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "在您的商务文档中查找数据"
    exclude: "DOCX"
    description: "GroupDocs.Search 支持 70+ 种文件格式，允许高效处理和搜索流行的办公文档。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "Microsoft Word Open XML 文档"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "Adobe 便携式文档格式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "PowerPoint Open XML 演示文稿"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "文本文档"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "Microsoft Excel Open XML 电子表格"
  

---