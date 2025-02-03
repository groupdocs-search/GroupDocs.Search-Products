
---
############################# Static ############################
layout: "format"
date:  2025-02-03T21:11:53
draft: false
lang: en
format: Pdf
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Search in PDF documents using Java"
head_description: "GroupDocs.Search for Java adds powerful text search to Java applications, supporting various business document formats."

############################# Header ############################
title: "Find text in business documents" 
description: "GroupDocs.Search for Java lets you search text in documents using flexible and precise queries. Easily integrate search functionality into Java applications."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download for free"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "What is GroupDocs.Search?"
    link: "/search/java/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) is a robust library for fast text search and document indexing. It supports over 70 file formats, including industry standards like PDF, Word, Excel, and PowerPoint. Enhance your applications with high-speed, accurate search capabilities.

############################# Steps ############################
steps:
    enable: true
    title: "How to search in PDF documents"
    content: |
      [GroupDocs.Search](/search/java/) allows fast and efficient text searches in PDF documents, perfect for Java applications.
      
      1. Specify a folder to store the search index.
      2. Select the folder containing your documents.
      3. Configure search options to limit results to PDF documents.
      4. Run the search and get results.
   
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
        // Directory to store the reusable search index
        Index index = new Index("c:/MyIndex");

        // Folder containing the documents
        index.add("c:/MyDocuments");

        // Filter searches by document format
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.createFileExtension(".pdf");

        // Retrieve search results
        SearchResult result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Enhanced search capabilities"
  description: "GroupDocs.Search for Java provides advanced text search across more than 70 file formats. Indexing speeds up searches and improves document management efficiency."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Key features of GroupDocs.Search"
  features:
    # feature loop
    - title: "Powerful text search"
      content: "Find text in popular document formats such as PDFs, Word files, presentations, and spreadsheets. Supports multiple search methods, including fuzzy search, homophones, and wildcards."

    # feature loop
    - title: "Optimized indexing for better performance"
      content: "Create and reuse search indexes to enhance search speed and efficiency, especially in large document collections."

    # feature loop
    - title: "Multilingual search support"
      content: "Search within documents written in over 80 languages. Detects different keyboard layouts and word variations for improved accuracy."

    # feature loop
    - title: "Customizable search options"
      content: "Narrow down search results with filters, regular expressions, and other advanced search settings."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filter documents before searching"
      content: |
        Learn how to refine searches using filters
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Set up an index that excludes certain file formats
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new Index("c:/MyIndex", settings);
              
          // Specify the document storage path
          index.add("c:/MyDocuments");

          // Retrieve search results
          SearchResult result = index.search("Lorem", options);
          
          // Process and use search results
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
            link: "/examples/search/formats/searchfilters.pdf"
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
    title: "Key features"
    exclude: "filters"
    description: "Perform precise and efficient text searches."
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
    title: "Search in business documents"
    exclude: "PDF"
    description: "GroupDocs.Search supports over 70 file formats, making it easy to search through widely used office documents."
    items: 
        # format loop 1
        - name: "Search in DOCX"
          format: "DOCX"
          link: "/search/java/filters/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Search in PDF"
          format: "PDF"
          link: "/search/java/filters/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Search in PPTX"
          format: "PPTX"
          link: "/search/java/filters/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Search in TXT"
          format: "TXT"
          link: "/search/java/filters/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "Search in XLSX"
          format: "XLSX"
          link: "/search/java/filters/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---