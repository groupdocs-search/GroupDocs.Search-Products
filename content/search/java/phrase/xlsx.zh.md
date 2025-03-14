
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: zh
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "在XLSX中使用Java搜索短语"
head_description: "GroupDocs.Search for Java 为Java应用程序增强了文档内容的高级短语搜索功能。"

############################# Header ############################
title: "在文档中查找短语" 
description: "使用GroupDocs.Search for Java快速定位特定短语。为您的Java应用程序添加强大的搜索功能。"
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "下载"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search 特性"
    link: "/search/java/"
    link_title: "了解更多"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) 是一个强大的库，可用于对文档中的文本进行索引和搜索。它支持超过70种文件格式，包括PDF、Word文档、Excel电子表格、图像和ZIP文件，确保快速而准确的搜索结果。

############################# Steps ############################
steps:
    enable: true
    title: "如何在XLSX文档中查找短语"
    content: |
      [GroupDocs.Search](/search/java/) 简化了在XLSX文档中进行短语搜索。利用各种选项在Java应用程序中细化搜索结果。
      
      1. 创建一个搜索索引目录。
      2. 指定包含XLSX文件的文件夹。
      3. 调整搜索参数。
      4. 检索并分析搜索结果。
   
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
        // 定义搜索索引路径
        Index index = new Index("c:/MyIndex");

        // 指定包含文档的文件夹
        index.add("c:/MyDocuments");

        // 设置搜索偏好
        SearchQuery word1 = SearchQuery.createWordQuery("lorem");
        SearchQuery word2 = SearchQuery.createWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.createWordQuery("dolor");

        SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, word2, word3);
        
        // 执行搜索查询
        SearchResult result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "探索Java文档搜索引擎"
  description: "GroupDocs.Search for Java 允许在70多种文件格式中进行短语搜索。利用高级搜索功能，轻松查找和组织数据。"
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "GroupDocs.Search 的关键功能"
  features:
    # feature loop
    - title: "短语搜索"
      content: "在商业文档中查找确切短语，如PDF、Word文件、演示文稿和电子表格。使用通配符和其他选项，当确切短语未知时。"

    # feature loop
    - title: "优化的数据索引"
      content: "通过创建和重用搜索索引来加快文档搜索。索引有效地组织数据，以实现更快和更准确的搜索。"

    # feature loop
    - title: "多语言兼容性"
      content: "在80多种语言中的文档进行搜索。支持不同的键盘布局和形态分析，以提高搜索精度。"

    # feature loop
    - title: "高级搜索选项"
      content: "通过区分大小写、模糊搜索、同音词匹配、文档过滤以及其他强大特性来定制搜索。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "使用高级搜索方法"
      content: |
        学习如何构建查询以在XLSX中进行搜索。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 定义搜索索引的目录
          Index index = new Index("c:/MyIndex");
              
          // 设置目标文档的路径
          index.add("c:/MyDocuments");

          // 为特定短语创建搜索查询
          SearchQuery word1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.createWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.createWordQuery("dolor");

          SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // 获取搜索结果
          SearchResult result = index.search(query);
          
          // 处理并利用检索到的结果
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
            link: "/examples/search/formats/searchphrase.xlsx"
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
    title: "高级搜索功能"
    exclude: "phrase"
    description: "利用尖端搜索功能提升精确度和性能。"
    items: 
          
        # operation loop 1
        - name: "条件搜索"
          operation: "boolean"
          link: "/search/java/boolean/xlsx/"
          description: "使用布尔条件在文档中查找信息"

        # operation loop 2
        - name: "区分大小写搜索"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/xlsx/"
          description: "通过考虑大小写敏感性提高搜索准确性"

        # operation loop 3
        - name: "文档索引"
          operation: "document"
          link: "/search/java/document/xlsx/"
          description: "一次索引文档，然后为多次搜索重用索引"

        # operation loop 4
        - name: "搜索过滤器"
          operation: "filters"
          link: "/search/java/filters/xlsx/"
          description: "使用过滤器缩小处理的数据范围"

        # operation loop 5
        - name: "精确短语"
          operation: "phrase"
          link: "/search/java/phrase/xlsx/"
          description: "搜索特定的句子或短语"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "在商业文档中搜索短语"
    exclude: "XLSX"
    description: "GroupDocs.Search 使70多种文档格式中的短语搜索成为可能。利用先进的选项和索引实现高效搜索。"
    items: 
        # format loop 1
        - name: "DOCX 短语搜索"
          format: "DOCX"
          link: "/search/java/phrase/docx/"
          description: "Microsoft Word Open XML 文档"
          
        # format loop 2
        - name: "PDF 短语搜索"
          format: "PDF"
          link: "/search/java/phrase/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 3
        - name: "PPTX 短语搜索"
          format: "PPTX"
          link: "/search/java/phrase/pptx/"
          description: "PowerPoint Open XML 演示文稿"

        # format loop 4
        - name: "TXT 短语搜索"
          format: "TXT"
          link: "/search/java/phrase/txt/"
          description: "文本文件"
          
        # format loop 5
        - name: "XLSX 短语搜索"
          format: "XLSX"
          link: "/search/java/phrase/xlsx/"
          description: "Microsoft Excel Open XML 电子表格"
  

---