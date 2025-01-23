<% configRef "..\\..\\configs\\index\\index.yml" %>
<% include "..\\..\\data\\family_data.md" %>
---
############################# Static ############################
layout: "family"
date:  <% date "utcnow" %>
draft: false

product: "Search"
product_tag: "search"

lang: <% lower ( get "lang") %>

############################# Head ############################
head_title: "<% "{index-content.head_title}" %>"
head_description: "<% "{index-content.head_description}" %>"

############################# Header ############################
title: "<% "{index-content.title}" %>"
description:  |
  <% "{index-content.description_1}" %>

  <% "{index-content.description_2}" %>

  <% "{index-content.description_3}" %>

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "<% "{index-content.platforms.head_title}" %>"
  title: "<% "{index-content.platforms.title}" %>"
  description: "<% "{index-content.platforms.description}" %>"
  details_link_title: "<% "{index-content.platforms.learn_more}" %>"

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
                    Atom <br> Visual Studio Code <br> <% "{index-content.platforms.any_other_text_editor}" %>
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats


############################# Features ###############################
features:
  enable: true
  title: "<% "{index-content.features.title}" %>"
  description: "<% "{index-content.features.description}" %>"

  items:
    # items loop
    - icon: "view"
      title: "<% "{index-content.features.feature_1.title}" %>"
      content: "<% "{index-content.features.feature_1.content}" %>"

    # items loop
    - icon: "manipulate"
      title: "<% "{index-content.features.feature_2.title}" %>"
      content: "<% "{index-content.features.feature_2.content}" %>"

    # items loop
    - icon: "merge"
      title: "<% "{index-content.features.feature_3.title}" %>"
      content: "<% "{index-content.features.feature_3.content}" %>"

    # items loop
    - icon: "additional"
      title: "<% "{index-content.features.feature_4.title}" %>"
      content: "<% "{index-content.features.feature_4.content}" %>"

############################# Code samples ############################
code_samples:
  enable: true
  title: "<% "{index-content.code_samples.index_title}" %>"
  description: "<% "{index-content.code_samples.index_description}" %>"
  items:
    # code sample loop
    - title: "<% "{index-content.code_samples.sample_index.title}" %>"
      content: |
       <% "{index-content.code_samples.sample_index.content}" %>
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // <% "{index-content.code_samples.sample_index.comment_1}" %>
            Index index = new Index("\\Index Folder");

            //<% "{index-content.code_samples.sample_index.comment_2}" %>
            index.Add("\\Documents Folder");

            //<% "{index-content.code_samples.sample_index.comment_3}" %>
            SearchOptions options = new SearchOptions();

            //<% "{index-content.code_samples.sample_index.comment_4}" %>
            SearchResult result = index.Search("ipsum dolor", options);

            //<% "{index-content.code_samples.sample_index.comment_5}" %>
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
            // <% "{index-content.code_samples.sample_index.comment_1}" %>
            Index index = new Index("\\Index Folder");

            //<% "{index-content.code_samples.sample_index.comment_2}" %>
            index.add("\\Documents Folder");

            //<% "{index-content.code_samples.sample_index.comment_3}" %>
            SearchOptions options = new SearchOptions();

            //<% "{index-content.code_samples.sample_index.comment_4}" %>
            SearchResult result = index.search("ipsum dolor", options);

            //<% "{index-content.code_samples.sample_index.comment_5}" %>
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

            // <% "{index-content.code_samples.sample_index.comment_1}" %>
            const index = new searchLib.Index('\\Index Folder');

            //<% "{index-content.code_samples.sample_index.comment_2}" %>
            index.add('\\Documents Folder');

            //<% "{index-content.code_samples.sample_index.comment_3}" %>
            const options = new searchLib.SearchOptions();

            //<% "{index-content.code_samples.sample_index.comment_4}" %>
            const result = index.search('ipsum dolor', options);

            //<% "{index-content.code_samples.sample_index.comment_5}" %>
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
  title: "<% "{index-content.formats.title}" %>"
  description: "<% "{index-content.formats.description}" %>"

############################# Metrics ###############################
metrics:
  enable: true
  title: "<% "{index-content.metrics.title}" %>"
  description: "<% "{index-content.metrics.description}" %>"

  items:
    # items loop
    - number: "70+"
      title: "<% "{index-content.metrics.item_1.title}" %>"
      content: "<% "{index-content.metrics.item_1.description}" %>"

    # items loop
    - number: "500k"
      title: "<% "{index-content.metrics.item_2.title}" %>"
      content: "<% "{index-content.metrics.item_2.description}" %>"

    # items loop
    - number: "12k"
      title: "<% "{index-content.metrics.item_3.title}" %>"
      content: "<% "{index-content.metrics.item_3.description}" %>"

    # items loop
    - number: "150+"
      title: "<% "{index-content.metrics.item_4.title}" %>"
      content: "<% "{index-content.metrics.item_4.description}" %>"


############################# Customers ###############################
customers:
  enable: true
  title: "<% "{index-content.customers.title}" %>"
  description: "<% "{index-content.customers.description}" %>"

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
  title: "<% "{index-content.actions.title}" %>"
  description: "<% "{index-content.actions.description_index}" %>"

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
  title: "<% "{index-content.faq.title}" %>"
  description: "<% "{index-content.faq.description}" %>"

  items:
    # items loop
    - question: "<% "{index-content.faq.item_1.question}" %>"
      answer: "<% "{index-content.faq.item_1.answer}" %>"

    # items loop
    - question: "<% "{index-content.faq.item_2.question}" %>"
      answer: "<% "{index-content.faq.item_2.answer}" %>"

    # items loop
    - question: "<% "{index-content.faq.item_3.question}" %>"
      answer: "<% "{index-content.faq.item_3.answer}" %>"

############################# App links ###############################
app_links:
  enable: true
  title: "<% "{index-content.app_links.title}" %>"
  description: "<% "{index-content.app_links.description}" %>"

  items:
    # items loop
    - title: "GroupDocs.Search Total"
      content: "<% "{index-content.app_links.item_1.content}" %>"
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/search/total"

    # items loop
    - title: "GroupDocs.Search Word"
      content: "<% "{index-content.app_links.item_2.content}" %>"
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/search/docx"

    # items loop
    - title: "GroupDocs.Search PDF"
      content: "<% "{index-content.app_links.item_3.content}" %>"
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/search/pdf"


---