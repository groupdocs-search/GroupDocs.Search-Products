---
############################# Static ############################
layout: "landing"
date: 2024-07-04T14:43:38
draft: false

lang: zh
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js 用于文档、PDF、Office 和 Web 的文本搜索和索引库"
head_description: "适用于 Node.js 应用程序的高级文本搜索解决方案，用于搜索、索引和收集文档中的数据：PDF、Word、Excel、演示文稿、电子邮件和网络文件格式。"

############################# Header ############################
title: "使用 Node.js API 搜索和索引文档"
description: "通过在所有流行文档格式中实施文本搜索来增强 Node.js 应用程序。"
words:
  for: "为了"

actions:
  main: "免费 NPM 下载"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "许可"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "准备好开始了吗？"
  description: "免费试用 GroupDocs.Search 功能或申请许可证"

release:
  title: "版本 {0} 已发布"
  notes: "看看有什么新鲜事"
  downloads: "下载"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "在带有 JavaScript 的文件夹中搜索"
  more: "更多示例"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    // 创建索引
    const index = new Index('c:/MyIndex');

    // 将文档添加到索引
    index.add('c:/MyDocuments');
    
    // 搜索各种单词，例如
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search 一目了然"
  description: "用于文本搜索的 Node.js JavaScript 库"
  features:
    # feature loop
    - title: "Node.js 索引和搜索操作"
      content: "GroupDocs.Search for Node.js via Java 中的索引收集、存储和解析数据，以实现精确、高效的搜索操作。这些索引经常用于执行搜索。"

    # feature loop
    - title: "合并多个索引以提高搜索效率"
      content: "GroupDocs.Search for Node.js via Java API 允许将多个索引合并为一个。频繁的修改会创建多个增量索引，这会降低搜索性能。我们的解决方案将这些增量索引合并为一个公共索引，包含合并后增量索引的所有信息，在保持增量索引不变的情况下显着提高搜索效率。可以配置各种功能来微调此过程。"

    # feature loop
    - title: "识别不同键盘布局的搜索查询"
      content: "GroupDocs.Search for Node.js via Java 可以识别与键盘布局不匹配的搜索查询。目前支持 88 种语言和 164 种不同的键盘布局。"

    # feature loop
    - title: "使用形态词形式进行搜索"
      content: "使用 GroupDocs.Search for Node.js via Java，您可以搜索各种单词形式，例如单数和复数名词，或动词的所有形式。英语和非英语语言可以定制特定的词形。"

############################# Platforms ############################
platforms:
  enable: true
  title: "平台独立性"
  description: "GroupDocs.Search for Node.js via Java 支持所有流行的操作系统和包管理器。"
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "支持的文件格式"
  description: |
    GroupDocs.Search for Node.js via Java 可以处理多种文件格式。 [浏览完整列表](https://docs.groupdocs.com/search/java/supported-document-formats/)。
  groups:
    # group loop
    - color: "green"
      content: |
        ### 流行的办公格式
        * **便携的:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **文本:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### 媒体格式
        * **流行的图像格式:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **多页图像:** GIF, WEBP, TIFF
        * **声音的:** MP3, WAV
        * **视频:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### 其他
        * **电子邮件:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **网络:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **其他的:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Search for Node.js via Java 功能"
  description: "使用我们的高级搜索引擎控制业务文档内容，支持流行的文件格式，包括 PDF、DOCX、XLSX、PPTX 等。"

  items:
    # feature loop
    - icon: "document_info"
      title: "灵活的参数"
      content: "使用日期范围和区分大小写作为搜索参数"

    # feature loop
    - icon: "detect"
      title: "拼写检查搜索"
      content: "使用带有拼写检查和通配符的搜索短语并在查询中跳过特殊字符"

    # feature loop
    - icon: "collect"
      title: "结果过滤"
      content: "在搜索结果中设置文档过滤"

    # feature loop
    - icon: "get"
      title: "进出口"
      content: "在索引和导出到文件期间执行导入或使用列表修改字符"

    # feature loop
    - icon: "remove"
      title: "跳过不必要的数据"
      content: "有选择地跳过特定文件的索引并跳过特定单词以更快地建立索引"

    # feature loop
    - icon: "style"
      title: "网址处理"
      content: "将 HTML 格式的文本提取到文件并生成 URL 以在 HTML 中导航搜索结果"

    # feature loop
    - icon: "detect"
      title: "快速搜索"
      content: "将搜索分成较小的块以快速搜索大型索引"

    # feature loop
    - icon: "manipulate"
      title: "流处理"
      content: "从流和数据结构中索引文档"

    # feature loop
    - icon: "compare"
      title: "处理拼写错误"
      content: "为每个找到的单词启用准确的出现次数，以便在出现拼写错误时提供替代单词建议"

    # feature loop
    - icon: "unreadable_characters"
      title: "存档支持"
      content: "在其他 ZIP 档案中索引压缩档案并检索档案中的索引文件列表"

    # feature loop
    - icon: "hidden_print"
      title: "节省磁盘空间"
      content: "通过紧凑索引和索引密码保护文档节省空间"

    # feature loop
    - icon: "style"
      title: "自定义同义词"
      content: "将英语同义词添加到默认同义词词典"

############################# Code samples ############################
code_samples:
  enable: true
  title: "代码示例"
  description: "通过示例探索 GroupDocs.Search for Node.js via Java 功能"
  items:
    # code sample loop
    - title: "使用模糊搜索提高生产力"
      content: |
        享受灵活的 GroupDocs.Search for Node.js via Java 功能，通过复杂的搜索算法增强文档内容控制。 [了解更多](https://docs.groupdocs.com/search/java/search-results/)。
        {{< landing/code title="如何处理搜索结果">}}
        ```javascript {style=abap}
        // 创建索引
        const index = new Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // 设置搜索选项
        var options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // 搜索包含单词“water”或短语“Lorem ipsum”的文档
        var query = "water OR \"Lorem ipsum\"";
        var result = index.search(query, options);
        
        // 处理搜索结果
        console.log("Documents: " + result.getDocumentCount());
        console.log("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            console.log('Document: ${document.getDocumentInfo().getFilePath()}');
            console.log('Occurrences: ${document.getOccurrenceCount()}');
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "正则表达式可用于高级搜索场景"
      content: |
        GroupDocs.Search for Node.js via Java 允许我们使用正则表达式来缩小搜索结果范围。 [深入研究高级搜索技术](https://docs.groupdocs.com/search/java/regular-expression-search/)。
        {{< landing/code title="如何使用正则表达式进行搜索">}}
        ```javascript {style=abap}   
        // 创建索引
        const index = new Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // 以文本形式搜索短语

        // 开头的第一个插入字符表示这是正则表达式搜索查询
        var query = "^^(.)\\1{1,}";
        // 搜索单词开头的两个或多个相同字符
        var result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
