
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:38
draft: false
lang: zh
format: Pdf
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "在 PDF 文档中搜索使用 Node.js"
head_description: "GroupDocs.Search for Node.js via Java 为 JavaScript 应用程序添加快速准确的文本搜索功能，支持多种文档格式。"

############################# Header ############################
title: "在商业文档中查找文本" 
description: "GroupDocs.Search for Node.js via Java 提供强大而灵活的文档搜索功能。将文本搜索集成到 Node.js 应用程序中。"
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费下载"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search 是什么？"
    link: "/search/nodejs-java/"
    link_title: "了解更多"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) 是一个强大的搜索和索引库，能够快速检索文档中的文本。它支持超过 70 种文件格式，包括 PDF、Word、Excel 和 PowerPoint，确保精确且高效的搜索。

############################# Steps ############################
steps:
    enable: true
    title: "如何在 PDF 文档中执行搜索"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) 使在 PDF 文档中搜索文本对于 Node.js via Java 应用程序变得简便和高效。
      
      1. 创建一个目录以存储搜索索引。
      2. 选择包含文档的文件夹。
      3. 设置搜索选项仅包括 PDF 文件。
      4. 运行搜索并检索结果。
   
    code:
      platform: "nodejs-java"
      copy_title: "复制"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "点击以复制"
        copy_done: "已复制"
      links:
        #  loop
        - title: "更多示例"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "文档"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // 定义用于存储搜索索引的目录
        const index = new searchLib.Index("c:/MyIndex");

        // 指定包含可搜索文档的文件夹
        index.add("c:/MyDocuments");

        // 限制搜索到特定文件格式
        const options = new searchLib.SearchOptions();
        options.SearchDocumentFilter = 
            searchLib.SearchDocumentFilter.createFileExtension(".pdf");

        // 检索并处理搜索结果
        const result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高级搜索功能"
  description: "GroupDocs.Search for Node.js via Java 通过索引超过 70 种文件格式来提高文档搜索的效率。通过先进的搜索技术优化内容检索。"
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "GroupDocs.Search 的主要功能"
  features:
    # feature loop
    - title: "全面的文本搜索"
      content: "提取并定位流行文档格式中的文本，如 PDF、Word 文件、电子表格和演示文稿。支持模糊搜索、同音词和通配符查询。"

    # feature loop
    - title: "优化的索引性能"
      content: "通过创建可重用的索引加快搜索速度。在处理大型文档集合时提高速度和效率。"

    # feature loop
    - title: "多语言支持"
      content: "在超过 80 种语言的文档中搜索。识别键盘布局和单词变体以提高准确性。"

    # feature loop
    - title: "可自定义的搜索选项"
      content: "通过过滤器、正则表达式、大小写敏感性和其他灵活设置微调搜索结果。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "过滤可搜索的文档"
      content: |
        学习如何使用过滤器来细化文档搜索。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // 配置索引以排除不需要的文件格式
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            searchLib.DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = 
            searchLib.DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new searchLib.Index("c:/MyIndex", settings);
              
          // 指定包含文档的目录
          index.add("c:/MyDocuments");

          // 处理搜索输出以供进一步使用
          const result = index.Search("Lorem", options);
          
          // 处理搜索输出以供进一步使用
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "复制"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "点击以复制"
          copy_done: "已复制"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchfilters.pdf"
        links:
          #  loop
          - title: "更多示例"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "文档"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "准备好开始了吗？"
  description: "免费试用 GroupDocs.Search 的功能或请求许可证"
  items:
    #  loop
    - title: "NPM 下载"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "许可证"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "关键功能"
    exclude: "filters"
    description: "在文档中执行快速而精确的文本搜索。"
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/pdf/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/pdf/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "在多种文档格式中搜索"
    exclude: "PDF"
    description: "GroupDocs.Search 支持超过 70 种文件类型，允许在各种办公和商业文档中高效搜索文本。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/filters/docx/"
          description: "Microsoft Word Open XML 文档"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/filters/pdf/"
          description: "Adobe 便携式文档格式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/filters/pptx/"
          description: "PowerPoint Open XML 演示文稿"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/filters/txt/"
          description: "文本文档"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Microsoft Excel Open XML 电子表格"
  

---