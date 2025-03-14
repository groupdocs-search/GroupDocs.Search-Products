
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: zh
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "在DOCX中使用Java进行区分大小写的搜索"
head_description: "GroupDocs.Search for Java API帮助Java开发人员在多种文档类型中进行区分大小写的搜索。"

############################# Header ############################
title: "区分大小写的文档搜索" 
description: "GroupDocs.Search for Java允许您在Java项目中实现精确的区分大小写搜索功能。"
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费获取"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "了解GroupDocs.Search"
    link: "/search/java/"
    link_title: "了解更多"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/)是一个多功能文本搜索和索引工具，支持各种文档的搜索。它支持超过70种格式，如PDF、Word文件、PowerPoint演示文稿、Excel表格、图像和ZIP文件，使您能够高效处理大型数据集。

############################# Steps ############################
steps:
    enable: true
    title: "在DOCX文件中进行区分大小写搜索的指南"
    content: |
      使用[GroupDocs.Search](/search/java/)，您可以在DOCX文档中执行区分大小写的搜索，从而增强您的Java项目。
      
      1. 设置用于存储搜索索引的文件夹。
      2. 选择包含DOCX文件的文件夹。
      3. 运行区分大小写的搜索并收集结果。
      4. 处理并使用搜索结果。
   
    code:
      platform: "java"
      copy_title: "复制"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "搜索结果"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-search</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "点击复制"
        copy_done: "已复制"
      links:
        #  loop
        - title: "更多示例"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "文档"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // 定义索引存储的位置
        Index index = new Index("c:/MyIndex");

        // 指向包含要搜索的文档的文件夹
        index.add("c:/MyDocuments");

        // 在搜索设置中启用区分大小写的模式
        SearchOptions options = new SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // 执行搜索
        SearchResult result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "增强的搜索和索引工具"
  description: "使用GroupDocs.Search for Java，您可以优化超过70种格式的文档搜索和索引，使定位和组织信息更加高效。"
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "GroupDocs.Search的亮点"
  features:
    # feature loop
    - title: "灵活的文本搜索"
      content: "在PDF、Word文件、电子表格和演示文稿中进行搜索。使用准确匹配、模糊搜索和通配符支持等工具，进一步细化搜索结果。"

    # feature loop
    - title: "高效的索引管理"
      content: "组织和索引大型数据集，以提高处理大文件集合时的搜索速度和性能。"

    # feature loop
    - title: "支持全球语言"
      content: "支持超过80种语言的搜索，适应不同的键盘布局和语言变体，以提高搜索准确性。"

    # feature loop
    - title: "可自定义的搜索过滤器"
      content: "可通过大小写敏感性、日期范围过滤和在索引期间排除不需要的词或数据等选项调整搜索条件。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "示例：区分大小写的搜索查询"
      content: |
        此示例演示了如何对DOCX文档实施区分大小写的搜索。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 定义搜索索引的目录
          Index index = new Index("c:/MyIndex");
              
          // 指定文档文件夹的位置
          index.add("c:/MyDocuments");

          // 设置搜索查询
          SearchQuery wordQuery = SearchQuery.createWordQuery("Lorem");

          // 在搜索选项中启用区分大小写
          SearchOptions options = new SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // 执行文档搜索
          SearchResult result = index.search(wordQuery, options);
          
          // 处理检索到的结果
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "复制"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-search</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "点击复制"
          copy_done: "已复制"
        top_links:
          #  loop
          - title: "下载结果"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.docx"
        links:
          #  loop
          - title: "更多示例"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "文档"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "准备好开始了吗？"
  description: "免费试用 GroupDocs.Search 的功能或申请许可证"
  items:
    #  loop
    - title: "Maven 下载"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "许可"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "关键特性概述"
    exclude: "case-sensitive"
    description: "探索GroupDocs.Search for Java提供的强大而有效的搜索能力。"
    items: 
          
        # operation loop 1
        - name: "条件搜索"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "使用布尔条件在文档中查找信息"

        # operation loop 2
        - name: "区分大小写搜索"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "通过考虑大小写敏感性提高搜索准确性"

        # operation loop 3
        - name: "文档索引"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "一次索引文档，然后为多次搜索重用索引"

        # operation loop 4
        - name: "搜索过滤器"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "使用过滤器缩小处理的数据范围"

        # operation loop 5
        - name: "精确短语"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "搜索特定的句子或短语"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "支持的搜索文件格式"
    exclude: "DOCX"
    description: "GroupDocs.Search支持超过70种流行的文档格式，提供可自定义的搜索设置和高效的索引功能。"
    items: 
        # format loop 1
        - name: "DOCX 大小写敏感搜索"
          format: "DOCX"
          link: "/search/java/case-sensitive/docx/"
          description: "Microsoft Word Open XML 文档"
          
        # format loop 2
        - name: "PDF 大小写敏感搜索"
          format: "PDF"
          link: "/search/java/case-sensitive/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 3
        - name: "PPTX 大小写敏感搜索"
          format: "PPTX"
          link: "/search/java/case-sensitive/pptx/"
          description: "PowerPoint Open XML 演示文稿"

        # format loop 4
        - name: "TXT 大小写敏感搜索"
          format: "TXT"
          link: "/search/java/case-sensitive/txt/"
          description: "文本文件"
          
        # format loop 5
        - name: "XLSX 大小写敏感搜索"
          format: "XLSX"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Microsoft Excel Open XML 电子表格"
  

---