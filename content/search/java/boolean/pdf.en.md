
---
############################# Static ############################
layout: "format"
date:  2025-01-23T14:09:57
draft: false
lang: en
format: Pdf
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Boolean search in PDF with Java"
head_description: "With GroupDocs.Search for Java, developers can perform document searches using Boolean operators like AND, OR, and NOT."

############################# Header ############################
title: "Boolean text search" 
description: "Use GroupDocs.Search for Java to create advanced boolean (AND, OR, NOT) search queries in your Java projects with ease."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download for Free"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Search"
    link: "/search/java/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) is a versatile library designed for text search and data indexing in documents. It supports over 70 file types, including PDF, Word, Excel, images, and ZIP archives, enabling efficient searches through large data collections.

############################# Steps ############################
steps:
    enable: true
    title: "How to perform boolean searches in PDF documents"
    content: |
      [GroupDocs.Search](/search/java/) enables easy text searches within PDF documents. With support for boolean conditions, you can enhance search accuracy in Java applications.
      
      1. Specify the folder to store the search index.
      2. Select the folder containing PDF documents.
      3. Execute the search query and retrieve results.
      4. Process the obtained results.
   
    code:
      platform: "java"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Search result"
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
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // Set the path for the index folder
        Index index = new Index("c:/MyIndex");

        // Provide the folder path containing documents for the search
        index.add("c:/MyDocuments");

        // Run a search with a complex query
        SearchResult result = index.search("theory AND relativity");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Powerful tools for document search and indexing"
  description: "GroupDocs.Search for Java simplifies text searches and data indexing for over 70 formats. Its advanced tools let you find and manage content effortlessly."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Key features of GroupDocs.Search"
  features:
    # feature loop
    - title: "Comprehensive text search"
      content: "Search across multiple formats like PDFs, Word documents, spreadsheets, and more. Use options such as exact matching, fuzzy search, and wildcard queries to refine results."

    # feature loop
    - title: "Efficient data indexing"
      content: "Build and maintain indexes for faster document searches. This feature organizes data efficiently, making it easy to handle large document collections."

    # feature loop
    - title: "Multi-language support"
      content: "Search in documents written in over 80 languages. Enhance accuracy by leveraging morphological word forms and different keyboard layouts."

    # feature loop
    - title: "Flexible search customization"
      content: "Adjust search settings with features like case sensitivity, date range filters, and exclusions to refine your results."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Using complex boolean search queries"
      content: |
        This example demonstrates how to perform Boolean searches in PDF files.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Set the folder for the search index
          Index index = new Index("c:/MyIndex");
              
          // Provide the path to the documents to search
          index.add("c:/MyDocuments");

          // Construct the query using Boolean logic
          SearchQuery wordQuery1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.createWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Retrieve the search results
          SearchResult result = index.search(booleanQuery);
          
          // Process the retrieved results
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "Copy"
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
          copy_tip: "click to copy"
          copy_done: "copied"
        top_links:
          #  loop
          - title: "Download result"
            icon: "download"
            link: "/examples/search/formats/search_boolean.pdf"
        links:
          #  loop
          - title: "More examples"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Search features for free or request a license"
  items:
    #  loop
    - title: "Maven download"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Key features at a glance"
    exclude: "boolean"
    description: "Unlock powerful and efficient search capabilities"
    items: 
          
        # operation loop 1
        - name: "Search by condition"
          operation: "boolean"
          link: "/search/java/boolean/pdf/"
          description: "Find information in documents using boolean conditions"

        # operation loop 2
        - name: "Case-sensitive search"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pdf/"
          description: "Improve search accuracy by considering case sensitivity"

        # operation loop 3
        - name: "Document indexing"
          operation: "document"
          link: "/search/java/document/pdf/"
          description: "Index documents once and reuse the index for multiple searches"

        # operation loop 4
        - name: "Search filters"
          operation: "filters"
          link: "/search/java/filters/pdf/"
          description: "Use filters to narrow down the data being processed"

        # operation loop 5
        - name: "Exact phrase"
          operation: "phrase"
          link: "/search/java/phrase/pdf/"
          description: "Search for a specific sentence or phrase"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Search popular document formats"
    exclude: "PDF"
    description: "GroupDocs.Search supports over 70 file formats, enabling you to customize search rules and use indexing to optimize performance."
    items: 
        # format loop 1
        - name: "Search in DOCX"
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Search in PDF"
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Search in PPTX"
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Search in TXT"
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "Search in XLSX"
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---