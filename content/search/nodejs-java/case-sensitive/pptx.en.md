
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:33
draft: false
lang: en
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Perform Case-Sensitive Searches in PPTX with Node.js"
head_description: "The GroupDocs.Search for Node.js via Java API allows JavaScript developers to execute case-sensitive searches across different document types."

############################# Header ############################
title: "Case-Sensitive Search" 
description: "GroupDocs.Search for Node.js via Java lets you easily implement advanced case-sensitive search functionality in your Node.js applications."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download for Free"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "What is GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) is a powerful library for searching and indexing text in documents. It supports over 70 formats, including PDFs, Word, Excel, PowePoint, images, and ZIP files, enabling efficient handling of large amounts of data.

############################# Steps ############################
steps:
    enable: true
    title: "Steps for Performing Case-Sensitive Searches in PPTX Files"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) makes it easy to carry out case-sensitive searches in PPTX files, enhancing your Node.js via Java workflows.
      
      1. Set up a folder to store the search index.
      2. Select the folder containing PPTX files.
      3. Run the search and get the results.
      4. Process and use the results.
   
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

        // Specify the path for the index folder
        const index = new searchLib.Index("c:/MyIndex");

        // Set the folder containing the documents to search
        index.add("c:/MyDocuments");

        // Enable case-sensitive search in the settings
        const options = new groupdocs.search.SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Execute the search
        const result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Key Features for Document Search and Indexing"
  description: "With GroupDocs.Search for Node.js via Java, you can easily search and index text in over 70 file formats. Access and organize information effortlessly using advanced search tools."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Core Features of GroupDocs.Search"
  features:
    # feature loop
    - title: "Comprehensive Text Search"
      content: "Find text in various document types like PDFs, Word files, spreadsheets, and presentations. Use options such as exact matches, fuzzy searches, and wildcards for accurate results."

    # feature loop
    - title: "Efficient Data Indexing"
      content: "Create and manage indexes to speed up searches. Indexing helps you organize and quickly locate data in large document collections."

    # feature loop
    - title: "Supports Multiple Languages"
      content: "Search documents in over 80 languages with support for diverse keyboard layouts and word variations, ensuring accurate search results."

    # feature loop
    - title: "Customizable Search Settings"
      content: "Adjust search settings, including case sensitivity, date filters, and exclusion of specific terms or data during indexing."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Example: Case-Sensitive Search Implementation"
      content: |
        This example demonstrates how to perform case-sensitive searches for PPTX documents.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Define the folder for the search index
          const index = new searchLib.Index("c:/MyIndex");
              
          // Provide the path to the document folder
          index.add("c:/MyDocuments");

          // Set up a search query
          const wordQuery = searchLib.SearchQuery.createWordQuery("Lorem");

          // Activate case-sensitive search settings
          const options = new groupdocs.search.SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Search for the text in documents
          const result = index.search(wordQuery, options);
          
          // Process and handle the results
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
            link: "/examples/search/formats/searchcase-sensitive.pptx"
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
    title: "Key Functionalities"
    exclude: "case-sensitive"
    description: "Explore advanced features for fast and precise document searching."
    items: 
          
        # operation loop 1
        - name: "Search by condition"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "Find information in documents using boolean conditions"

        # operation loop 2
        - name: "Case-sensitive search"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "Improve search accuracy by considering case sensitivity"

        # operation loop 3
        - name: "Document indexing"
          operation: "document"
          link: "/search/nodejs-java/document/pptx/"
          description: "Index documents once and reuse the index for multiple searches"

        # operation loop 4
        - name: "Search filters"
          operation: "filters"
          link: "/search/nodejs-java/filters/pptx/"
          description: "Use filters to narrow down the data being processed"

        # operation loop 5
        - name: "Exact phrase"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "Search for a specific sentence or phrase"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Compatible Document Formats"
    exclude: "PPTX"
    description: "GroupDocs.Search supports over 70 document formats. Customize your search options and save time with indexing."
    items: 
        # format loop 1
        - name: "DOCX case-sensitive search"
          format: "DOCX"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "PDF case-sensitive search"
          format: "PDF"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "PPTX case-sensitive search"
          format: "PPTX"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "TXT case-sensitive search"
          format: "TXT"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "XLSX case-sensitive search"
          format: "XLSX"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---