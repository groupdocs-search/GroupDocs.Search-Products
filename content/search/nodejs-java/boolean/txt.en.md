
---
############################# Static ############################
layout: "format"
date:  2025-02-13T15:29:05
draft: false
lang: en
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Boolean TXT search via Node.js"
head_description: "Use GroupDocs.Search for Node.js via Java API to execute advanced searches in document content with boolean operators like AND, OR, and NOT, tailored for JavaScript developers."

############################# Header ############################
title: "Perform boolean logic searches" 
description: "With GroupDocs.Search for Node.js via Java, you can create advanced search queries using boolean operators (AND, OR, NOT) seamlessly within your Node.js environment."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download Now"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "What is GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) is a robust tool for searching and indexing text within documents. It supports over 70 formats like PDF, Word, Excel, PowerPoint, images, and ZIP files, making it easy to process large amounts of information efficiently.

############################# Steps ############################
steps:
    enable: true
    title: "How to search in TXT documents using boolean operators"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) allows you to search content in TXT files effectively. With boolean logic, you can refine your search queries in Node.js via Java applications for improved accuracy.
      
      1. Set up the folder to store the search index.
      2. Select the folder containing TXT files for the search.
      3. Run the search query and retrieve results.
      4. Process and analyze the search results.
   
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

        // Set the location for the index folder
        const index = new searchLib.Index("c:/MyIndex");

        // Specify the folder containing documents to search
        index.add("c:/MyDocuments");

        // Execute a search query with advanced logic
        const result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Powerful tools for document search and indexing"
  description: "GroupDocs.Search for Node.js via Java streamlines text search and indexing for over 70 file types, helping you find and manage information faster and with precision."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Key features of GroupDocs.Search"
  features:
    # feature loop
    - title: "Enhanced text search"
      content: "Find text quickly across various formats such as PDFs, Word documents, presentations, and spreadsheets. Use features like exact matches, wildcard searches, and fuzzy search for precise results."

    # feature loop
    - title: "Efficient data indexing"
      content: "Build and manage indexes to speed up searches in large document collections. Indexing ensures fast and structured access to your data."

    # feature loop
    - title: "Multilingual support"
      content: "Search in documents written in over 80 languages. Morphological support and keyboard layout compatibility enhance search results in different languages."

    # feature loop
    - title: "Flexible search settings"
      content: "Customize your search by enabling case sensitivity, applying date filters, or skipping specific words and data during indexing."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Example of advanced boolean search"
      content: |
        This example demonstrates how to create Boolean-based queries for searching content in TXT documents.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Define the folder for the search index
          const index = new searchLib.Index("c:/MyIndex");
              
          // Provide the location of the documents to search
          index.add("c:/MyDocuments");

          // Build a query using Boolean operators
          const wordQuery1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wordQuery2 = searchLib.SearchQuery.createWordQuery("ipsum");
          const booleanQuery = searchLib.SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Retrieve search results
          const result = index.search(booleanQuery);
          
          // Process and use the search results
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
            link: "/examples/search/formats/searchboolean.txt"
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
    title: "Key capabilities of GroupDocs.Search"
    exclude: "boolean"
    description: "Unlock advanced, efficient, and customizable search features."
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
    title: "Search popular document formats"
    exclude: "TXT"
    description: "GroupDocs.Search supports over 70 file formats, providing flexible search rules and efficient indexing to save time and effort."
    items: 
        # format loop 1
        - name: "Boolean search DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/boolean/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Boolean search PDF"
          format: "PDF"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Boolean search PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Boolean search TXT"
          format: "TXT"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "Boolean search XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---