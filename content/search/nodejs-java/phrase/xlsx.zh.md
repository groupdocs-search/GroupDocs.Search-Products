
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:54
draft: false
lang: zh
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "在XLSX中搜索短语，使用Node.js"
head_description: "GroupDocs.Search for Node.js via Java为JavaScript应用程序添加强大的短语搜索功能，以实现高效的文档搜索。"

############################# Header ############################
title: "在文档中查找短语" 
description: "使用GroupDocs.Search for Node.js via Java快速定位特定短语。将快速且准确的搜索功能集成到您的Node.js应用程序中。"
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "下载"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search功能"
    link: "/search/nodejs-java/"
    link_title: "了解更多"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/)是一个高性能库，用于索引和搜索文档中的文本。它支持70多种文件格式，包括PDF、Word文档、Excel电子表格、图像和ZIP档案，确保准确且快速的搜索结果。

############################# Steps ############################
steps:
    enable: true
    title: "如何在XLSX文档中查找短语"
    content: |
      [GroupDocs.Search](/search/nodejs-java/)使在XLSX文档中进行短语搜索成为可能。应用不同的搜索选项以优化Node.js via Java应用程序中的结果。
      
      1. 设置搜索索引文件夹。
      2. 定义包含XLSX文件的文件夹。
      3. 配置搜索参数。
      4. 获取并处理搜索结果。
   
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

        // 指定存储搜索索引的路径
        const index = new searchLib.Index("c:/MyIndex");

        // 设置包含文档的文件夹
        index.add("c:/MyDocuments");

        // 配置搜索设置
        const word1 = searchLib.SearchQuery.createWordQuery("lorem");
        const word2 = searchLib.SearchQuery.createWordQuery("ipsum");
        const word3 = searchLib.SearchQuery.createWordQuery("dolor");

        const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, word2, word3);

        // 运行搜索查询
        const result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "发现Node.js文档搜索引擎"
  description: "GroupDocs.Search for Node.js via Java支持在70多种文件格式中进行短语搜索，使得使用高级搜索功能查找和整理数据变得更加高效。"
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "GroupDocs.Search的关键功能"
  features:
    # feature loop
    - title: "短语搜索"
      content: "在商业文档中查找确切短语，如PDF、Word文件、演示文稿和电子表格。在不完全知道短语的情况下，使用通配符和灵活的搜索选项。"

    # feature loop
    - title: "优化的数据索引"
      content: "通过创建可重用的索引来提升搜索性能。结构化索引加快文档搜索速度，并提高准确性。"

    # feature loop
    - title: "多语言兼容性"
      content: "在80多种语言的文档中进行搜索，支持不同的键盘布局和形态变化，确保精确结果。"

    # feature loop
    - title: "高级搜索选项"
      content: "通过区分大小写、模糊匹配、同音词检测、文档过滤和其他强大功能定制搜索。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "使用高级搜索技术"
      content: |
        学习如何构造查询以在XLSX中进行搜索。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // 定义搜索索引目录
          const index = new searchLib.Index("c:/MyIndex");
              
          // 设置目标文档的路径
          index.add("c:/MyDocuments");

          // 为所需短语创建查询
          const word1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wildcard = searchLib.SearchQuery.createWildcardQuery(1, 7);
          const word2 = searchLib.SearchQuery.createWordQuery("dolor");

          const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // 获取搜索结果
          const result = index.search(query);
          
          // 处理并使用结果
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
            link: "/examples/search/formats/searchphrase.xlsx"
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
    title: "高级搜索功能"
    exclude: "phrase"
    description: "利用强大的搜索功能实现更快速和更准确的结果。"
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
    title: "在商业文档中搜索短语"
    exclude: "XLSX"
    description: "GroupDocs.Search支持在70多种文档格式中进行短语搜索。利用高级选项和索引简化搜索过程。"
    items: 
        # format loop 1
        - name: "DOCX 短语搜索"
          format: "DOCX"
          link: "/search/nodejs-java/phrase/docx/"
          description: "Microsoft Word Open XML 文档"
          
        # format loop 2
        - name: "PDF 短语搜索"
          format: "PDF"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 3
        - name: "PPTX 短语搜索"
          format: "PPTX"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "PowerPoint Open XML 演示文稿"

        # format loop 4
        - name: "TXT 短语搜索"
          format: "TXT"
          link: "/search/nodejs-java/phrase/txt/"
          description: "文本文件"
          
        # format loop 5
        - name: "XLSX 短语搜索"
          format: "XLSX"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Microsoft Excel Open XML 电子表格"
  

---