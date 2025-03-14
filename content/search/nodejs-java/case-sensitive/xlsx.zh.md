
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:48
draft: false
lang: zh
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "在XLSX中执行区分大小写的搜索 - Node.js"
head_description: "GroupDocs.Search for Node.js via Java API允许JavaScript开发人员在不同的文档类型中执行区分大小写的搜索。"

############################# Header ############################
title: "区分大小写的搜索" 
description: "GroupDocs.Search for Node.js via Java使您能够在Node.js应用程序中实现高级区分大小写搜索功能。"
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
    title: "什么是GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "了解更多"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/)是一个强大的库，用于在文档中搜索和索引文本。它支持超过70种格式，包括PDF、Word、Excel、PowerPoint、图片和ZIP文件，能够高效处理大量数据。

############################# Steps ############################
steps:
    enable: true
    title: "在XLSX文件中执行区分大小写搜索的步骤"
    content: |
      [GroupDocs.Search](/search/nodejs-java/)使在XLSX文件中进行区分大小写搜索成为可能，提高您的Node.js via Java工作流程。
      
      1. 设置一个文件夹以存放搜索索引。
      2. 选择包含XLSX文件的文件夹。
      3. 运行搜索并获取结果。
      4. 处理并使用结果。
   
    code:
      platform: "nodejs-java"
      copy_title: "复制"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "搜索结果"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "点击复制"
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

        // 指定索引文件夹的路径
        const index = new searchLib.Index("c:/MyIndex");

        // 设置包含要搜索的文档的文件夹
        index.add("c:/MyDocuments");

        // 在设置中启用区分大小写的搜索
        const options = new groupdocs.search.SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // 执行搜索
        const result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "文档搜索和索引的关键特性"
  description: "使用GroupDocs.Search for Node.js via Java，您可以搜索和索引超过70种文件格式中的文本。利用先进的搜索工具，轻松访问和组织信息。"
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "GroupDocs.Search的核心功能"
  features:
    # feature loop
    - title: "全面的文本搜索"
      content: "在各种文档类型中找到文本，如PDF、Word文件、电子表格和演示文稿。使用精确匹配、模糊搜索和通配符等选项以获得准确的结果。"

    # feature loop
    - title: "高效的数据索引"
      content: "创建和管理索引以加快搜索速度。索引有助于组织和快速定位大型文档集合中的数据。"

    # feature loop
    - title: "支持多种语言"
      content: "在超过80种语言中搜索文档，并支持多种键盘布局和单词变体，确保搜索结果的准确性。"

    # feature loop
    - title: "可定制的搜索设置"
      content: "调整搜索设置，包括区分大小写、日期过滤器，以及在索引过程中排除特定术语或数据。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "示例：区分大小写搜索的实现"
      content: |
        此示例演示如何在XLSX文档中执行区分大小写的搜索。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // 定义搜索索引的文件夹
          const index = new searchLib.Index("c:/MyIndex");
              
          // 提供文档文件夹的路径
          index.add("c:/MyDocuments");

          // 设置搜索查询
          const wordQuery = searchLib.SearchQuery.createWordQuery("Lorem");

          // 激活区分大小写的搜索设置
          const options = new groupdocs.search.SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // 在文档中搜索文本
          const result = index.search(wordQuery, options);
          
          // 处理和处理结果
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "复制"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "点击复制"
          copy_done: "已复制"
        top_links:
          #  loop
          - title: "下载结果"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.xlsx"
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
  description: "免费试用 GroupDocs.Search 的功能或申请许可证"
  items:
    #  loop
    - title: "NPM 下载"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "许可"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "关键功能"
    exclude: "case-sensitive"
    description: "探索用于快速精准文档搜索的高级功能。"
    items: 
          
        # operation loop 1
        - name: "条件搜索"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "使用布尔条件在文档中查找信息"

        # operation loop 2
        - name: "区分大小写搜索"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "通过考虑大小写敏感性提高搜索准确性"

        # operation loop 3
        - name: "文档索引"
          operation: "document"
          link: "/search/nodejs-java/document/xlsx/"
          description: "一次索引文档，然后为多次搜索重用索引"

        # operation loop 4
        - name: "搜索过滤器"
          operation: "filters"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "使用过滤器缩小处理的数据范围"

        # operation loop 5
        - name: "精确短语"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "搜索特定的句子或短语"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "兼容的文档格式"
    exclude: "XLSX"
    description: "GroupDocs.Search支持超过70种文档格式。自定义您的搜索选项，通过索引节省时间。"
    items: 
        # format loop 1
        - name: "DOCX 大小写敏感搜索"
          format: "DOCX"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "Microsoft Word Open XML 文档"
          
        # format loop 2
        - name: "PDF 大小写敏感搜索"
          format: "PDF"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 3
        - name: "PPTX 大小写敏感搜索"
          format: "PPTX"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "PowerPoint Open XML 演示文稿"

        # format loop 4
        - name: "TXT 大小写敏感搜索"
          format: "TXT"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "文本文件"
          
        # format loop 5
        - name: "XLSX 大小写敏感搜索"
          format: "XLSX"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Microsoft Excel Open XML 电子表格"
  

---