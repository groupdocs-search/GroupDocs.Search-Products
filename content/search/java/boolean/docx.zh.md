
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:29
draft: false
lang: zh
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "在DOCX中使用Java进行布尔搜索"
head_description: "借助GroupDocs.Search for Java，开发人员可以使用布尔运算符，如AND、OR和NOT，执行文档搜索。"

############################# Header ############################
title: "布尔文本搜索" 
description: "使用GroupDocs.Search for Java在您的Java项目中创建先进的布尔（AND、OR、NOT）搜索查询。"
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "免费下载"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "关于GroupDocs.Search"
    link: "/search/java/"
    link_title: "了解更多"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/)是一个多功能库，旨在实现文档中的文本搜索和数据索引。它支持超过70种文件类型，包括PDF、Word、Excel、PowerPoint图片和ZIP归档，可有效搜索大型数据集合。

############################# Steps ############################
steps:
    enable: true
    title: "如何在DOCX文档中执行布尔搜索"
    content: |
      [GroupDocs.Search](/search/java/)使得在DOCX文档中进行文本搜索成为可能。通过支持布尔条件，您可以在Java应用程序中提高搜索精度。
      
      1. 指定存储搜索索引的文件夹。
      2. 选择包含DOCX文档的文件夹。
      3. 执行搜索查询并检索结果。
      4. 处理获取的结果。
   
    code:
      platform: "java"
      copy_title: "复制"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
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
        copy_tip: "点击以复制"
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
        // 设置索引文件夹的路径
        Index index = new Index("c:/MyIndex");

        // 提供包含要搜索的文档的文件夹路径
        index.add("c:/MyDocuments");

        // 使用复杂查询运行搜索
        SearchResult result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "强大的文档搜索和索引工具"
  description: "GroupDocs.Search for Java简化了对70多种格式的文本搜索和数据索引。其先进的工具使您能够轻松查找和管理内容。"
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "GroupDocs.Search的关键特性"
  features:
    # feature loop
    - title: "全面的文本搜索"
      content: "在多个格式中进行搜索，如PDF、Word文档、演示文稿、电子表格等。使用精确匹配、模糊搜索和通配符查询等选项来优化结果。"

    # feature loop
    - title: "高效的数据索引"
      content: "建立和维护索引以加快文档搜索。此功能高效组织数据，方便处理大量文档集合。"

    # feature loop
    - title: "多语言支持"
      content: "在超过80种语言的文档中进行搜索。通过利用形态变化的单词形式和不同的键盘布局来增强准确性。"

    # feature loop
    - title: "灵活的搜索自定义"
      content: "通过启用区分大小写、日期范围过滤和排除等功能，调整搜索设置，以优化您的结果。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "使用复杂的布尔搜索查询"
      content: |
        本示例演示如何在DOCX文件中执行布尔搜索。
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 设置搜索索引的文件夹
          Index index = new Index("c:/MyIndex");
              
          // 提供要搜索的文档的路径
          index.add("c:/MyDocuments");

          // 使用布尔逻辑构造查询
          SearchQuery wordQuery1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.createWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // 检索搜索结果
          SearchResult result = index.search(booleanQuery);
          
          // 处理获取的结果
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
          copy_tip: "点击以复制"
          copy_done: "已复制"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchboolean.docx"
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
  description: "免费试用 GroupDocs.Search 的功能或请求许可证"
  items:
    #  loop
    - title: "Maven 下载"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "许可证"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "关键特性一览"
    exclude: "boolean"
    description: "解锁强大而高效的搜索功能"
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "搜索流行的文档格式"
    exclude: "DOCX"
    description: "GroupDocs.Search支持超过70种文件格式，使您能够自定义搜索规则，并使用索引来优化性能。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "Microsoft Word Open XML 文档"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "Adobe 便携式文档格式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "PowerPoint Open XML 演示文稿"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "文本文档"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "Microsoft Excel Open XML 电子表格"
  

---