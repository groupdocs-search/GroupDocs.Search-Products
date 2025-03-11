
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:34
draft: false
lang: en
format: Txt
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Find text in TXT docs with GroupDocs.Search for Java"
head_description: "GroupDocs.Search for Java helps Java developers quickly search text within various document formats."

############################# Header ############################
title: "Smart document text search" 
description: "With GroupDocs.Search for Java, you can seamlessly search and extract text from multiple document types in your Java applications."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Get Free Trial"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "What does GroupDocs.Search do?"
    link: "/search/java/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) is a robust document search and indexing library that supports over 70 file formats, including PDF, Word, PowerPoint, Excel, images, and ZIP archives. It enables fast, precise, and scalable search capabilities for large document collections.

############################# Steps ############################
steps:
    enable: true
    title: "Perform textual searches in TXT files"
    content: |
      [GroupDocs.Search](/search/java/) makes it easy to search TXT files using sophisticated logic and indexing, improving search accuracy in Java applications.
      
      1. Set up a directory to store the search index.
      2. Choose a folder containing TXT files.
      3. Define additional search options.
      4. Execute the search and analyze the results.
   
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
        // Set the directory for storing the search index
        Index index = new Index("c:/MyIndex");

        // Specify the folder containing searchable documents
        index.add("c:/MyDocuments");

        // Enable homophone search to match words with similar pronunciation
        SearchOptions options = new SearchOptions();
        options.setUseHomophoneSearch(true);

        // Execute an advanced search query
        SearchResult result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Enhanced search and indexing capabilities"
  description: "GroupDocs.Search for Java simplifies text searching and indexing across 70+ document formats, providing efficient tools to manage and retrieve information quickly."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Core Features of GroupDocs.Search"
  features:
    # feature loop
    - title: "Comprehensive text search"
      content: "Find text across multiple document formats like PDFs, Word documents, PowerPoint presentations, and spreadsheets. Use exact matches, fuzzy search, and wildcard operators for refined search results."

    # feature loop
    - title: "Optimized indexing for large data"
      content: "Create structured indexes to speed up searches, making it easy to navigate through extensive document repositories efficiently."

    # feature loop
    - title: "Supports multiple languages"
      content: "Perform searches in 80+ languages with built-in support for different keyboard layouts and word morphology variations, improving accuracy."

    # feature loop
    - title: "Flexible search settings"
      content: "Customize searches with options like case sensitivity, date-based filtering, and the ability to exclude specific words for precise results."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Implementing advanced search queries"
      content: |
        This example illustrates how to use search queries to search within TXT docs efficiently.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Define the directory for search indexing
          Index index = new Index("c:/MyIndex");
              
          // Provide the file path for the documents
          index.add("c:/MyDocuments");

          // Enter the password for encrypted documents
          index.getDictionaries().getDocumentPasswords().add("protected.txt", "123456");

          // Activate fuzzy search to detect similar words
          SearchOptions options = new SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8));

          // Fetch search results
          SearchResult result = index.Search("Loarem", options);
          
          // Process and analyze search results
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
            link: "/examples/search/formats/searchdocument.txt"
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
    title: "Key features overview"
    exclude: "document"
    description: "Discover high-performance text search functionalities designed for efficiency and precision."
    items: 
          
        # operation loop 1
        - name: "Search by condition"
          operation: "boolean"
          link: "/search/java/boolean/txt/"
          description: "Find information in documents using boolean conditions"

        # operation loop 2
        - name: "Case-sensitive search"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/txt/"
          description: "Improve search accuracy by considering case sensitivity"

        # operation loop 3
        - name: "Document indexing"
          operation: "document"
          link: "/search/java/document/txt/"
          description: "Index documents once and reuse the index for multiple searches"

        # operation loop 4
        - name: "Search filters"
          operation: "filters"
          link: "/search/java/filters/txt/"
          description: "Use filters to narrow down the data being processed"

        # operation loop 5
        - name: "Exact phrase"
          operation: "phrase"
          link: "/search/java/phrase/txt/"
          description: "Search for a specific sentence or phrase"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Find information across TXT documents with GroupDocs.Search"
    exclude: "TXT"
    description: "GroupDocs.Search supports over 70 formats, including office files, enabling fast searches with advanced indexing features."
    items: 
        # format loop 1
        - name: "Search in DOCX document"
          format: "DOCX"
          link: "/search/java/document/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Search in PDF document"
          format: "PDF"
          link: "/search/java/document/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Search in PPTX document"
          format: "PPTX"
          link: "/search/java/document/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Search in TXT document"
          format: "TXT"
          link: "/search/java/document/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "Search in XLSX document"
          format: "XLSX"
          link: "/search/java/document/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---