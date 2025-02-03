---
############################# Static ############################
layout: "landing"
date: 2025-02-03T08:17:12
draft: false

lang: zh
product: "Search"
product_tag: "search"
platform: "Net"
platform_tag: "net"

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
head_title: ".NET 文档搜索和索引库，支持PDF、Office文件等"
head_description: "强大的.NET解决方案，用于在文档（如PDF、Word、Excel、演示文稿、电子邮件和网页格式）中进行文本搜索和索引。"

############################# Header ############################
title: "使用.NET API进行高级文档搜索和索引"
description: "提升.NET应用程序，通过流行文档格式提供尖端文本搜索能力。"
words:
  for: "为"

actions:
  main: "免费下载Nuget"
  main_link: "https://www.nuget.org/packages/GroupDocs.Search"
  alt: "许可"
  alt_link: "https://purchase.groupdocs.com/pricing/search/net/"
  title: "今天就开始您的旅程！"
  description: "免费体验GroupDocs.Search的功能，或申请许可以解锁其全部潜力。"

release:
  title: "版本 {0} 已发布"
  notes: "查看新功能"
  downloads: "下载"

code:
  title: "在目录文件中搜索文本"
  more: "更多示例"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
  install: "dotnet add package GroupDocs.Search"
  content: |
    ```csharp {style=abap}   
    // 为您的文档创建索引
    Index index = new Index("c:/MyIndex");

    // 将文档添加到索引中以实现高效搜索
    index.Add("c:/MyDocuments");
    
    // 搜索特定单词或短语，例如
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.Search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search 概述"
  description: "探索.NET C#库，以实现强大的文本搜索和索引。"
  features:
    # feature loop
    - title: ".NET 索引和搜索功能"
      content: "有效索引、存储和处理文档数据，使用GroupDocs.Search for .NET进行高精度和快速搜索操作。"

    # feature loop
    - title: "合并索引以提高搜索速度"
      content: "GroupDocs.Search for .NET允许您合并多个索引以优化性能。通过将多个增量索引合并为一个综合索引，减少增量索引的影响，以实现更顺畅的搜索。"

    # feature loop
    - title: "跨不同键盘布局搜索"
      content: "使用GroupDocs.Search for .NET的智能识别，轻松处理来自88种语言和164种键盘布局的搜索查询。"

    # feature loop
    - title: "形态学单词搜索"
      content: "GroupDocs.Search for .NET支持对单词变化（如单数/复数名词和不同动词形式）进行搜索，可以针对不同语言进行自定义。"

############################# Platforms ############################
platforms:
  enable: true
  title: "平台独立性"
  description: "GroupDocs.Search for .NET 在各大操作系统和软件包管理器中无缝工作。"
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "支持的文件格式"
  description: |
    使用GroupDocs.Search for .NET处理各种文件格式。[查看所有支持的格式](https://docs.groupdocs.com/search/net/supported-document-formats/)。
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
  title: "GroupDocs.Search for .NET 的主要功能"
  description: "通过在流行格式（如PDF、DOCX、XLSX、PPTX等）中提供高级搜索能力，简化文档管理。"

  items:
    # feature loop
    - icon: "document_info"
      title: "灵活的搜索参数"
      content: "使用日期范围和区分大小写等筛选器来改进搜索。"

    # feature loop
    - icon: "detect"
      title: "智能拼写检查"
      content: "使用拼写纠正、通配符和忽略特殊字符的搜索短语。"

    # feature loop
    - icon: "collect"
      title: "过滤搜索结果"
      content: "按文档类型或标准自定义和过滤搜索结果。"

    # feature loop
    - icon: "get"
      title: "索引导入与导出"
      content: "导入数据，修改索引设置，并导出已索引的结果。"

    # feature loop
    - icon: "remove"
      title: "排除无关数据"
      content: "通过跳过特定文件或单词来优化索引。"

    # feature loop
    - icon: "style"
      title: "URL提取"
      content: "将HTML格式的文本转换为文件，并为搜索结果生成链接。"

    # feature loop
    - icon: "detect"
      title: "高速搜索"
      content: "将大索引划分为小部分，以便更快地处理。"

    # feature loop
    - icon: "manipulate"
      title: "简化数据处理"
      content: "直接从数据流和结构中索引文档。"

    # feature loop
    - icon: "compare"
      title: "拼写错误检测"
      content: "建议替代词，并跟踪发生次数以提高准确性。"

    # feature loop
    - icon: "unreadable_characters"
      title: "归档支持"
      content: "索引嵌套ZIP归档，并检索其中的文件详细信息。"

    # feature loop
    - icon: "hidden_print"
      title: "高效索引"
      content: "通过紧凑的索引节省磁盘空间，并处理密码保护的文档。"

    # feature loop
    - icon: "style"
      title: "自定义同义词"
      content: "添加和管理同义词，以实现定制的搜索结果。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "代码示例"
  description: "通过示例发现GroupDocs.Search for .NET的强大能力。"
  items:
    # code sample loop
    - title: "通过模糊搜索提升生产力"
      content: |
        利用GroupDocs.Search for .NET的先进搜索算法，通过灵活和准确的内容控制。 [探索更多](https://docs.groupdocs.com/search/net/search-results/)。
        {{< landing/code title="如何处理搜索结果">}}
        ```csharp {style=abap}
        // 创建索引
        Index index = new Index("C:/IndexFolder");
        index.Add("C:/DocumentFolder");

        // 设置搜索选项
        SearchOptions options = new SearchOptions();
        options.FuzzySearch.Enabled = true;
        options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3);

        // 搜索包含'water'这个词或短语'Lorem ipsum'的文档
        string query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.Search(query, options);
        
        // 处理搜索结果
        Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
        Console.WriteLine("Occurrences: " + document.OccurrenceCount);
        for (int i = 0; i < result.DocumentCount; i++) {
            FoundDocument document = result.GetFoundDocument(i);
            Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
            Console.WriteLine("Occurrences: " + document.OccurrenceCount);
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "使用正则表达式进行高级搜索"
      content: |
        GroupDocs.Search for .NET支持正则表达式进行精准搜索。 [了解先进技术](https://docs.groupdocs.com/search/net/regular-expression-search/)。
        {{< landing/code title="如何使用正则表达式搜索">}}
        ```csharp {style=abap}   
        // 创建索引
        Index index = new Index("c:/IndexFolder");
        index.Add("c:/DocumentFolder");
 
        // 搜索文本形式的短语

        // 第一个插入符号字符表示这是一个正则表达式搜索查询
        string query = "^^(.)\\1{1,}";
        // 搜索单词开头的两个或多个相同字符
        SearchResult result = index.Search(query);
 
        ```
        {{< /landing/code >}}

---
