<% configRef "..\\..\\configs\\index\\index_nodejs.yml" %>
<% include "..\\..\\data\\platform_data.md" %>
---
############################# Static ############################
layout: "landing"
date: <% date "utcnow" %>
draft: false

lang: <% lower ( get "lang") %>
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
head_title: "<% "{index-content-nodejs-java.head_title}" %>"
head_description: "<% "{index-content-nodejs-java.head_description}" %>"

############################# Header ############################
title: "<% "{index-content-nodejs-java.title}" %>"
description: "<% "{index-content-nodejs-java.description}" %>"
words:
  for: "<% "{index-content.words_for}" %>"

actions:
  main: "<% "{index-content-nodejs-java.actions_main}" %>"
  main_link: "<% get "PackageUrl" %>"
  alt: "<% "{index-content.actions.alt}" %>"
  alt_link: "<% get "PricesUrl" %>"
  title: "<% "{index-content.actions.title}" %>"
  description: "<% "{index-content.actions.description}" %>"

release:
  title: "<% "{index-content.release_title}" %>"
  notes: "<% "{index-content.release_notes}" %>"
  downloads: "<% "{index-content.release_downloads}" %>"
  link: "<% "{products.nodejs-java.release_downloads}" %>"

code:
  title: "<% "{index-content-nodejs-java.code_title}" %>"
  more: "<% "{index-content.code_more}" %>"
  more_link: "<% dict "products.nodejs-java.more_link" %>"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    // <% "{index-content.code_comment_1}" %>
    const index = new Index('c:/MyIndex');

    // <% "{index-content.code_comment_2}" %>
    index.add('c:/MyDocuments');
    
    // <% "{index-content.code_comment_3}" %>
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "<% "{index-content.overview_title}" %>"
  description: "<% "{index-content-nodejs-java.overview_description}" %>"
  features:
    # feature loop
    - title: "<% "{index-content-nodejs-java.overview_feature_1.title}" %>"
      content: "<% "{index-content-nodejs-java.overview_feature_1.description}" %>"

    # feature loop
    - title: "<% "{index-content-nodejs-java.overview_feature_2.title}" %>"
      content: "<% "{index-content-nodejs-java.overview_feature_2.description}" %>"

    # feature loop
    - title: "<% "{index-content-nodejs-java.overview_feature_3.title}" %>"
      content: "<% "{index-content-nodejs-java.overview_feature_3.description}" %>"

    # feature loop
    - title: "<% "{index-content-nodejs-java.overview_feature_4.title}" %>"
      content: "<% "{index-content-nodejs-java.overview_feature_4.description}" %>"

############################# Platforms ############################
platforms:
  enable: true
  title: "<% "{index-content.platforms.title}" %>"
  description: "<% "{index-content-nodejs-java.platforms_description}" %>"
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
  title: "<% "{index-content.formats_title}" %>"
  description: |
    <% "{index-content-nodejs-java.formats_description}" %>
  groups:
    # group loop
    - color: "green"
      content: |
        ### <% "{index-content.formats_groups.title_1}" %>
        * **<% "{index-content.formats_groups.format_portable}" %>:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **<% "{index-content.formats_groups.format_text}" %>:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### <% "{index-content.formats_groups.title_2}" %>
        * **<% "{index-content.formats_groups.format_popular_images}" %>:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **<% "{index-content.formats_groups.format_multi_images}" %>:** GIF, WEBP, TIFF
        * **<% "{index-content.formats_groups.format_multi_audio}" %>:** MP3, WAV
        * **<% "{index-content.formats_groups.format_multi_video}" %>:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### <% "{index-content.formats_groups.title_3}" %>
        * **<% "{index-content.formats_groups.format_email}" %>:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **<% "{index-content.formats_groups.format_web}" %>:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **<% "{index-content.formats_groups.format_others}" %>:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "<% "{index-content-nodejs-java.features.title}" %>"
  description: "<% "{index-content-nodejs-java.features.description}" %>"

  items:
    # feature loop
    - icon: "document_info"
      title: "<% "{index-content-nodejs-java.features.feature_1.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_1.content}" %>"

    # feature loop
    - icon: "detect"
      title: "<% "{index-content-nodejs-java.features.feature_2.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_2.content}" %>"

    # feature loop
    - icon: "collect"
      title: "<% "{index-content-nodejs-java.features.feature_3.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_3.content}" %>"

    # feature loop
    - icon: "get"
      title: "<% "{index-content-nodejs-java.features.feature_4.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_4.content}" %>"

    # feature loop
    - icon: "remove"
      title: "<% "{index-content-nodejs-java.features.feature_5.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_5.content}" %>"

    # feature loop
    - icon: "style"
      title: "<% "{index-content-nodejs-java.features.feature_6.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_6.content}" %>"

    # feature loop
    - icon: "detect"
      title: "<% "{index-content-nodejs-java.features.feature_7.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_7.content}" %>"

    # feature loop
    - icon: "manipulate"
      title: "<% "{index-content-nodejs-java.features.feature_8.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_8.content}" %>"

    # feature loop
    - icon: "compare"
      title: "<% "{index-content-nodejs-java.features.feature_9.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_9.content}" %>"

    # feature loop
    - icon: "unreadable_characters"
      title: "<% "{index-content-nodejs-java.features.feature_10.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_10.content}" %>"

    # feature loop
    - icon: "hidden_print"
      title: "<% "{index-content-nodejs-java.features.feature_11.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_11.content}" %>"

    # feature loop
    - icon: "style"
      title: "<% "{index-content-nodejs-java.features.feature_12.title}" %>"
      content: "<% "{index-content-nodejs-java.features.feature_12.content}" %>"

############################# Code samples ############################
code_samples:
  enable: true
  title: "<% "{index-content.code_samples.title}" %>"
  description: "<% "{index-content-nodejs-java.code_samples_description}" %>"
  items:
    # code sample loop
    - title: "<% "{index-content-nodejs-java.code_title_sample_1}" %>"
      content: |
        <% "{index-content-nodejs-java.code_samples_sample_1_content}" %>
        {{< landing/code title="<% "{index-content.code_samples.sample_1.code_title}" %>">}}
        ```javascript {style=abap}
        // <% "{index-content.code_samples.sample_1.comment_1}" %>
        const index = new Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // <% "{index-content.code_samples.sample_1.comment_2}" %>
        var options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // <% "{index-content.code_samples.sample_1.comment_3}" %>
        var query = "water OR \"Lorem ipsum\"";
        var result = index.search(query, options);
        
        // <% "{index-content.code_samples.sample_1.comment_4}" %>
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
    - title: "<% "{index-content-nodejs-java.code_title_sample_2}" %>"
      content: |
        <% "{index-content-nodejs-java.code_samples_sample_2_content}" %>
        {{< landing/code title="<% "{index-content.code_samples.sample_2.code_title}" %>">}}
        ```javascript {style=abap}   
        // <% "{index-content.code_samples.sample_2.comment_1}" %>
        const index = new Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // <% "{index-content.code_samples.sample_2.comment_2}" %>

        // <% "{index-content.code_samples.sample_2.comment_3}" %>
        var query = "^^(.)\\1{1,}";
        // <% "{index-content.code_samples.sample_2.comment_4}" %>
        var result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
