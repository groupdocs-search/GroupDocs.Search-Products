---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "用于文档、PDF、Office 和 Web 的 Java 文本搜索和索引 API"
head_description: "用于 Java 应用程序的高级文本搜索 API，用于搜索、索引和检索文档中的数据：PDF、Word、Excel、演示文稿、电子邮件和 Web 文件格式."

############################# Header ############################
title: "通过 Java API 搜索和索引文档"
description: "构建 Java 应用程序以执行所有流行文档格式的文本搜索操作。"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Search for Java"
        image: "/border/groupdocs-search-java.svg"
        product: "GroupDocs.Search"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "概述"

            # button loop
            - link: "#features"
              text: "特征"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/search"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/search/java"
              text: "价钱"

    right:
        link_download: "https://downloads.groupdocs.com/search"
        link_learn: "https://docs.groupdocs.com/search/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# 概述 ############################
overview:
    enable: true
    content: |
      GroupDocs.Search for Java 允许您生成允许您的最终用户以前所未有的方式执行搜索操作的业务应用程序。我们的 Java API 使用户能够操作基本到高级的文本搜索功能。创建和合并多个索引。使用简单、布尔、正则表达式 (Regex)、模糊和其他类型的查询来快速、智能地搜索索引。您可以从文件、文档、电子邮件和档案中获取所需的信息，因为 GroupDocs.Search for Java 支持所有流行的文件格式。
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          以下是 GroupDocs.Search for Java 的概述：

        left:
          enable: true
          icon: "fas fa-search"
          title: "索引"
          content: |
            * 创建和管理
            * 合并多个索引
            * Multi-Threading Async 索引
            * Compact 索引
            * Archived Files 索引
        
        right:
          enable: true
          icon: "fas fa-search-plus"
          title: "高级搜索和搜索查询"
          content: |
            * 模糊搜索
            * 同义词搜索
            * 电子邮件搜索
            * 谐音词的处理
            * 搜索受保护的文件
            * 简单的
            * 外卡
            * 正则表达式 (Regex)
            * 分面和布尔值
            * 区分大小写
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Search for Java 支持所有流行的[文档文件格式](https://docs.groupdocs.com/search/java/supported-document-formats/)，包括：微软办公软件、图像、图表等.

        left:
          enable: true
          table:
            # table loop
            - title: "微软办公格式"
              content: |
                * **Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM
                * **Excel**: XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
                * **PowerPoint**: PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
                * **Project**: MPP
                * **Diagram**: VSD, VSS
                * **Microsoft Compiled HTML**: CHM
                * **OneNote**: ONE

        right:
          enable: true
          table:
            # table loop
            - title: "OpenDocument & 其他格式"
              content: |
                * **便携式文档格式**：PDF
                * **OpenDocument**：ODT、OTT、ODS、OTS、ODP
                * **电子邮件**：PST、OST、MSG、EML、EMLX
                * **Web 文件格式**：XML、HTM、HTML、XHTML、MHT、MHTML
                * **音频**：MP3、WAV
                * **视频**：AVI、MOV、QT、FLV、ASF
                * **文字**：TXT
                * **富文本格式**：RTF
                * **Markdown 文档文件**：MD
                * **图像**：BMP、GIF、JP2、PNG、WEBP、TIFF、EMF、WMF、JPG、PSD
                * **其他**：TORRENT、ZIP、DCM、DJVU、EPUB、FB2

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Search for Java 支持以下操作系统、框架和包管理器:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "操作系统"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "支持的框架"
              content: |
                * Java 7 (1.7) 及更高版本

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "开发环境"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "构建自动化工具"
              content: |
                * Maven

############################# 特征 ############################
features:
    enable: true
    title: "GroupDocs.Search for Java 特征"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "使用异步多线程在磁盘或内存中构建索引"

      # feature loop
      - icon: "fas fa-eye"
        content: "查看索引创建和更新进度"

      # feature loop
      - icon: "fas fa-bolt"
        content: "选择性地跳过特定文件的索引并跳过特定单词以更快地索引"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "在索引和导出到文件期间执行导入或使用列表来修改字符"

      # feature loop
      - icon: "fas fa-code"
        content: "索引错误时重新加载索引并警告用户设置矛盾"

      # feature loop
      - icon: "fas fa-cloud"
        content: "最新处理文件的索引状态通知"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "在其他 ZIP 档案中索引压缩档案并获取档案中的索引文件列表"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "通过紧凑索引和密码保护文档节省空间"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "从索引或源文件中提取文档文本"

      # feature loop
      - icon: "fas fa-border-all"
        content: "HTML 格式的教科书建议到文件并生成 URL 以在 HTML 中导航搜索结果"

      # feature loop
      - icon: "fas fa-wrench"
        content: "在索引期间向每个文档添加任意附加字段"

      # feature loop
      - icon: "fas fa-columns"
        content: "为模糊搜索配置相似度并显示最佳结果"

      # feature loop
      - icon: "fas fa-file-word"
        content: "通过模糊搜索智能管理错别字"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Use 分面和布尔值 Search Simultaneously"

      # feature loop
      - icon: "fas fa-print"
        content: "配置和执行同义词搜索并巧妙地处理谐音词"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "使用日期范围和区分大小写作为搜索参数"

      # feature loop
      - icon: "fas fa-lock"
        content: "通过 Aspose.Email API 建立索引以搜索和浏览电子邮件"

      # feature loop
      - icon: "fas fa-file-code"
        content: "使用带有拼写检查和外卡的搜索短语并在查询中跳过特殊字符"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "通过组合多个查询制作单个对象树"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "将搜索划分为更小的块以快速搜索巨大的索引"

      # feature loop
      - icon: "fas fa-heading"
        content: "来自流和数据结构的索引文档"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "在搜索结果中设置文档过滤"

      # feature loop
      - icon: "fas fa-cube"
        content: "将英语同义词添加到默认同义词词典"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "为每个找到的单词启用准确的出现次数，以在拼写错误的情况下提供替代单词建议"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "将文本属性添加到索引文档而不重新索引"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "基于字符执行索引和搜索操作"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "非文本文档格式的索引元数据"

    more_feature:
      # more_feature_loop
      - title: "索引 and Search Operation"
        content: |
          GroupDocs.Search for Java 使用索引来收集数据，并存储和解析数据以实现准确高效的搜索操作。 GroupDocs.Search for Java 经常使用此类索引来执行搜索。

          * **创建索引**：创建索引文件夹并将文档添加/索引到该文件夹​​。
          * **加载索引**：加载现有索引。
          * **将文档添加到索引**：将文档异步添加到现有索引。
          * **更新索引**：在修改、添加或删除文档时更新现有索引。这使搜索结果保持最新。
          
          ```java
          / 创建索引
          Index index = new Index("c:\\MyIndex");
          // 将文档添加到索引
          index.addToIndex("c:\\MyDocuments");
          // 在文档中搜索单词“影响”或“影响 'principal', 'principle', 'principles', or 'principally'
          SearchResults results = index.search("?ffect & princip?(2~4)");
          ```
      # more_feature_loop
      - title: "合并多个索引以提高搜索效率"
        content: "GroupDocs.Search for Java API 提供了将多个索引合并为一个公共索引的功能。对于经常修改的索引，会创建多个增量索引。然而，这种方法会使搜索性能变慢。 GroupDocs.Search for Java 通过合并各种 delta 索引来创建一个通用索引，从而克服了这一瓶颈。这个共同的合并索引包含合并的增量索引的所有信息。这种方法在保持增量索引不变的同时显着提高了搜索效率。您可以配置各种功能以进一步调整此过程."

      # more_feature_loop
      - title: "识别不同键盘布局的搜索查询"
        content: "GroupDocs.Search for Java 可识别与您的键盘布局不匹配的搜索查询。目前，GroupDocs.Search for Java 可以成功识别 88 种语言和 164 种不同的键盘布局。"

      # more_feature_loop
      - title: "使用形态词形式搜索"
        content: "使用 GroupDocs.Search for Java，您可以自由搜索各种单词形式。您可以搜索特定名词的单数和复数形式。或者您可以选择搜索动词的所有形式。还可以搜索词根、第三人称单数和一般过去时以及各种其他形式。对于非英语语言，您可以配置自定义单词形式."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Search 为其他流行的开发环境提供文档查看 API"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Search for .NET"
          image: "/border/groupdocs-search-net.svg"
          product: "GroupDocs.Search"
          platform: ".NET"
          link: "/search/net/"

        # solution loop
        - img_alt: "GroupDocs.Search for Node.js"
          image: "/border/groupdocs-search-nodejs-java.svg"
          product: "GroupDocs.Search"
          platform: "Node.js via Java"
          link: "/search/nodejs-java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---