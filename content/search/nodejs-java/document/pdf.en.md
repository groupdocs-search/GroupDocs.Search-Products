
---
############################# Static ############################
layout: "format"
date:  2025-01-29T16:07:41
draft: false
lang: en
format: Pdf
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Find text in PDF with GroupDocs.Search in Node.js"
head_description: "Use GroupDocs.Search for Node.js via Java with JavaScript to search text efficiently in various document formats."

############################# Header ############################
title: "Smart document search solution" 
description: "Easily locate text in different document formats using GroupDocs.Search for Node.js via Java. Create advanced search queries within your Node.js applications."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Try for Free"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Introduction to GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) is a high-performance library for full-text search and document indexing. It supports 70+ file types, including PDF, Word, Excel, images, and ZIP archives, ensuring fast and accurate results.

############################# Steps ############################
steps:
    enable: true
    title: "Perform search in PDF files"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) allows you to execute searches in PDF files, refining results in Node.js via Java applications.
      
      1. Define a storage folder for the search index.
      2. Select a folder with PDF files.
      3. Set additional search parameters.
      4. Run the search and analyze results.
   
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

        // Specify the directory for search index storage
        const index = new searchLib.Index("c:/MyIndex");

        // Choose the folder containing documents to search
        index.add("c:/MyDocuments");

        // Enable homophone search for words that sound similar
        const options = new SearchOptions();
        options.setUseHomophoneSearch(true);

        // Run a complex search query
        const result = index.search("metis");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Advanced search & indexing capabilities"
  description: "GroupDocs.Search for Node.js via Java provides powerful text search and indexing tools across 70+ document formats, making it easy to find and organize information."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Key Benefits of GroupDocs.Search"
  features:
    # feature loop
    - title: "Comprehensive text search"
      content: "Locate text in multiple document types, including PDFs, Word files, and spreadsheets. Use exact matches, fuzzy search, and wildcards for refined results."

    # feature loop
    - title: "Efficient indexing for large data"
      content: "Speed up searches by creating structured indexes, making it easier to retrieve information from large document collections."

    # feature loop
    - title: "Supports 80+ languages"
      content: "Search across documents in different languages, with automatic recognition of various word forms and keyboard layouts."

    # feature loop
    - title: "Custom search settings"
      content: "Adjust search options such as case sensitivity, date filters, and word exclusions to get precise results."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Using search for PDF documents"
      content: |
        This example shows how to use search queries within PDF documents.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Set the directory for search indexing
          const index = new searchLib.Index("c:/MyIndex");
              
          // Provide the file path for document storage
          index.add("c:/MyDocuments");

          // Enter the password for protected files
          index.getDictionaries().getDocumentPasswords().add("protected.pdf", '123456');

          // Enable fuzzy search for similar word detection
          const options = new SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new searchLib.SimilarityLevel(0.8));

          // Extract search results
          const result = index.Search("Loarem", options);
          
          // Process and review the results
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
            link: "/examples/search/formats/searchdocument.pdf"
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
    title: "Explore key features"
    exclude: "document"
    description: "Discover high-speed search features designed to enhance efficiency and accuracy."
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
    title: "Search in a variety of documents"
    exclude: "PDF"
    description: "GroupDocs.Search works with over 70 file formats, including office documents, ensuring quick and accurate searches with indexing support."
    items: 
        # format loop 1
        - name: "Search in DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/document/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Search in PDF"
          format: "PDF"
          link: "/search/nodejs-java/document/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Search in PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/document/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Search in TXT"
          format: "TXT"
          link: "/search/nodejs-java/document/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "Search in XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---