
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: en
format: Pdf
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Perform Case-Sensitive Searches in PDF with Java"
head_description: "The GroupDocs.Search for Java API helps Java developers run case-sensitive searches across multiple document types."

############################# Header ############################
title: "Case-Sensitive Document Search" 
description: "GroupDocs.Search for Java allows you to implement precise case-sensitive search functionality in your Java projects."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Get It for Free"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Learn About GroupDocs.Search"
    link: "/search/java/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) is a versatile tool for text search and indexing across various documents. It supports over 70 formats like PDFs, Word files, PowePoint presentations, Excel sheets, images, and ZIPs, enabling you to efficiently handle extensive datasets.

############################# Steps ############################
steps:
    enable: true
    title: "Guide to Case-Sensitive Search in PDF Files"
    content: |
      Using [GroupDocs.Search](/search/java/), you can easily perform case-sensitive searches in PDF documents, enhancing your Java projects.
      
      1. Set the folder for storing the search index.
      2. Select the folder containing PDF files.
      3. Run the case-sensitive search and collect results.
      4. Process and use the search results.
   
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
        // Define the location for the index storage
        Index index = new Index("c:/MyIndex");

        // Point to the folder containing documents to search
        index.add("c:/MyDocuments");

        // Enable case-sensitive mode in the search settings
        SearchOptions options = new SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Execute the search
        SearchResult result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Enhanced Search and Indexing Tools"
  description: "With GroupDocs.Search for Java, you can streamline document search and indexing for more than 70 formats, making it easier to locate and organize information."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Highlights of GroupDocs.Search"
  features:
    # feature loop
    - title: "Flexible Text Search"
      content: "Search through documents such as PDFs, Word files, spreadsheets, and presentations with ease. Use tools like exact match, fuzzy search, and wildcard support to refine your results."

    # feature loop
    - title: "Efficient Index Management"
      content: "Organize and index large datasets to improve search speed and performance when handling big document collections."

    # feature loop
    - title: "Support for Global Languages"
      content: "Perform searches in more than 80 languages, accommodating different keyboard layouts and linguistic variations for better accuracy."

    # feature loop
    - title: "Customizable Search Filters"
      content: "Adjust search criteria with options like case sensitivity, date range filtering, and exclusion of unwanted words or data during indexing."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Example: Case-Sensitive Search Queries"
      content: |
        This example demonstrates how to implement case-sensitive searches for PDF documents.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Define the directory for the search index
          Index index = new Index("c:/MyIndex");
              
          // Specify the location of the document folder
          index.add("c:/MyDocuments");

          // Set up a search query
          SearchQuery wordQuery = SearchQuery.createWordQuery("Lorem");

          // Activate case sensitivity in search options
          SearchOptions options = new SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Perform the document search
          SearchResult result = index.search(wordQuery, options);
          
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
            link: "/examples/search/formats/searchcase-sensitive.pdf"
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
    title: "Key Features Overview"
    exclude: "case-sensitive"
    description: "Discover the robust and effective search capabilities offered by GroupDocs.Search for Java."
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
    title: "Supported File Formats for Searching"
    exclude: "PDF"
    description: "GroupDocs.Search works with over 70 popular document formats, offering customizable search settings and efficient indexing."
    items: 
        # format loop 1
        - name: "DOCX case-sensitive search"
          format: "DOCX"
          link: "/search/java/case-sensitive/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "PDF case-sensitive search"
          format: "PDF"
          link: "/search/java/case-sensitive/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "PPTX case-sensitive search"
          format: "PPTX"
          link: "/search/java/case-sensitive/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "TXT case-sensitive search"
          format: "TXT"
          link: "/search/java/case-sensitive/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "XLSX case-sensitive search"
          format: "XLSX"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---