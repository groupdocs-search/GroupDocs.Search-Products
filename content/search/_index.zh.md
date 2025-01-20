---
############################# Static ############################
layout: "family"
date:  2025-01-20T14:28:24
draft: false

product: "Search"
product_tag: "search"

lang: zh

############################# Head ############################
head_title: "文档文本搜索和索引 | API和免费网络应用"
head_description: "使用我们的API或免费在线文档搜索应用程序，在PDF、MS Office、OpenDocument和其他流行文件格式上执行高效文本搜索和数据索引。"

############################# Header ############################
title: "综合文档搜索和索引解决方案"
description:  |
  在PDF、Microsoft Office、OpenOffice和许多其他文档文件格式上执行文本搜索和索引。

  借助先进的全文搜索功能，快速定位大型文档集合中的信息。

  自定义搜索功能，如同义词、模糊搜索和词干提取，以提高准确性和结果。

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "选择您的平台"
  title: "平台独立性"
  description: "GroupDocs.Search 与以下操作系统和框架兼容："
  details_link_title: "了解更多"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Search .NET 
      color: "blue"
      tag: "net"
      link: "/search/net/"
      features_link: "https://docs.groupdocs.com/search/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.5 or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Search Java
      color: "red"
      tag: "java"
      link: "/search/java/"
      features_link: "https://docs.groupdocs.com/search/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java SE 8 (1.8) or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Node.js"
      description: GroupDocs.Search Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/search/nodejs-java/"
      features_link: "https://docs.groupdocs.com/search/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> 任何其他文本编辑器
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats


############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Search 的主要功能"
  description: "GroupDocs.Search 提供强大的工具，用于在流行的文档格式中进行索引和搜索文本。通过先进的搜索功能简化和增强文档管理。"

  items:
    # items loop
    - icon: "view"
      title: "高级文本搜索"
      content: "在索引文档中执行快速且准确的文本搜索。"

    # items loop
    - icon: "manipulate"
      title: "可定制搜索选项"
      content: "利用模糊搜索、同义词和词干提取等功能，以获取更精确的结果。"

    # items loop
    - icon: "merge"
      title: "支持多种格式"
      content: "在Microsoft Office、PDF、OpenOffice 和其他常见格式中索引和搜索内容。"

    # items loop
    - icon: "additional"
      title: "高效索引"
      content: "快速构建和维护大型文档集合的索引。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "在流行文档格式中搜索文本"
  description: "GroupDocs.Search 代码示例"
  items:
    # code sample loop
    - title: "文本搜索"
      content: |
       GroupDocs.Search 是一个强大的工具，用于在文档中查找文本。您可以在特定文件夹中搜索多个不同格式的文档。搜索结果保存在单独的文件夹中，允许您访问和重用，而无须再次进行搜索。
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // 创建一个 Index 类的实例，指定用于存储索引的文件夹。
            Index index = new Index("\\Index Folder");

            //指定将在其中进行搜索的文档路径。
            index.Add("\\Documents Folder");

            //创建 SearchOptions 对象的实例。
            SearchOptions options = new SearchOptions();

            //执行所需文本的搜索。
            SearchResult result = index.Search("ipsum dolor", options);

            //处理和处理搜索结果。
            if (result.DocumentCount > 0){
                Console.WriteLine("Documents: " + result.DocumentCount);
                for (int i = 0; i < result.DocumentCount; i++)
                {
                    FoundDocument document = result.GetFoundDocument(i);
                    Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
                    Console.WriteLine("Found: " + document.FoundFields.Length);
                }
            }

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // 创建一个 Index 类的实例，指定用于存储索引的文件夹。
            Index index = new Index("\\Index Folder");

            //指定将在其中进行搜索的文档路径。
            index.add("\\Documents Folder");

            //创建 SearchOptions 对象的实例。
            SearchOptions options = new SearchOptions();

            //执行所需文本的搜索。
            SearchResult result = index.search("ipsum dolor", options);

            //处理和处理搜索结果。
            if (result.getDocumentCount() > 0){
                System.out.println("Documents: " + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    FoundDocument document = result.getFoundDocument(i);
                    System.out.println("Document: " + document.getDocumentInfo().getFilePath());
                    System.out.println("Found: " + document.getFoundFields().length);
                }
            }

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const searchLib = require('@groupdocs/groupdocs.search');

            // 创建一个 Index 类的实例，指定用于存储索引的文件夹。
            const index = new searchLib.Index('\\Index Folder');

            //指定将在其中进行搜索的文档路径。
            index.add('\\Documents Folder');

            //创建 SearchOptions 对象的实例。
            const options = new searchLib.SearchOptions();

            //执行所需文本的搜索。
            const result = index.search('ipsum dolor', options);

            //处理和处理搜索结果。
            if (result.getDocumentCount() > 0){
                console.log('Documents: ' + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    const document = result.getFoundDocument(i);
                    console.log('Document: ' + document.getDocumentInfo().getFilePath());
                    console.log('Found: ' + document.getFoundFields().length);
                }
            }

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "支持70多种文件格式"
  description: "GroupDocs.Search几乎支持所有广泛使用的文件格式"

