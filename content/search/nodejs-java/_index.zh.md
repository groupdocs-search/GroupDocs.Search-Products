---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
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
head_title: "Node.js 文本搜索和索引库，支持文档、PDF、Office和网页"
head_description: "针对Node.js应用程序的高级文本搜索解决方案，以搜索、索引和收集文档中的数据：PDF、Word、Excel、演示文稿、电子邮件和网页文件格式。"

############################# Header ############################
title: "使用Node.js API搜索和索引文档"
description: "通过在所有流行文档格式中实施文本搜索，增强Node.js应用程序。"
words:
  for: "为"

actions:
  main: "免费NPM下载"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "许可"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "今天就开始您的旅程！"
  description: "免费体验GroupDocs.Search的功能，或申请许可以解锁其全部潜力。"

release:
  title: "版本 {0} 已发布"
  notes: "查看新功能"
  downloads: "下载"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "使用JavaScript在文件夹中执行文本搜索"
  more: "更多示例"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    const searchLib = require('@groupdocs/groupdocs.search');

    // 为您的文档创建索引
    const index = new searchLib.Index('c:/MyIndex');

    // 将文档添加到索引中以实现高效搜索
    index.add('c:/MyDocuments');
    
    // 搜索特定单词或短语，例如
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search 概述"
  description: "Node.js JavaScript库进行文本搜索"
  features:
    # feature loop
    - title: "Node.js 索引和搜索操作"
      content: "在GroupDocs.Search for Node.js via Java中进行索引，收集、存储和解析数据，以实现精确和高效的搜索操作。这些索引通常用于执行搜索。"

    # feature loop
    - title: "合并多个索引以增强搜索效率"
      content: "GroupDocs.Search for Node.js via Java API允许将多个索引合并为一个。频繁的修改会创建多个增量索引，可能会减慢搜索性能。我们的解决方案将这些增量索引合并为一个公共索引，包含所有合并增量索引的信息，显著提高搜索效率，同时保持增量索引不变。可以配置多种功能以微调此过程。"

    # feature loop
    - title: "识别来自不同键盘布局的搜索查询"
      content: "GroupDocs.Search for Node.js via Java可以识别与键盘布局不匹配的搜索查询。目前支持88种语言和164种不同的键盘布局。"

    # feature loop
    - title: "使用形态学单词形式搜索"
      content: "使用GroupDocs.Search for Node.js via Java，您可以搜索多种单词形式，例如单数和复数名词，或动词的所有形式。英语和非英语语言可以针对特定单词形式进行自定义。"

############################# Platforms ############################
platforms:
  enable: true
  title: "平台独立性"
  description: "GroupDocs.Search for Node.js via Java支持所有流行操作系统和软件包管理器。"
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
    GroupDocs.Search for Node.js via Java可以处理广泛的文件格式。[探索完整列表](https://docs.groupdocs.com/search/nodejs-java/supported-document-formats/)。
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
  title: "GroupDocs.Search for Node.js via Java 的功能"
  description: "使用我们的高级搜索引擎控制业务文档内容，支持流行的文件格式，包括PDF、DOCX、XLSX、PPTX等。"

  items:
    # feature loop
    - icon: "document_info"
      title: "灵活参数"
      content: "使用日期范围和区分大小写作为搜索参数"

    # feature loop
    - icon: "detect"
      title: "拼写检查搜索"
      content: "使用拼写检查和通配符的搜索短语，跳过查询中的特殊字符"

    # feature loop
    - icon: "collect"
      title: "结果过滤"
      content: "在搜索结果中设置文档过滤"

    # feature loop
    - icon: "get"
      title: "导入和导出"
      content: "导入或使用列表修改索引期间的字符，并导出到文件"

    # feature loop
    - icon: "remove"
      title: "跳过不必要的数据"
      content: "有选择性地跳过特定文件的索引，和跳过特定单词以更快地索引"

    # feature loop
    - icon: "style"
      title: "URL处理"
      content: "提取HTML格式的文本到文件，并生成URL以在HTML中导航搜索结果"

    # feature loop
    - icon: "detect"
      title: "快速搜索"
      content: "将搜索分解为更小的块，以快速搜索大型索引"

    # feature loop
    - icon: "manipulate"
      title: "流处理"
      content: "从流和数据结构中索引文档"

    # feature loop
    - icon: "compare"
      title: "处理拼写错误"
      content: "为每个找到的单词提供准确的出现次数，并在拼写错误时提供替代词建议"

    # feature loop
    - icon: "unreadable_characters"
      title: "归档支持"
      content: "索引嵌套的ZIP归档，并检索归档中索引文件的列表"

    # feature loop
    - icon: "hidden_print"
      title: "节省磁盘空间"
      content: "以压缩的方式索引，占用更少空间，并索引密码保护的文档"

    # feature loop
    - icon: "style"
      title: "自定义同义词"
      content: "将英语同义词添加到默认同义词字典"

############################# Code samples ############################
code_samples:
  enable: true
  title: "代码示例"
  description: "通过示例探索GroupDocs.Search for Node.js via Java的功能"
  items:
    # code sample loop
    - title: "使用'模糊'搜索提升生产力"
      content: |
        享受GroupDocs.Search for Node.js via Java的灵活功能，通过复杂的搜索算法增强文档内容控制。[了解更多](https://docs.groupdocs.com/search/nodejs-java/search-results/)。
        {{< landing/code title="如何处理搜索结果">}}
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search');

        // 创建索引
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // 设置搜索选项
        const options = new searchLib.SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // 搜索包含'water'这个词或短语'Lorem ipsum'的文档
        const query = 'water OR "Lorem ipsum"';
        const result = index.search(query, options);
        
        // 处理搜索结果
        console.log('Documents: ' + result.getDocumentCount());
        console.log('Total occurrences: ' + result.getOccurrenceCount());
        for (let i = 0; i < result.getDocumentCount(); i++) {
            const document = result.getFoundDocument(i);
            console.log('Document: ' + document.getDocumentInfo().getFilePath());
            console.log('Occurrences:  + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "正则表达式可用于高级搜索场景"
      content: |
        GroupDocs.Search for Node.js via Java允许我们使用正则表达式来缩小搜索结果。[深入了解高级搜索技术](https://docs.groupdocs.com/search/nodejs-java/regular-expression-search/)。
        {{< landing/code title="如何使用正则表达式搜索">}}
        ```javascript {style=abap}   
        const searchLib = require('@groupdocs/groupdocs.search');

        // 创建索引
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // 搜索文本形式的短语

        // 第一个插入符号字符表示这是一个正则表达式搜索查询
        const query = '^^(.)\\1{1,}';
        // 搜索单词开头的两个或多个相同字符
        const result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
