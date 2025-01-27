
---
############################# Static ############################
layout: "format"
date:  2025-01-27T20:14:10
draft: false
lang: en
format: Docx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Case-Sensitive Search in DOCX Using .NET"
head_description: "The GroupDocs.Search for .NET API enables C# developers to perform case-sensitive searches across various documents."

############################# Header ############################
title: "Case-Sensitive Search" 
description: "GroupDocs.Search for .NET makes it easy to create advanced case-sensitive search queries within your .NET applications."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download for Free"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "What is GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) is a robust library for text search and indexing in documents. It supports over 70 file formats, including PDF, Word, Excel, images, and ZIP files, ensuring efficient handling of large data volumes.

############################# Steps ############################
steps:
    enable: true
    title: "How to Perform Case-Sensitive Search in DOCX Documents"
    content: |
      [GroupDocs.Search](/search/net/) simplifies case-sensitive search in DOCX documents. Use it to refine results in .NET applications.
      
      1. Define the folder to store the search index.
      2. Choose the folder containing DOCX files.
      3. Run the search and retrieve results.
      4. Process the results.
   
    code:
      platform: "net"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Search result"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // Set the path to the index folder
        Index index = new Index("c:/MyIndex");

        // Specify the folder containing the documents to search
        index.Add("c:/MyDocuments");

        // Enable case-sensitive search in options
        SearchOptions options = new SearchOptions();
        options.UseCaseSensitiveSearch = true;

        // Run the search
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Advanced Features for Document Search and Indexing"
  description: "The GroupDocs.Search for .NET library simplifies text search and indexing across 70+ file formats. Easily locate and manage information with powerful search tools."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Key Features of GroupDocs.Search"
  features:
    # feature loop
    - title: "Advanced Text Search"
      content: "Search text across various file formats, including PDFs, Word documents, and spreadsheets. Use options like exact matches, fuzzy search, and wildcards for precise results."

    # feature loop
    - title: "Index Large Data Sets"
      content: "Build and maintain indexes for faster searches. Organized indexing simplifies searching extensive collections of documents."

    # feature loop
    - title: "Multi-Language Support"
      content: "Search across documents in over 80 languages, with support for different keyboard layouts and word forms for more accurate results."

    # feature loop
    - title: "Customizable Search Options"
      content: "Customize search settings with case sensitivity, date range filters, and the ability to exclude specific words or data during indexing."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Using Case-Sensitive Search Queries"
      content: |
        This example shows how to use case-sensitive queries for searching DOCX documents.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Set the folder for the search index
          Index index = new Index("c:/MyIndex");
              
          // Specify the path to the documents to be searched
          index.Add("c:/MyDocuments");

          // Create a search query
          SearchQuery wordQuery = SearchQuery.CreateWordQuery("Lorem");

          // Enable case-sensitive search options
          SearchOptions options = new SearchOptions();
          options.UseCaseSensitiveSearch = true;

          // Search for text in the documents
          SearchResult result = index.Search(wordQuery, options);
          
          // Process the search results
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "Copy"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "click to copy"
          copy_done: "copied"
        top_links:
          #  loop
          - title: "Download result"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.docx"
        links:
          #  loop
          - title: "More examples"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Search features for free or request a license"
  items:
    #  loop
    - title: "Nuget download"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Discover Key Features"
    exclude: "case-sensitive"
    description: "Explore advanced and efficient search functionalities."
    items: 
          
        # operation loop 1
        - name: "Search by condition"
          operation: "boolean"
          link: "/search/net/boolean/docx/"
          description: "Find information in documents using boolean conditions"

        # operation loop 2
        - name: "Case-sensitive search"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/docx/"
          description: "Improve search accuracy by considering case sensitivity"

        # operation loop 3
        - name: "Document indexing"
          operation: "document"
          link: "/search/net/document/docx/"
          description: "Index documents once and reuse the index for multiple searches"

        # operation loop 4
        - name: "Search filters"
          operation: "filters"
          link: "/search/net/filters/docx/"
          description: "Use filters to narrow down the data being processed"

        # operation loop 5
        - name: "Exact phrase"
          operation: "phrase"
          link: "/search/net/phrase/docx/"
          description: "Search for a specific sentence or phrase"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Search Popular Document Formats"
    exclude: "DOCX"
    description: "GroupDocs.Search supports over 70 file formats. Customize search rules and use indexing to save time and effort."
    items: 
        # format loop 1
        - name: "Search in DOCX"
          format: "DOCX"
          link: "/search/net/case-sensitive/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Search in PDF"
          format: "PDF"
          link: "/search/net/case-sensitive/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Search in PPTX"
          format: "PPTX"
          link: "/search/net/case-sensitive/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Search in TXT"
          format: "TXT"
          link: "/search/net/case-sensitive/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "Search in XLSX"
          format: "XLSX"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---