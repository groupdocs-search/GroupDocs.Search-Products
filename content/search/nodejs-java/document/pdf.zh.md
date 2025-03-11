
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:35
draft: false
lang: zh
format: Pdf
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "在 PDF 中使用 GroupDocs.Search 查找文本，适用于 Node.js"
head_description: "使用 GroupDocs.Search for Node.js via Java 和 JavaScript 高效地在各种文档格式中搜索文本。"

############################# Header ############################
title: "智能文档搜索解决方案" 
description: "利用 GroupDocs.Search for Node.js via Java 在不同文档格式中定位文本。在 Node.js 应用程序中创建高级搜索查询。"
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费试用"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "关于 GroupDocs.Search 的介绍"
    link: "/search/nodejs-java/"
    link_title: "了解更多"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) 是一款高性能的全文搜索和文档索引库。它支持超过 70 种文件类型，包括 PDF、Word、PowerPoint、Excel、图像和 ZIP 压缩文件，确保快速和准确的结果。

############################# Steps ############################
steps:
    enable: true
    title: "在 PDF 文件中执行搜索"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) 允许您在 PDF 文件中执行搜索，从而在 Node.js via Java 应用程序中精细化结果。
      
      1. 定义搜索索引的存储文件夹。
      2. 选择包含 PDF 文件的文件夹。
      3. 设置其他搜索参数。
      4. 运行搜索并分析结果。
   
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

        // 指定搜索索引存储的目录
        const index = new searchLib.Index("c:/MyIndex");

        // 选择包含要搜索文档的文件夹
        index.add("c:/MyDocuments");

        // 启用同音词搜索以查找发音相似的单词
        const options = new searchLib.SearchOptions();
        options.setUseHomophoneSearch(true);

        // 运行复杂的搜索查询
        const result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高级搜索与索引功能"
  description: "GroupDocs.Search for Node.js via Java 提供强大的文本搜索和索引工具，支持 70 多种文档格式，便于查找和组织信息。"
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "GroupDocs.Search 的关键好处"
  features:
    # feature loop
    - title: "全面的文本搜索"
      content: "在多个文档类型中定位文本，包括 PDF、Word 文档、PowerPoint 演示文稿和电子表格。使用精确匹配、模糊搜索和通配符以获得精细结果。"

    # feature loop
    - title: "大数据的高效索引"
      content: "通过创建结构化索引加快搜索速度，使从大型文档集合中检索信息更加容易。"

    # feature loop
    - title: "支持 80 多种语言"
      content: "在不同语言的文档中进行搜索，自动识别各种单词形式和键盘布局。"

    # feature loop
    - title: "自定义搜索设置"
      content: "调整搜索选项，如区分大小写、日期过滤和单词排除，以获得精确结果。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "在 PDF 文档中使用搜索"
      content: |
        此示例展示了如何在 PDF 文档中使用搜索查询。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // 设置搜索索引的目录
          const index = new searchLib.Index("c:/MyIndex");
              
          // 提供文档存储的文件路径
          index.add("c:/MyDocuments");

          // 输入受保护文件的密码
          index.getDictionaries().getDocumentPasswords().add("protected.pdf", '123456');

          // 启用模糊搜索以检测相似单词
          const options = new searchLib.SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new searchLib.SimilarityLevel(0.8));

          // 提取搜索结果
          const result = index.search("Loarem", options);
          
          // 处理并审查结果
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
            link: "/examples/search/formats/searchdocument.pdf"
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
    title: "探索关键功能"
    exclude: "document"
    description: "发现旨在提高效率和准确性的高速搜索功能。"
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
    title: "在各种文档中搜索"
    exclude: "PDF"
    description: "GroupDocs.Search 支持超过 70 种文件格式，包括办公文档，确保快速和准确的搜索并支持索引。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/document/docx/"
          description: "Microsoft Word Open XML 文档"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/document/pdf/"
          description: "Adobe 便携式文档格式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/document/pptx/"
          description: "PowerPoint Open XML 演示文稿"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/document/txt/"
          description: "文本文档"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Microsoft Excel Open XML 电子表格"
  

---