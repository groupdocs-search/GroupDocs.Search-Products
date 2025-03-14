
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: zh
format: Pdf
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "在 PDF 文档中搜索，使用 Java"
head_description: "GroupDocs.Search for Java 为 Java 应用程序添加强大的文本搜索功能，支持多种商务文档格式。"

############################# Header ############################
title: "在商务文档中查找文本" 
description: "GroupDocs.Search for Java 允许您使用灵活而精准的查询在文档中搜索文本。将搜索功能无缝集成到 Java 应用程序中。"
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
    title: "什么是 GroupDocs.Search？"
    link: "/search/java/"
    link_title: "了解更多"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) 是一个强大的库，提供快速的文本搜索和文档索引功能。它支持超过 70 种文件格式，包括 PDF、Word、Excel 和 PowerPoint 等行业标准。通过高速度和准确的搜索能力提升您的应用程序。

############################# Steps ############################
steps:
    enable: true
    title: "如何在 PDF 文档中搜索"
    content: |
      [GroupDocs.Search](/search/java/) 允许在 PDF 文档中进行快速高效的文本搜索，非常适合 Java 应用程序。
      
      1. 指定一个文件夹来存储搜索索引。
      2. 选择包含您的文档的文件夹。
      3. 配置搜索选项，将结果限制为 PDF 文档。
      4. 运行搜索并获取结果。
   
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
        // 存储可重用搜索索引的目录
        Index index = new Index("c:/MyIndex");

        // 包含文档的文件夹
        index.add("c:/MyDocuments");

        // 按文档格式筛选搜索
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.createFileExtension(".pdf");

        // 检索搜索结果
        SearchResult result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "增强的搜索功能"
  description: "GroupDocs.Search for Java 在超过 70 种文件格式中提供高级文本搜索。索引功能加速搜索并提高文档管理效率。"
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "GroupDocs.Search 的关键功能"
  features:
    # feature loop
    - title: "强大的文本搜索"
      content: "在常见文档格式中查找文本，例如 PDF、Word 文件、演示文稿和电子表格。支持多种搜索方法，包括模糊搜索、同音词和通配符。"

    # feature loop
    - title: "优化的索引以提高性能"
      content: "创建和重用搜索索引以增强搜索速度和效率，特别是在大型文档集合中。"

    # feature loop
    - title: "多语言搜索支持"
      content: "支持在超过 80 种语言的文档中搜索。识别不同的键盘布局和单词变体以提高准确性。"

    # feature loop
    - title: "可定制的搜索选项"
      content: "通过过滤器、正则表达式和其他高级搜索设置缩小搜索结果。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "搜索前过滤文档"
      content: |
        了解如何使用过滤器优化搜索
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 设置排除某些文件格式的索引
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new Index("c:/MyIndex", settings);
              
          // 指定文档存储路径
          index.add("c:/MyDocuments");

          // 检索搜索结果
          SearchResult result = index.search("Lorem", options);
          
          // 处理并使用搜索结果
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
            link: "/examples/search/formats/searchfilters.pdf"
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
    title: "关键功能"
    exclude: "filters"
    description: "进行精准高效的文本搜索。"
    items: 
          
        # operation loop 1
        - name: "条件搜索"
          operation: "boolean"
          link: "/search/java/boolean/pdf/"
          description: "使用布尔条件在文档中查找信息"

        # operation loop 2
        - name: "区分大小写搜索"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pdf/"
          description: "通过考虑大小写敏感性提高搜索准确性"

        # operation loop 3
        - name: "文档索引"
          operation: "document"
          link: "/search/java/document/pdf/"
          description: "一次索引文档，然后为多次搜索重用索引"

        # operation loop 4
        - name: "搜索过滤器"
          operation: "filters"
          link: "/search/java/filters/pdf/"
          description: "使用过滤器缩小处理的数据范围"

        # operation loop 5
        - name: "精确短语"
          operation: "phrase"
          link: "/search/java/phrase/pdf/"
          description: "搜索特定的句子或短语"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "在商务文档中搜索"
    exclude: "PDF"
    description: "GroupDocs.Search 支持超过 70 种文件格式，便于在被广泛使用的办公文档中进行搜索。"
    items: 
        # format loop 1
        - name: "DOCX 搜索过滤器"
          format: "DOCX"
          link: "/search/java/filters/docx/"
          description: "Microsoft Word Open XML 文档"
          
        # format loop 2
        - name: "PDF 搜索过滤器"
          format: "PDF"
          link: "/search/java/filters/pdf/"
          description: "Adobe 可移植文档格式"
          
        # format loop 3
        - name: "PPTX 搜索过滤器"
          format: "PPTX"
          link: "/search/java/filters/pptx/"
          description: "PowerPoint Open XML 演示文稿"

        # format loop 4
        - name: "TXT 搜索过滤器"
          format: "TXT"
          link: "/search/java/filters/txt/"
          description: "文本文件"
          
        # format loop 5
        - name: "XLSX 搜索过滤器"
          format: "XLSX"
          link: "/search/java/filters/xlsx/"
          description: "Microsoft Excel Open XML 电子表格"
  

---