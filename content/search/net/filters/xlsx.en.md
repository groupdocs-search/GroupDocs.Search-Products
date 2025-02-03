
---
############################# Static ############################
layout: "format"
date:  2025-02-03T21:11:53
draft: false
lang: en
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Search in XLSX documents using .NET"
head_description: "GroupDocs.Search for .NET enhances C# applications with efficient text search across various business document formats."

############################# Header ############################
title: "Search for text in business documents" 
description: "GroupDocs.Search for .NET enables powerful and flexible text searches in your documents. Easily integrate search functionality into .NET applications."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download for free"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "What is GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) is a powerful library for efficient text search and document indexing. It supports over 70 file formats, including industry-standard documents such as PDF, Word, Excel, and PowerPoint. Improve search performance with fast and accurate results.

############################# Steps ############################
steps:
    enable: true
    title: "How to search in XLSX data"
    content: |
      [GroupDocs.Search](/search/net/) enables efficient text searches in XLSX documents, making it ideal for .NET applications.
      
      1. Set up a folder for storing the search index.
      2. Select the folder containing your files.
      3. Configure search options to process only XLSX documents.
      4. Execute the search and retrieve results.
   
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
        // Path to store the reusable search index
        Index index = new Index("c:/MyIndex");

        // Folder containing documents
        index.Add("c:/MyDocuments");

        // Search only within specific file formats
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".xlsx");

        // Retrieve search results
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Advanced searching features"
  description: "GroupDocs.Search for .NET enables sophisticated text searches across more than 70 file formats. Indexing improves search efficiency and helps manage document content effectively."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Main features of GroupDocs.Search"
  features:
    # feature loop
    - title: "Advanced text search"
      content: "Extract relevant text from popular business documents, including PDFs, Word files, presentations, and spreadsheets. Supports multiple search techniques such as fuzzy search, homophone detection, and wildcards."

    # feature loop
    - title: "Optimized indexing for faster searches"
      content: "Build and reuse search indexes to enhance search speed. Indexing optimizes performance when searching through large document collections."

    # feature loop
    - title: "Support for multiple languages"
      content: "Perform searches in documents written in over 80 languages. Detects different keyboard layouts and word variations to improve accuracy."

    # feature loop
    - title: "Flexible search settings"
      content: "Refine search results with customizable options, including filters, regular expressions, and case sensitivity settings."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filter documents to be processed"
      content: |
        Learn how to narrow down document searches using filters
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Set up an index that excludes certain file formats
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.CreateFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter);
          settings.DocumentFilter = invertedFilter;

          Index index = new Index("c:/MyIndex", settings);
              
          // Specify the document directory
          index.Add("c:/MyDocuments");

          // Retrieve search results
          SearchResult result = index.Search("Lorem");
          
          // Process and use the search output
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
            link: "/examples/search/formats/searchfilters.xlsx"
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
    title: "Key features"
    exclude: "filters"
    description: "Perform accurate and efficient data searches."
    items: 
          
        # operation loop 1
        - name: "Search by condition"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "Find information in documents using boolean conditions"

        # operation loop 2
        - name: "Case-sensitive search"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Improve search accuracy by considering case sensitivity"

        # operation loop 3
        - name: "Document indexing"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "Index documents once and reuse the index for multiple searches"

        # operation loop 4
        - name: "Search filters"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "Use filters to narrow down the data being processed"

        # operation loop 5
        - name: "Exact phrase"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "Search for a specific sentence or phrase"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Find data in your business documents"
    exclude: "XLSX"
    description: "GroupDocs.Search supports 70+ file formats, allowing efficient processing and searching of popular office documents."
    items: 
        # format loop 1
        - name: "Search in DOCX"
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Search in PDF"
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Search in PPTX"
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Search in TXT"
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "Search in XLSX"
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---