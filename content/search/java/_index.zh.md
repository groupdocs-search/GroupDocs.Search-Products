---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: zh
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Java 文档搜索和索引解决方案，支持PDF、Office文件和网页内容"
head_description: "强大的文本搜索和索引能力用于Java应用程序。轻松搜索和组织PDF、Word、Excel、演示文稿、电子邮件和网页格式中的数据。"

############################# Header ############################
title: "使用Java API进行高效文档搜索和索引"
description: "通过在所有流行文档格式上实施强大的文本搜索功能，增强Java应用程序。"
words:
  for: "为"

actions:
  main: "免费下载Maven"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-search/"
  alt: "许可"
  alt_link: "https://purchase.groupdocs.com/pricing/search/java/"
  title: "今天就开始您的旅程！"
  description: "免费体验GroupDocs.Search的功能，或申请许可以解锁其全部潜力。"

release:
  title: "版本 {0} 已发布"
  notes: "查看新功能"
  downloads: "下载"

code:
  title: "使用Java寻找文件中的文本"
  more: "更多示例"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-search</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // 为您的文档创建索引
    Index index = new Index("c:/MyIndex");

    // 将文档添加到索引中以实现高效搜索
    index.add("c:/MyDocuments");
    
    // 搜索特定单词或短语，例如
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search 概述"
  description: "发现Java Java库的强大文本搜索能力。"
  features:
    # feature loop
    - title: "Java 中的索引和搜索操作"
      content: "使用GroupDocs.Search for Java，您可以有效地收集、存储和分析数据，以创建详细的索引，从而实现更快速、更准确的搜索。"

    # feature loop
    - title: "通过合并索引优化搜索"
      content: "轻松结合多个索引，使用GroupDocs.Search for Java来优化搜索。通过将多个增量索引合并为单个高性能索引来减少小的增量索引的影响。"

    # feature loop
    - title: "支持多语言键盘布局"
      content: "使用GroupDocs.Search for Java跨不同语言和键盘布局进行搜索。它支持88种语言和164种键盘配置，灵活多变无与伦比。"

    # feature loop
    - title: "形态学搜索能力"
      content: "使用GroupDocs.Search for Java查找不同的单词形式，例如单数/复数名词或动词变化。为英语和其他语言定制搜索选项。"

############################# Platforms ############################
platforms:
  enable: true
  title: "平台独立性"
  description: "GroupDocs.Search for Java 与主要操作系统和软件包管理器兼容。"
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "支持的文件格式"
  description: |
    使用GroupDocs.Search for Java处理广泛的文件格式。[查看完整列表](https://docs.groupdocs.com/search/java/supported-document-formats/)。
  groups:
    # group loop
    - color: "green"
      content: |
        ### 流行的办公格式
        * **便携式:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **文本:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### 媒体格式
        * **流行图片格式:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **多页图像:** GIF, WEBP, TIFF
        * **音频:** MP3, WAV
        * **视频:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### 其他
        * **电子邮件:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **网页:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **其他:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Search for Java 的功能"
  description: "有效管理文档内容，提供支持PDF、DOCX、XLSX、PPTX等格式的高级搜索能力。"

  items:
    # feature loop
    - icon: "document_info"
      title: "可定制的搜索参数"
      content: "使用日期范围和区分大小写筛选器来改进搜索。"

    # feature loop
    - icon: "detect"
      title: "增强的拼写检查"
      content: "通过拼写检查、通配符和忽略特殊字符有效搜索。"

    # feature loop
    - icon: "collect"
      title: "过滤搜索结果"
      content: "应用筛选器，以根据特定文档类型或标准关注搜索结果。"

    # feature loop
    - icon: "get"
      title: "数据的导入和导出"
      content: "轻松导入索引数据或将结果导出到文件以供进一步使用。"

    # feature loop
    - icon: "remove"
      title: "跳过不必要的文件"
      content: "通过排除特定文件或单词来优化索引。"

    # feature loop
    - icon: "style"
      title: "HTML和URL处理"
      content: "提取HTML内容到文件，并为搜索结果生成URL链接。"

    # feature loop
    - icon: "detect"
      title: "在大型索引中快速搜索"
      content: "通过将大型索引分割为可管理的块来加速搜索操作。"

    # feature loop
    - icon: "manipulate"
      title: "基于流的索引"
      content: "直接从流或数据结构中索引数据。"

    # feature loop
    - icon: "compare"
      title: "处理拼写错误的查询"
      content: "检测拼写错误，并建议替代词以提高搜索准确性。"

    # feature loop
    - icon: "unreadable_characters"
      title: "全面的归档支持"
      content: "索引嵌套归档，并检索ZIP文件中详细的文件列表。"

    # feature loop
    - icon: "hidden_print"
      title: "节省磁盘空间的索引"
      content: "通过紧凑的索引节省磁盘空间，并处理受密码保护的文件。"

    # feature loop
    - icon: "style"
      title: "自定义同义词支持"
      content: "扩展同义词字典，以增强搜索精度，提供定制选项。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "代码示例"
  description: "通过这些代码示例试用GroupDocs.Search for Java功能。"
  items:
    # code sample loop
    - title: "通过模糊匹配提升搜索准确性"
      content: |
        探索GroupDocs.Search for Java的灵活性，通过先进的模糊搜索功能，管理内容。 [了解更多](https://docs.groupdocs.com/search/java/search-results/)。
        {{< landing/code title="如何处理搜索结果">}}
        ```java {style=abap}
        // 创建索引
        Index index = new Index("C:/IndexFolder");
        index.add("C:/DocumentFolder");

        // 设置搜索选项
        SearchOptions options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // 搜索包含'water'这个词或短语'Lorem ipsum'的文档
        String query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.search(query, options);
        
        // 处理搜索结果
        System.out.println("Documents: " + result.getDocumentCount());
        System.out.println("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            System.out.println("Document: " + document.getDocumentInfo().getFilePath());
            System.out.println("Occurrences " + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "使用正则表达式精细化结果"
      content: |
        在GroupDocs.Search for Java中使用正则表达式，以创建精确且详细的搜索结果。 [探索先进技术](https://docs.groupdocs.com/search/java/regular-expression-search/)。
        {{< landing/code title="如何使用正则表达式搜索">}}
        ```java {style=abap}   
        // 创建索引
        Index index = new Index("C:/IndexFolder");
        index.add("c:/DocumentFolder");
 
        // 搜索文本形式的短语

        // 第一个插入符号字符表示这是一个正则表达式搜索查询
        String query = "^^(.)\\1{1,}";
        // 搜索单词开头的两个或多个相同字符
        SearchResult result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