############################# Metrics ###############################
metrics:
  enable: true
  title: "我们的产品统计"
  description: "发现展示我们性能、覆盖范围和增长的关键指标。"

  items:
    # items loop
    - number: "70+"
      title: "支持的格式"
      content: "我们提供超过70种流行文档格式的兼容性。"

    # items loop
    - number: "500k"
      title: "NuGet下载"
      content: "GroupDocs.Search for .NET 在NuGet上已被下载超过500,000次。"

    # items loop
    - number: "12k"
      title: "Maven下载"
      content: "Java开发者在Maven上下载了GroupDocs.Search超过12,000次。"

    # items loop
    - number: "150+"
      title: "满意的客户"
      content: "全球开发者和领先企业依赖我们的产品提供创新解决方案。"


############################# Customers ###############################
customers:
  enable: true
  title: "我们的满意客户"
  description: "GroupDocs库获得全球领先品牌和组织的信任。"

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "今天就开始您的旅程！"
  description: "在您首选的平台上体验GroupDocs.Search的免费服务。"

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/search/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/search/java/"

    # items loop
    - title: "Node.js via Java"
      color: "green"
      link: "/search/nodejs-java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "常见问题"
  description: "查找有关GroupDocs.Search的常见问题答案。"

  items:
    # items loop
    - question: "GroupDocs.Search是否需要外部工具来搜索文档？"
      answer: "不需要，GroupDocs.Search作为独立解决方案工作，无需其他工具或软件（如Adobe Acrobat或Microsoft Office）即可执行搜索。"

    # items loop
    - question: "我可以在购买之前测试GroupDocs.Search吗？"
      answer: "可以！GroupDocs.Search提供免费试用。您可以探索其特点，尽管试用版本可能包含水印或功能限制。要解锁所有功能，请申请免费的30天临时许可。了解更多信息，请访问[临时许可](https://purchase.groupdocs.com/temporary-license/)页面。"

    # items loop
    - question: "有哪些许可选项可供选择？"
      answer: "我们为GroupDocs.Search提供几种许可模式，以满足不同的需求。根据团队规模、使用场景或是否需要SDK/API进行客户端分发，选择一种许可。为了灵活使用，您可以考虑按照实际使用量支付的计量许可。有关您的选项的更多信息，请访问[定价](https://purchase.groupdocs.com/pricing/search/net/)页面。"

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Search 网络应用"
  description: "使用我们的免费网络应用程序探索 GroupDocs.Search。直接在您的浏览器中对超过70种流行文件格式执行文本搜索和索引——完全免费。"

  items:
    # items loop
    - title: "GroupDocs.Search Total"
      content: "直接从网页浏览器中搜索PDF、Excel、Word、PowerPoint和其他文件类型。"
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/search/total"

    # items loop
    - title: "GroupDocs.Search Word"
      content: "上传DOCX以便执行不需要安装软件的高级文本搜索。"
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/search/docx"

    # items loop
    - title: "GroupDocs.Search PDF"
      content: "免费测试PDF的索引和检索功能，支持各种格式。"
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/search/pdf"


---