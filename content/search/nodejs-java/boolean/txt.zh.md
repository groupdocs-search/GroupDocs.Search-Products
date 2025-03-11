
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:31
draft: false
lang: zh
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "通过 Node.js 进行布尔 TXT 搜索"
head_description: "使用 GroupDocs.Search for Node.js via Java API，在文档内容中执行高级搜索，利用布尔运算符如 AND、OR 和 NOT，专为 JavaScript 开发者量身定制。"

############################# Header ############################
title: "执行布尔逻辑搜索" 
description: "借助 GroupDocs.Search for Node.js via Java，您可以在 Node.js 环境中无缝创建使用布尔运算符（AND、OR、NOT）的高级搜索查询。"
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "立即下载"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search 是什么？"
    link: "/search/nodejs-java/"
    link_title: "了解更多"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) 是一个强大的文本搜索和索引工具，支持超过 70 种格式，例如 PDF、Word、Excel、PowerPoint、图像和 ZIP 文件，使您能高效处理大量信息。

############################# Steps ############################
steps:
    enable: true
    title: "如何使用布尔运算符在 TXT 文档中搜索"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) 可以有效地搜索 TXT 文件中的内容。通过布尔逻辑，您可以在 Node.js via Java 应用程序中针对搜索查询进行优化，提高准确性。
      
      1. 设置用于存储搜索索引的文件夹。
      2. 选择包含 TXT 文件的文件夹进行搜索。
      3. 运行搜索查询并检索结果。
      4. 处理和分析搜索结果。
   
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

        // 设置索引文件夹的位置
        const index = new searchLib.Index("c:/MyIndex");

        // 指定包含要搜索文档的文件夹
        index.add("c:/MyDocuments");

        // 执行带有高级逻辑的搜索查询
        const result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "强大的文档搜索和索引工具"
  description: "GroupDocs.Search for Node.js via Java 为超过 70 种文件类型简化文本搜索和索引，帮助您更快速、精准地找到和管理信息。"
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "GroupDocs.Search的主要功能"
  features:
    # feature loop
    - title: "增强的文本搜索"
      content: "快速找到各种格式中的文本，例如 PDF、Word 文档、演示文稿和电子表格。使用精确匹配、通配符搜索和模糊搜索等功能以获取准确结果。"

    # feature loop
    - title: "高效的数据索引"
      content: "构建和管理索引以加快大型文档集合中的搜索速度。索引确保了对数据的快速和结构化访问。"

    # feature loop
    - title: "多语言支持"
      content: "支持在超过 80 种语言的文档中进行搜索。形态学支持和键盘布局兼容性增强了不同语言的搜索结果。"

    # feature loop
    - title: "灵活的搜索设置"
      content: "通过启用区分大小写、应用日期过滤器或在索引过程中跳过特定单词和数据来自定义您的搜索。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "高级布尔搜索示例"
      content: |
        本示例演示了如何创建基于布尔的查询以搜索 TXT 文档中的内容。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // 定义搜索索引的文件夹
          const index = new searchLib.Index("c:/MyIndex");
              
          // 提供要搜索的文档位置
          index.add("c:/MyDocuments");

          // 使用布尔运算符构建查询
          const wordQuery1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wordQuery2 = searchLib.SearchQuery.createWordQuery("ipsum");
          const booleanQuery = searchLib.SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // 检索搜索结果
          const result = index.search(booleanQuery);
          
          // 处理和使用搜索结果
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
            link: "/examples/search/formats/searchboolean.txt"
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
    title: "GroupDocs.Search 的主要功能"
    exclude: "boolean"
    description: "解锁高级、高效和可自定义的搜索功能。"
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "搜索常见文档格式"
    exclude: "TXT"
    description: "GroupDocs.Search 支持超过 70 种文件格式，提供灵活的搜索规则和高效的索引，节省时间和精力。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/boolean/docx/"
          description: "Microsoft Word Open XML 文档"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "Adobe 便携式文档格式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "PowerPoint Open XML 演示文稿"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/boolean/txt/"
          description: "文本文档"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Microsoft Excel Open XML 电子表格"
  

---