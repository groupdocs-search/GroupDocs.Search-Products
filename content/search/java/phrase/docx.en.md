
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:52
draft: false
lang: en
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Search phrases in DOCX using Java"
head_description: "GroupDocs.Search for Java enhances Java applications with advanced phrase search capabilities for document content."

############################# Header ############################
title: "Find phrases in documents" 
description: "Quickly locate specific phrases with GroupDocs.Search for Java. Add powerful search functionality to your Java applications."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search features"
    link: "/search/java/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) is a robust library for indexing and searching text within documents. It supports over 70 file formats, including PDFs, Word documents, Excel spreadsheets, images, and ZIP files, ensuring fast and precise search results.

############################# Steps ############################
steps:
    enable: true
    title: "How to find phrases in DOCX documents"
    content: |
      [GroupDocs.Search](/search/java/) simplifies phrase searching in DOCX documents. Use various options to refine search results in Java applications.
      
      1. Create a search index directory.
      2. Specify the folder with DOCX files.
      3. Adjust search parameters.
      4. Retrieve and analyze search results.
   
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
        // Define the search index path
        Index index = new Index("c:/MyIndex");

        // Specify the folder containing documents
        index.add("c:/MyDocuments");

        // Set search preferences
        SearchQuery word1 = SearchQuery.createWordQuery("lorem");
        SearchQuery word2 = SearchQuery.createWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.createWordQuery("dolor");

        SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, word2, word3);
        
        // Execute the search query
        SearchResult result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Explore Java document search engine"
  description: "GroupDocs.Search for Java allows phrase searches across 70+ file formats. Easily find and organize data using advanced search features."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Key capabilities of GroupDocs.Search"
  features:
    # feature loop
    - title: "Phrase search"
      content: "Locate exact phrases in business documents, such as PDFs, Word files, presentations, and spreadsheets. Use wildcards and other options when the exact phrase is unknown."

    # feature loop
    - title: "Optimized data indexing"
      content: "Speed up document searches by creating and reusing search indexes. Indexing organizes data efficiently for faster and more accurate searches."

    # feature loop
    - title: "Multi-language compatibility"
      content: "Search documents in over 80 languages. Supports different keyboard layouts and morphological analysis to improve search precision."

    # feature loop
    - title: "Advanced search options"
      content: "Customize searches with case sensitivity, fuzzy search, homophone matching, document filtering, and other powerful features."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utilizing advanced search methods"
      content: |
        Learn how to construct queries for searching in DOCX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Define the directory for the search index
          Index index = new Index("c:/MyIndex");
              
          // Set the path to the target documents
          index.add("c:/MyDocuments");

          // Create a search query for a specific phrase
          SearchQuery word1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.createWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.createWordQuery("dolor");

          SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Fetch the search results
          SearchResult result = index.search(query);
          
          // Process and utilize the retrieved results
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
            link: "/examples/search/formats/searchphrase.docx"
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
    title: "Advanced search capabilities"
    exclude: "phrase"
    description: "Utilize cutting-edge search functionalities for improved accuracy and performance."
    items: 
          
        # operation loop 1
        - name: "Search by condition"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "Find information in documents using boolean conditions"

        # operation loop 2
        - name: "Case-sensitive search"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "Improve search accuracy by considering case sensitivity"

        # operation loop 3
        - name: "Document indexing"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "Index documents once and reuse the index for multiple searches"

        # operation loop 4
        - name: "Search filters"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "Use filters to narrow down the data being processed"

        # operation loop 5
        - name: "Exact phrase"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "Search for a specific sentence or phrase"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Search phrases in business documents"
    exclude: "DOCX"
    description: "GroupDocs.Search enables phrase searches in 70+ document formats. Leverage advanced options and indexing for efficient searches."
    items: 
        # format loop 1
        - name: "DOCX phrase search"
          format: "DOCX"
          link: "/search/java/phrase/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "PDF phrase search"
          format: "PDF"
          link: "/search/java/phrase/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "PPTX phrase search"
          format: "PPTX"
          link: "/search/java/phrase/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "TXT phrase search"
          format: "TXT"
          link: "/search/java/phrase/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "XLSX phrase search"
          format: "XLSX"
          link: "/search/java/phrase/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---