
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:40
draft: false
lang: en
format: Pdf
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Search phrases in PDF using Node.js"
head_description: "GroupDocs.Search for Node.js via Java adds powerful phrase search functionality to JavaScript applications for efficient document search."

############################# Header ############################
title: "Find phrases in documents" 
description: "Quickly locate specific phrases with GroupDocs.Search for Node.js via Java. Integrate fast and accurate search capabilities into your Node.js applications."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search features"
    link: "/search/nodejs-java/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) is a high-performance library for indexing and searching text in documents. It supports over 70 file formats, including PDFs, Word documents, Excel spreadsheets, images, and ZIP archives, ensuring accurate and fast search results.

############################# Steps ############################
steps:
    enable: true
    title: "How to find phrases in PDF documents"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) makes phrase searching in PDF documents easy. Apply different search options to refine results in Node.js via Java applications.
      
      1. Set up a search index folder.
      2. Define the folder containing PDF files.
      3. Configure search parameters.
      4. Retrieve and process search results.
   
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

        // Specify the path for storing the search index
        const index = new searchLib.Index("c:/MyIndex");

        // Set the folder containing documents
        index.add("c:/MyDocuments");

        // Configure search settings
        const word1 = searchLib.SearchQuery.createWordQuery("lorem");
        const word2 = searchLib.SearchQuery.createWordQuery("ipsum");
        const word3 = searchLib.SearchQuery.createWordQuery("dolor");

        const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, word2, word3);

        // Run the search query
        const result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Discover Node.js document search engine"
  description: "GroupDocs.Search for Node.js via Java enables phrase searches across 70+ file formats, making it easy to find and organize data with advanced search features."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Key capabilities of GroupDocs.Search"
  features:
    # feature loop
    - title: "Phrase search"
      content: "Find exact phrases in business documents like PDFs, Word files, presentations, and spreadsheets. Use wildcards and flexible search options when the full phrase is unknown."

    # feature loop
    - title: "Optimized data indexing"
      content: "Boost search performance by creating reusable indexes. Structured indexing speeds up document searches and improves accuracy."

    # feature loop
    - title: "Multi-language compatibility"
      content: "Search documents in over 80 languages with support for different keyboard layouts and morphological word variations, ensuring precise results."

    # feature loop
    - title: "Advanced search options"
      content: "Customize searches with case sensitivity, fuzzy matching, homophone detection, document filtering, and other powerful features."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Using advanced search techniques"
      content: |
        Learn how to construct queries for searching in PDF.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Define the search index directory
          const index = new searchLib.Index("c:/MyIndex");
              
          // Set the path to the target documents
          index.add("c:/MyDocuments");

          // Create a query for the desired phrase
          const word1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wildcard = searchLib.SearchQuery.createWildcardQuery(1, 7);
          const word2 = searchLib.SearchQuery.createWordQuery("dolor");

          const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Retrieve the search results
          const result = index.search(query);
          
          // Process and use the results
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
            link: "/examples/search/formats/searchphrase.pdf"
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
    title: "Advanced search capabilities"
    exclude: "phrase"
    description: "Leverage powerful search features for faster and more accurate results."
    items: 
          
        # operation loop 1
        - name: "Search by condition"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "Find information in documents using boolean conditions"

        # operation loop 2
        - name: "Case-sensitive search"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "Improve search accuracy by considering case sensitivity"

        # operation loop 3
        - name: "Document indexing"
          operation: "document"
          link: "/search/nodejs-java/document/pdf/"
          description: "Index documents once and reuse the index for multiple searches"

        # operation loop 4
        - name: "Search filters"
          operation: "filters"
          link: "/search/nodejs-java/filters/pdf/"
          description: "Use filters to narrow down the data being processed"

        # operation loop 5
        - name: "Exact phrase"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "Search for a specific sentence or phrase"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Search phrases in business documents"
    exclude: "PDF"
    description: "GroupDocs.Search supports phrase searches in 70+ document formats. Use advanced options and indexing to streamline the search process."
    items: 
        # format loop 1
        - name: "DOCX phrase search"
          format: "DOCX"
          link: "/search/nodejs-java/phrase/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "PDF phrase search"
          format: "PDF"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "PPTX phrase search"
          format: "PPTX"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "TXT phrase search"
          format: "TXT"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "XLSX phrase search"
          format: "XLSX"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---