
---
############################# Static ############################
layout: "format"
date:  2025-02-03T21:11:53
draft: false
lang: en
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Search in TXT documents using Node.js"
head_description: "GroupDocs.Search for Node.js via Java adds fast and accurate text search capabilities to JavaScript applications, supporting multiple document formats."

############################# Header ############################
title: "Find text in business documents" 
description: "GroupDocs.Search for Node.js via Java provides powerful and flexible search functionality for documents. Easily integrate text search into Node.js applications."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download for free"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "What is GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) is a robust search and indexing library that enables fast text retrieval in documents. It supports over 70 file formats, including PDFs, Word, Excel, and PowerPoint, ensuring precise and efficient searches.

############################# Steps ############################
steps:
    enable: true
    title: "How to perform a search in TXT documents"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) makes searching text in TXT documents simple and efficient for Node.js via Java applications.
      
      1. Create a directory to store the search index.
      2. Choose the folder that contains the documents.
      3. Set search options to include only TXT files.
      4. Run the search and retrieve the results.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Search result"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // Define a directory for storing the search index
        const index = new searchLib.Index("c:/MyIndex");

        // Specify the folder containing searchable documents
        index.add("c:/MyDocuments");

        // Restrict search to specific file formats
        const options = new searchLib.SearchOptions();
        options.SearchDocumentFilter = 
            searchLib.SearchDocumentFilter.createFileExtension(".txt");

        // Retrieve and process search results
        const result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Advanced search capabilities"
  description: "GroupDocs.Search for Node.js via Java enhances document search efficiency by indexing over 70 file formats. Optimize content retrieval with advanced search techniques."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Key features of GroupDocs.Search"
  features:
    # feature loop
    - title: "Comprehensive text search"
      content: "Extract and locate text in popular document formats, such as PDFs, Word files, spreadsheets, and presentations. Supports fuzzy search, homophones, and wildcard queries."

    # feature loop
    - title: "Optimized indexing for performance"
      content: "Accelerate searches by creating reusable indexes. Enhances speed and efficiency when working with large document collections."

    # feature loop
    - title: "Multi-language support"
      content: "Search through documents in over 80 languages. Recognizes keyboard layouts and word variations for better accuracy."

    # feature loop
    - title: "Customizable search options"
      content: "Fine-tune search results with filters, regular expressions, case sensitivity, and other flexible settings."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filter searchable documents"
      content: |
        Learn how to refine document searches using filters.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Configure an index to exclude unwanted file formats
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            searchLib.DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = 
            searchLib.DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new searchLib.Index("c:/MyIndex", settings);
              
          // Specify the directory containing documents
          index.add("c:/MyDocuments");

          // Process search output for further use
          const result = index.Search("Lorem", options);
          
          // Process search output for further use
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "Copy"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "click to copy"
          copy_done: "copied"
        top_links:
          #  loop
          - title: "Download result"
            icon: "download"
            link: "/examples/search/formats/searchfilters.txt"
        links:
          #  loop
          - title: "More examples"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Search features for free or request a license"
  items:
    #  loop
    - title: "NPM download"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Key functionalities"
    exclude: "filters"
    description: "Perform fast and precise text searches across documents."
    items: 
          
        # operation loop 1
        - name: "Search by condition"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Find information in documents using boolean conditions"

        # operation loop 2
        - name: "Case-sensitive search"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Improve search accuracy by considering case sensitivity"

        # operation loop 3
        - name: "Document indexing"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "Index documents once and reuse the index for multiple searches"

        # operation loop 4
        - name: "Search filters"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "Use filters to narrow down the data being processed"

        # operation loop 5
        - name: "Exact phrase"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Search for a specific sentence or phrase"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Search in diverse document formats"
    exclude: "TXT"
    description: "GroupDocs.Search supports over 70 file types, allowing efficient text search across various office and business documents."
    items: 
        # format loop 1
        - name: "Search in DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/filters/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Search in PDF"
          format: "PDF"
          link: "/search/nodejs-java/filters/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Search in PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/filters/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Search in TXT"
          format: "TXT"
          link: "/search/nodejs-java/filters/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "Search in XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---