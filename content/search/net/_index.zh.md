---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C# .NET 文本搜索和索引 API for Word Excel PDF 电子邮件 HTML"
head_description: "C# .NET 文本搜索 API 智能地索引和检索 PDF、MS Office Word、Excel、演示文稿、OneNote、电子邮件、ZIP、EPUB 和 Web 文件中的数据。"

############################# Header ############################
title: ".NET API 来搜索和索引文档"
description: "在所有流行文档格式中使用 .NET 应用程序索引数据和执行文本搜索的 API."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Search for .NET"
        image: "/border/groupdocs-search-net.svg"
        product: "GroupDocs.Search"
        platform: ".NET"

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
            - link: "https://purchase.groupdocs.com/pricing/search/net"
              text: "价钱"

    right:
        link_download: "https://downloads.groupdocs.com/search"
        link_learn: "https://docs.groupdocs.com/search/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# 概述 ############################
overview:
    enable: true
    content: |
      GroupDocs.Search for .NET 是一个文档和文本搜索 API，用于使用 C#、ASP.NET 和其他 .NET 技术开发的业务应用程序。这个 .NET API 支持从基本到高级的搜索功能，例如，创建和合并多个索引，使用简单的、布尔值、模糊、正则表达式 (regex) 和其他查询类型搜索索引以从文件、文档中获取所需的数据和电子邮件，通过智能搜索。如果您想为您的最终用户构建一个快速、可靠、智能且功能丰富的搜索应用程序，支持所有流行的文件格式，GroupDocs.Search for .NET 就是您所需要的。
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          以下是 GroupDocs.Search for .NET 的概述：
      
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
          GroupDocs.Search for .NET 支持以下 [文档文件格式](https://docs.groupdocs.com/search/net/supported-document-formats/)：

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
          GroupDocs.Search .NET 支持以下操作系统、框架和包管理器:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "操作系统"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux

            # table loop
            - icon: "fas fa-code"
              title: "支持的框架"
              content: |
                * .NET Framework 2.0 或更高版本
                * Mono 框架 1.2 或更高版本
                * .NET 标准 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "包管理器"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "开发环境"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# 特征 ############################
features:
    enable: true
    title: "GroupDocs.Search for .NET 特征"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "在内存或磁盘上创建索引并执行多线程索引和合并"

      # feature loop
      - icon: "fas fa-eye"
        content: "防止已索引文件或名称中包含特定字符串的索引"

      # feature loop
      - icon: "fas fa-bolt"
        content: "查看索引创建和更新的进度百分比并获取搜索报告"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "通过排除最近处理的文件的特定单词和索引状态通知来加快索引"

      # feature loop
      - icon: "fas fa-code"
        content: "在 ZIP 存档中索引 ZIP 存档并获取存档中包含的索引文件列表"

      # feature loop
      - icon: "fas fa-cloud"
        content: "在索引期间使用列表或导入替换字符并将它们导出到文件"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "索引和搜索受密码保护的文件和紧凑索引以节省磁盘空间"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "从索引或源文件中提取文本并在索引中自动保存文本文件编码"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "在索引期间向每个文档添加任意附加字段"

      # feature loop
      - icon: "fas fa-border-all"
        content: "在搜索结果中设置文档过滤"

      # feature loop
      - icon: "fas fa-wrench"
        content: "通过模糊搜索处理输入错误，在模糊搜索中设置相似度并仅显示最佳结果"

      # feature loop
      - icon: "fas fa-columns"
        content: "来自流和数据结构的索引文档"

      # feature loop
      - icon: "fas fa-file-word"
        content: "使用停用词搜索完整短语并将分面搜索与布尔搜索相结合"

      # feature loop
      - icon: "fas fa-envelope"
        content: "根据谐音词、同义词、日期范围、外卡和区分大小写进行搜索"

      # feature loop
      - icon: "fas fa-print"
        content: "使用 Aspose.Email API 索引和搜索 Outlook 中的电子邮件和浏览"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "支持搜索查询中的拼写检查和外卡和跳过搜索短语中的特殊字符"

      # feature loop
      - icon: "fas fa-lock"
        content: "限制搜索查询中每个术语以及所有结果的结果"

      # feature loop
      - icon: "fas fa-file-code"
        content: "将 HTML 文本提取到文件并生成 URL 以导航 HTML 格式的搜索结果"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "将多个查询组合成单个对象树"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "在索引错误的情况下提醒用户非支持设置和自动索引重新加载"

      # feature loop
      - icon: "fas fa-heading"
        content: "为每个找到的单词启用准确的出现次数，以在拼写错误的情况下提供替代单词建议"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "将文本属性添加到索引文档而不重新索引"

      # feature loop
      - icon: "fas fa-cube"
        content: "基于字符执行索引和搜索操作"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "非文本文档格式的索引元数据"

    more_feature:
      # more_feature_loop
      - title: "索引 & Search"
        content: |
          GroupDocs.Search for .NET API 经常使用索引来执行搜索。索引用于收集、解析或存储数据，以实现快速准确的搜索。

          * **创建索引**：创建索引文件夹并将文档添加/索引到该文件夹​​。
          * **加载索引**：加载现有索引。
          * **将文档添加到索引**：将文档异步添加到现有索引。
          * **更新索引**：在修改、添加或删除文档时更新现有索引。这使搜索结果保持最新。

          ```cs
           // 创建索引
          Index  index = new Index(@"c:\MyIndex");
          // 将文档添加到索引
          index.AddToIndex(@"c:\MyDocuments");
          // 在索引中搜索
          SearchResults searchResults =  index.Search("searchTerm");
          ```
      # more_feature_loop
      - title: "合并多个索引以提高搜索效率"
        content: "GroupDocs.Search for .NET 能够将多个索引合并为一个单一索引。如果一个索引经常更新，它有几个增量索引，但这种方法会降低搜索性能。 GroupDocs.Search for .NET API 将所有增量索引合并到一个合并索引中。主合并索引将包含来自合并增量索引的所有信息；但是，delta 指数将保持不变。我们的 API 使用的这种方法大大提高了搜索效率。索引合并功能，提供许多功能来调整以进一步调整此过程。"

      # more_feature_loop
      - title: "在索引中存储文本以生成 HTML 标记"
        content: "GroupDocs.Search for .NET 可以在索引中缓存索引文档的文本。然后，此缓存文本用于通过突出显示搜索结果快速生成 HTML 标记。这种方法比直接从文件中提取文本要快得多。即使源文件不再可用，也可以从缓存中检索文本。可以通过应用各种压缩级别来存储缓存的文本以占用更少的磁盘空间和更快的索引时间."

      # more_feature_loop
      - title: "通过模糊和正则表达式搜索获取相关文档"
        content: "当您执行模糊或正则表达式搜索时，您可以获得与您提供的输入完全匹配的文档列表。但是，您还将获得包含与您的输入相似的单词或术语的文档列表。例如，如果使用 GroupDocs.Search for .NET，对查询“cost”执行模糊搜索，您将获得包含单词“cost”的文档和包含类似单词（如“coat”）的文档。结果将取决于您使用此 API 配置的模糊程度."

      # more_feature_loop
      - title: "识别不同键盘布局的搜索查询"
        content: "GroupDocs.Search for .Net 可以识别以与您的键盘布局不匹配的语言编写的搜索查询。目前，这个 .NET API 可以成功识别 88 种语言和 164 种不同的键盘布局."

      # more_feature_loop
      - title: "使用形态词形式搜索"
        content: "GroupDocs.Search for .NET API 允许您搜索各种单词形式。例如，对于一个名词，您可以搜索其单数和复数形式。对于动词，您可以搜索该动词的所有形式。您还可以搜索词根、第三人称单数、一般过去时和其他各种形式。对于英语以外的语言，您可以实现自定义单词形式."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Search 为其他流行的开发环境提供文档查看 API"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Search for Java"
          image: "/border/groupdocs-search-java.svg"
          product: "GroupDocs.Search"
          platform: "Java"
          link: "/search/java/"

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
